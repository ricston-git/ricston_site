## About class

A template for creating new objects that describes the common state(s) and behavior(s). NOT TO BE CONFUSED WITH CSS CLASSES. Use [css] instead.

**Not to be confused with CSS classes.** Use [css](http://stackoverflow.com/questions/tagged/css "show questions tagged 'css'") instead.

* * *

In [object-oriented programming](http://en.wikipedia.org/wiki/Object-oriented_programming) (see: [oop](http://stackoverflow.com/questions/tagged/oop "show questions tagged 'oop'")), a class is a construct that is used as a **blueprint** (or a **template**) to create objects of that class. This blueprint describes the **state** and **behavior** that the objects of the class all share. An object of a given class is called an **instance** of the class. The class that contains (and was used to create) that instance can be considered as the **type** of that object, e.g. an object instance of the `Fruit` class would be of the type `Fruit`.

A class usually represents a noun, such as a person, place or (possibly quite abstract) thing - it is a model of a concept within a computer program. Fundamentally, it encapsulates the state and behavior of the concept it represents. It encapsulates state through data placeholders called **attributes** (or member variables or instance variables or fields); it encapsulates behavior through reusable sections of code called **methods**.

More technically, a class is a cohesive package that consists of a particular kind of metadata. A class has both an **interface** and a **structure**. The interface describes how to interact with the class and its instances using methods, while the structure describes how the data is partitioned into attributes within an instance. A class may also have a representation (metaobject) at run time, which provides run time support for manipulating the class-related metadata. In object-oriented design, a class is the most specific type of an object in relation to a specific layer.

Example of class declaration in C#:

    /// <summary>
    /// Class which objects will say "Hello" to any target :)
    /// </summary>
    class HelloAnything
    {
        /// <summary>
        /// Target for "Hello". Private attribute that will be set only once
        ////when object is created. Only objects of this class can access
        /// their own target attribute.
        /// </summary>
        private readonly string target;

        /// <summary>
        /// Constructor. Code that will execute when instance of class is created.
        /// </summary>
        /// <param name="target">Target for "Hello". If nothing specified then
        /// will be used default value "World".</param>
        public HelloAnything(string target = "World")
        {
            //Save value in the inner attribute for using in the future.
            this.target = target;
        }

        /// <summary>
        /// Returns phrase with greeting to the specified target.
        /// </summary>
        /// <returns>Text of greeting.</returns>
        public string SayHello()
        {
            return "Hello, " + target + "!";
        }
    }

Using example of the defined class:

    class Program
    {
        static void Main(string[] args)
        {
            //Say hello to the specified target.
            HelloAnything greeting = new HelloAnything("Stack Overflow");
            Console.WriteLine(greeting.SayHello());

            //Say hello to the "default" target.
            greeting = new HelloAnything();
            Console.WriteLine(greeting.SayHello());
        }
    }

Output result:

    Hello, Stack Overflow!
    Hello, World!

Computer programs usually model aspects of some real or abstract world (the Domain). Because each class models a concept, classes provide a more natural way to create such models. Each class in the model represents a noun in the domain, and the methods of the class represent verbs that may apply to that noun.

For example in a typical business system, various aspects of the business are modelled, using such classes as `Customer`, `Product`, `Worker`, `Invoice`, `Job`, etc. An `Invoice` may have methods like `Create`, `Print` or `Send`, a `Job` may be `Perform`-ed or `Cancel`-led, etc.

Once the system can model aspects of the business accurately, it can provide users of the system with useful information about those aspects. Classes allow a clear correspondence (mapping) between the model and the domain, making it easier to design, build, modify and understand these models. Classes provide some control over the often challenging complexity of such models.

Classes can accelerate development by reducing redundant program code, testing and bug fixing. If a class has been thoroughly tested and is known to be a 'solid work', it is usually true that using or extending the well-tested class will reduce the number of bugs - as compared to the use of freshly-developed or ad hoc code - in the final output. In addition, efficient class reuse means that many bugs need to be fixed in only one place when problems are discovered.

Another reason for using classes is to simplify the relationships of interrelated data. Rather than writing code to repeatedly call a graphical user interface (GUI) window drawing subroutine on the terminal screen (as would be typical for structured programming), it is more intuitive. With classes, GUI items that are similar to windows (such as dialog boxes) can simply inherit most of their functionality and data structures from the window class. The programmer then need only add code to the dialog class that is unique to its operation. Indeed, GUIs are a very common and useful application of classes, and GUI programming is generally much easier with a good class framework.

_Source: [Wikipedia](http://en.wikipedia.org/wiki/Class)._

See also:

*   [object](http://stackoverflow.com/questions/tagged/object "show questions tagged 'object'")
*   [record](http://stackoverflow.com/questions/tagged/record "show questions tagged 'record'")
*   [struct](http://stackoverflow.com/questions/tagged/struct "show questions tagged 'struct'")
*   [instance](http://stackoverflow.com/questions/tagged/instance "show questions tagged 'instance'")