## About objective-c

This tag should be used only on questions that are about Objective-C features or depend on code in the language. The tags "cocoa" and "cocoa-touch" should be used to ask about Apple's frameworks or classes. Use the related tags [ios] and [osx] for issues specific to those platforms.

[Objective-C](http://en.wikipedia.org/wiki/Objective-C) is an object-oriented programming language combining features of [C](http://en.wikipedia.org/wiki/C) ([c](http://stackoverflow.com/questions/tagged/c "show questions tagged 'c'")) and [Smalltalk](http://en.wikipedia.org/wiki/Smalltalk) ([smalltalk](http://stackoverflow.com/questions/tagged/smalltalk "show questions tagged 'smalltalk'")). It is a strict superset of C (any valid C code is equally valid Objective-C code), and it inherits its object-oriented capabilities from Smalltalk. All procedural syntax is identical to that of C, and all object-oriented syntax is an implementation of Smalltalk messaging.

Objective-C was created primarily by [Brad Cox](http://en.wikipedia.org/wiki/Brad_Cox) and Tom Love in the early 1980s at their company [Stepstone](http://en.wikipedia.org/wiki/Stepstone). It is now primarily developed by [Apple, Inc](http://en.wikipedia.org/wiki/Apple_Inc.).

Objective-C is a general-purpose, high-level, object-oriented programming language that adds Smalltalk-style messaging to the C programming language. It is the main programming language used by Apple for [osx](http://stackoverflow.com/questions/tagged/osx "show questions tagged 'osx'") and [ios](http://stackoverflow.com/questions/tagged/ios "show questions tagged 'ios'") and their respective APIs, [cocoa](http://stackoverflow.com/questions/tagged/cocoa "show questions tagged 'cocoa'") and [cocoa-touch](http://stackoverflow.com/questions/tagged/cocoa-touch "show questions tagged 'cocoa-touch'").

Objective-C inherits the syntax, primitive types, and flow control statements of C and adds syntax for defining classes and methods. It also adds language-level support for object graph management and object literals while providing dynamic typing and binding, deferring many responsibilities until runtime.

# Hello world in Objective C

    #import <stdio.h>

    int main(void)
    {
        NSLog(@"Hello, world!\n");
        return 0;
    }

## Syntax

Objective-C is a thin layer on top of C, and moreover is a strict superset of C; it is possible to compile any C program with an Objective-C compiler, and to freely include C code within an Objective-C class. Objective-C derives its object syntax from Smalltalk. All of the syntax for non-object-oriented operations (including primitive variables, pre-processing, expressions, function declarations, and function calls) are identical to that of C, while the syntax for object-oriented features is an implementation of Smalltalk-style messaging.

## References

*   [Programming with Objective-C](https://developer.apple.com/library/ios/#documentation/Cocoa/Conceptual/ProgrammingWithObjectiveC/Introduction/Introduction.html#//apple_ref/doc/uid/TP40011210)
*   [Concepts in Objective-C Programming](https://developer.apple.com/library/ios/#documentation/General/Conceptual/CocoaEncyclopedia/Introduction/Introduction.html#//apple_ref/doc/uid/TP40010810)
*   [Cocoa Memory Management Programming Guide](http://developer.apple.com/mac/library/documentation/Cocoa/Conceptual/MemoryMgmt/Articles/mmRules.html), an essential read, especially the part about [Ownership Policy](https://developer.apple.com/library/mac/documentation/CoreFoundation/Conceptual/CFMemoryMgmt/Concepts/Ownership.html)
*   [Learn Objective-C](http://cocoadevcentral.com/d/learn_objectivec/) from Cocoa Dev Central, an introductory tutorial to the language
*   [Object-Oriented Programming with Objective-C](https://developer.apple.com/library/ios/#documentation/Cocoa/Conceptual/OOP_ObjC/Introduction/Introduction.html#//apple_ref/doc/uid/TP40005149)
*   WWDC 2012 videos on [Modern Objective-C](https://developer.apple.com/videos/wwdc/2012/?id=405) and [Migrating to Modern Objective-C](https://developer.apple.com/videos/wwdc/2012/?id=413)
*   [Advanced Memory Management Programming Guide](https://developer.apple.com/library/mac/#documentation/Cocoa/Conceptual/MemoryMgmt/Articles/MemoryMgmt.html)
*   [Learn Objective-C basics from CodeSchool](http://tryobjectivec.codeschool.com)
*   [Ry’s Objective-C Tutorial](http://rypress.com/tutorials/objective-c/index.html)
*   [Objective-C Guide For Developers](http://matteomanferdini.com/objective-c-guide-for-developers-part-1/)
*   [Objective-C Cheat Sheet and Quick Reference](http://www.raywenderlich.com/4872/objective-c-cheat-sheet-and-quick-reference)

### Stack Overflow questions with links to resources

*   [Cocoa and Objective-C resources?](http://stackoverflow.com/questions/7571/cocoa-and-objective-c-resources)

### Frequently posted questions in the Obj-C tag

*   [What's the difference between the atomic and nonatomic attributes?](http://stackoverflow.com/questions/588866/atomic-vs-nonatomic-properties)
*   [How does an underscore in front of a variable in a cocoa objective-c class work?](http://stackoverflow.com/q/822487)
*   [Getting date from [NSDate date] off by a few hours](http://stackoverflow.com/questions/8466744/get-wrong-nsdate/)
*   [Objective C Equivalent of PHP's "Variable Variables"](http://stackoverflow.com/questions/2283374/objective-c-equivalent-of-phps-variable-variables)
*   [NSMutableArray addObject not working](http://stackoverflow.com/questions/1827058/nsmutablearray-addobject-not-working)
*   [Objective C for Windows](http://stackoverflow.com/questions/56708/objective-c-for-windows)
*   [Objective C NSString* property retain count oddity](http://stackoverflow.com/questions/403112/objective-c-nsstring-property-retain-count-oddity)
*   [How to add percent sign to NSString](http://stackoverflow.com/questions/739682/how-to-add-percent-sign-to-nsstring)
*   [Passing Data between View Controllers](http://stackoverflow.com/questions/5210535/passing-data-between-view-controllers)

Code Language (used for [syntax highlighting](http://google-code-prettify.googlecode.com/svn/trunk/README.html)): lang-c

  lang-c