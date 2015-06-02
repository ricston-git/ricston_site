## About arrays

An array is an ordered data structure consisting of a collection of elements (values or variables), each identified by one (single dimensional array, or vector) or multiple indexes.

An [array](http://en.wikipedia.org/wiki/Array_data_type) is an ordered data structure consisting of a collection of elements (values or variables), each identified by at least one index, stored in contiguous memory locations. An array is typically stored so that the position of each element can be computed from its index tuple by a mathematical formula. In some languages (C, Java, etc.) the length of the array must be set beforehand. In other languages (Ruby, Python, LISP, etc.) the length of the array grows dynamically as elements are added.

When tagging a question with this tag, also tag the question with the programming language being used.

## Array in specific languages

### C#:

In [c#](http://stackoverflow.com/questions/tagged/c%23 "show questions tagged 'c#'"), arrays are actually objects, and not just addressable regions of contiguous memory as in C and C++. Array is the abstract base type of all array types. You can use the properties, and other class members, that Array has.

### C:

Arrays in [c](http://stackoverflow.com/questions/tagged/c "show questions tagged 'c'") act to store related data under a single variable name with an index, also known as a subscript. It is easiest to think of an array as simply a list or ordered grouping for variables of the same type. As such, arrays often help a programmer organize collections of data efficiently and intuitively.

### C++:

[c++](http://stackoverflow.com/questions/tagged/c%2b%2b "show questions tagged 'c++'") arrays are stored in row-major order. Row-major order means the last subscript varies the fastest.

### Ruby

In [ruby](http://stackoverflow.com/questions/tagged/ruby "show questions tagged 'ruby'") the normal array class is called an `Array`.

### Python

In [python](http://stackoverflow.com/questions/tagged/python "show questions tagged 'python'") the normal array datatype is called a `list`, while the [`array`](http://en.wikipedia.org/wiki/Array_data_type) type is used for homogeneous arrays.

### PHP

In [php](http://stackoverflow.com/questions/tagged/php "show questions tagged 'php'") arrays are implemented as ordered maps which may contain a mix of numeric or string keys.

### JavaScript

In [javascript](http://stackoverflow.com/questions/tagged/javascript "show questions tagged 'javascript'") arrays are just objects with a different prototype (with additional functions more useful for array-like structures), with numerical indexes stored as strings (all JavaScript keys are strings).

### Scala

In [scala](http://stackoverflow.com/questions/tagged/scala "show questions tagged 'scala'") normal array class is called Array. To get element from array you don't use square brackets as in most other languages but parentheses.

## Characteristics

Elements of an array are generally specified with a 0-first index, for example, `myarray[0]` would represent the first element of `myarray`. `myarray[l]` (where `l` is the length of the array minus 1) would represent the last element in the array. However, some languages such as old Fortran and Lua use 1 as the initial index.

Some languages ([c++](http://stackoverflow.com/questions/tagged/c%2b%2b "show questions tagged 'c++'"), [java](http://stackoverflow.com/questions/tagged/java "show questions tagged 'java'"), [c#](http://stackoverflow.com/questions/tagged/c%23 "show questions tagged 'c#'")) have "basic arrays" and collections. Basic arrays are supported by the compiler directly; have fixed size and only provide element access by index. Collections, like Java's [arraylist](http://stackoverflow.com/questions/tagged/arraylist "show questions tagged 'arraylist'"), are system library classes implemented on the top of these basic arrays and have a wide range of various methods. In such cases the tag `arrays` should be used to name the simple arrays.

Arrays can be statically allocated or dynamically allocated. The way in which you access the array and its type varies based on how it is declared and allocated.

Arrays can contain multiple indices. For example, an array with one index (e.g. `array[0]`) is known as a one dimensional array. If it has two indices (e.g. `array[0][0]`) it is considered two dimensional, and can be visualized as a grid.

## References

*   [Array Data Type (Wikipedia)](http://en.wikipedia.org/wiki/Array_data_type)
*   [Array Data Structure (Wikipedia)](http://en.wikipedia.org/wiki/Array_data_structure)
*   [Fundamental of Array and Q+A](http://introcs.cs.princeton.edu/java/14array/)

## Related tags

Where talking about specific variants of arrays, use these related tags instead.

*   [vector](http://stackoverflow.com/questions/tagged/vector "show questions tagged 'vector'")
*   [arraylist](http://stackoverflow.com/questions/tagged/arraylist "show questions tagged 'arraylist'")