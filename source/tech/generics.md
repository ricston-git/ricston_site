## About generics

Generics are a form of parametric polymorphism found in a range of languages, including .NET languages and in Java.

Generics are a language feature found in certain languages to enable a form of parametric polymorphism. They typically allow the programmer to express concepts such as "A list of some type T" in a type-safe manner. Prior to the addition of generics to the Java language and the .NET CLR, programmers using these languages were forced to downcast from the base `Object` when using some general purpose classes, such as collection classes.

With the addition of generics, the programmer can instead use types such as `List<int>` to create type-safe lists which only store `int` objects.

In-depth detail for examples and concepts specifically for C# Generics is provided by Microsoft [here](http://msdn.microsoft.com/en-us/library/512aeb7t(v=vs.80).aspx). Information on Java generics can be found [here](http://docs.oracle.com/javase/tutorial/extra/generics/index.html).

Unlike C++ templates, generics are typically limited to simple type substitution, without the ability of templates to specialize for specific types (infamously misused in the C++ standard library in `std::vector<bool>` which behaves radically different form any other `std::vector<T>`). This also means that generics are not well suited for [generic-programming](http://stackoverflow.com/questions/tagged/generic-programming "show questions tagged 'generic-programming'"), which typically relies on an ability to tailor generic algorithms for specific parameter types (again using a C++ example, pointers are usable with any generic algorithm expecting arguments to be iterators).

## Java Generic Tutorials

1.  [Java Generic methods and generic classes Tutorials](http://docs.oracle.com/javase/tutorial/extra/generics/index.html)
2.  [Java Generics FAQs](http://www.angelikalanger.com/GenericsFAQ/JavaGenericsFAQ.html)

## .NET Generic Tutorials

1.  [Introduction to Generics](http://msdn.microsoft.com/en-us/library/0x6a29h6.aspx)
2.  [C# Generics](http://www.tutorialspoint.com/csharp/csharp_generics.htm)