## About linq

Language Integrated Query (LINQ) is a Microsoft .NET Framework component that adds native data querying capabilities to .NET languages.

LINQ is a .NET-based DSL (Domain Specific Language), introduced in [.net-3.5](http://stackoverflow.com/questions/tagged/.net-3.5 "show questions tagged '.net-3.5'"), for querying data sources such as databases, XML files or in-memory object lists. All these data sources can be queried using the exact same, readable and easy-to-use syntax - or rather, _syntaxes_, because LINQ supports two notations:

*   Inline LINQ or query syntax, where queries are expressed in a SQL-like language, with dialects in both [C#](http://msdn.microsoft.com/en-us/library/bb397676.aspx) and [VB.NET](http://msdn.microsoft.com/en-us/library/vstudio/bb763068.aspx).

*   Fluent LINQ or query operators, where queries are expressed as [lambda expressions](http://en.wikipedia.org/wiki/Anonymous_function#C.23_lambda_expressions) and can be linked (LINQed?) using a fluent syntax.

All LINQ query operations consist of three distinct actions: 1\. Obtain the data source. 2\. Create the query. 3\. Execute the query.

**Major Implementations:**

`.NET languages (C#, F#, VB.NET)`

**Some examples:**

_Fluent syntax (C#)_

    var result = dbContext.Products
                          .Where(p => p.Category.Name == "Toys" && p.Price >= 250)
                          .Select(p => p.Name);

_Query syntax (C#)_

    var result = from product in dbContext.Products
                 where product.Category.Name == "Toys"
                 where product.Price >= 2.50
                 select product.Name;

_Query syntax (VB.NET)_

    Dim result = From product in dbContext.Products _
                 Where product.Category.Name = "Toys" _
                 Where product.Price >= 2.50 _
                 Select product.Name

This query would return the name of all products in the "Toys" category with a price greater than or equal to 2.50.

**Flavors**

LINQ comes in many flavors, the most notable are

*   [LINQ to Objects](http://stackoverflow.com/tags/linq-to-objects/info) - For querying collections of POCO (Plain old CLR objects)
*   [LINQ to SQL](http://stackoverflow.com/tags/linq-to-sql/info) - For querying SQL databases
*   [LINQ to Entities](http://stackoverflow.com/tags/linq-to-entities/info) - For querying SQL databases through [Entity Framework](http://en.wikipedia.org/wiki/ADO.NET_Entity_Framework)
*   [LINQ to XML](http://stackoverflow.com/tags/linq-to-xml/info) - For querying XML documents
*   [PLINQ](http://stackoverflow.com/tags/plinq/info) - for querying in parallel.

LINQ has many extensions implemented online and a variety of extension open-source projects like [MORELINQ](https://code.google.com/p/morelinq/) which adds more operators to the _.NET_ operators, and many others.

There are other implementations of LINQ which can be found on the Internet, such as [LINQ to SharePoint](http://linqtosharepoint.codeplex.com/), [LINQ to Twitter](http://linqtotwitter.codeplex.com/), [LINQ to CSV](http://www.codeproject.com/Articles/25133/LINQ-to-CSV-library), [LINQ to Excel](https://code.google.com/p/linqtoexcel/), [LINQ to JSON](http://james.newtonking.com/json/help/html/LINQtoJSON.htm) and [LINQ to Google](http://www.codeplex.com/glinq).

Code Language (used for [syntax highlighting](http://google-code-prettify.googlecode.com/svn/trunk/README.html)): default

  default