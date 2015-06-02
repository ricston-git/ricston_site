title: 'Do any proven, enterprise-grade, transactional, ACID compliant JSON database engines exist?'
date: 2015-05-31 12:19:26
tags:
- acid
- postgress
- json
- richard.donovan
---


## Do any proven, enterprise-grade, transactional, ACID compliant JSON database engines exist?

Companies face the constant challenge to modernize their stack and allow them to take advantage of a new web technologies. Typical roadmap adoption includes
* nodejs/micro servcies replacing older php/java and .asp stacks
* json replacing xml and other forms of information inter-change
* adoption of nosql key value and document stores.

However when challenged to find a "enterprise-grade, transactional, ACID compliant JSON database" our seach took us through the usual modern suspects from couchbase, mongo, redis and manny more. All of these proved to be excellent products in their own right when it came to performance, scaling and replication. Where they all fell short was the managing (acid) transactions.

After reviewing many compromise and increasingly complex solutions the surprising answer came to us from a traditional technology we knew well. Postgres Sql Datbase or it's commercially  supported variant EnterpriseDB

## Customer Win-Win (and win)
The big win-win for our partner client is that they already had existing sql data as well as support and maintenance skills, so introducing Postgres was the least disruptive option.

In addition Postgres ended up solving a number of other roadmap goals including moving to more cost effective and open source solutions improved performance over the legacy systems




## Postgres/EnterpriseDb Json
Below is an example of basic json crud operations on a postgres sql database
* create a table and populate with json data
* select and update on the data

# Creating Json Data
```
CREATE TABLE books ( id integer, data json );

INSERT INTO books VALUES (1,
  '{ "name": "Book the First", "author": { "first_name": "Bob", "last_name": "White" } }');
INSERT INTO books VALUES (2,
  '{ "name": "Book the Second", "author": { "first_name": "Charles", "last_name": "Xavier" } }');
INSERT INTO books VALUES (3,
  '{ "name": "Book the Third", "author": { "first_name": "Jim", "last_name": "Brown" } }');
```


Selecting

You can use the JSON operators to pull values out of JSON columns:
```
SELECT id, data->>'name' AS name FROM books;
```

returns
```
 id |      name
----+-----------------
  1 | Book the First
  2 | Book the Second
  3 | Book the Third
```

The `->` operator returns the original JSON type (which might be an object), whereas ->> returns text. You can use the -> to return a nested object and thus chain the operators:

```
SELECT id, data->'author'->>'first_name' as author_first_name FROM books;
```
returns

```
 id | author_first_name
----+-------------------
  1 | Bob
  2 | Charles
  3 | Jim
```


## Filtering

Treating json as a clob would be very limiting however Postgres is not like that
You can also select rows based on a value inside your JSON:

```
SELECT * FROM books WHERE data->>'name' = 'Book the First';
```

returns

```
 id |                                         data
----+---------------------------------------------------------------------------------------
  1 | '{ "name": "Book the First", "author": { "first_name": "Bob", "last_name": "White" } }'
```

You can also find rows based on the value of a nested JSON object:

```
SELECT * FROM books WHERE data->'author'->>'first_name' = 'Charles';

 id |                                            data
----+---------------------------------------------------------------------------------------------
  2 | '{ "name": "Book the Second", "author": { "first_name": "Charles", "last_name": "Xavier" } }'

```

## Indexing

You can add indexes on any of these using PostgreSQL’s expression indexes, which means you can even add unique constraints based on your nested JSON data:

```
CREATE UNIQUE INDEX books_author_first_name ON books ((data->'author'->>'first_name'));
```
and

```
INSERT INTO books VALUES (4,
  '{ "name": "Book the Fourth", "author": { "first_name": "Charles", "last_name": "Davis" } }');
ERROR:  duplicate key value violates unique constraint "books_author_first_name"
DETAIL:  Key (((data -> 'author'::text) ->> 'first_name'::text))=(Charles) already exists.
```

Expression indexes are somewhat expensive to create, but once in place will make querying on any JSON property very fast.

## Even Table Data to Json

The simplest way to return JSON is with row_to_json() function. It accepts a row value and returns a JSON value.
```
select row_to_json(words) from words;
```

This will return a single column per row in the words table.
```
{"id":6013,"text":"advancement","pronunciation":"advancement",...}
```
