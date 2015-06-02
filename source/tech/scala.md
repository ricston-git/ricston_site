Back [Home](\wiki)

## About Scala

Scala is a general purpose programming language principally targeting the Java Virtual Machine. Designed to express common programming patterns in a concise, elegant, and type-safe way, it fuses both imperative and functional programming styles. Its key features are: advanced static type system with type inference; function types; pattern-matching; implicit parameters and conversions; operator overloading; full interoperability with Java; concurrency

[Scala](http://en.wikipedia.org/wiki/Scala_%28programming_language%29) is a general purpose programming language principally targeting the Java Virtual Machine. Designed to express common programming patterns in a concise, elegant, and type-safe way, it fuses both imperative and functional programming styles. Its key features are:

*   Static typing
*   Advanced type system with type inference and declaration-site variance
*   Function types (including anonymous) which support _lexical closures_
*   Pattern-matching
*   Implicit parameters and conversions which support the _typeclass_ and _enrich-my-library_ patterns
*   Mixin composition
*   Full interoperability with Java
*   Powerful concurrency constructs
*   Advanced language constructs such as delimited continuations and an experimental macro system

For more information, see the official [Scala Introduction](http://www.scala-lang.org/node/25) and [Scala Documentation](http://docs.scala-lang.org).

To search for Scala symbols such as "=>" in Stack Overflow, you can use [symbolhound search](http://symbolhound.com/).

To search Scala documentation, you can use [scalex](http://scalex.org/).

### Free Scala programming books and guides

*   [Programming in Scala, First Edition](http://www.artima.com/pins1ed/)
*   [Scala By Example](http://www.scala-lang.org/docu/files/ScalaByExample.pdf) (PDF)
*   [A Scala Tutorial for Java programmers](http://docs.scala-lang.org/tutorials/scala-for-java-programmers.html)
*   [Scala for Java refugees](http://www.codecommit.com/blog/scala/roundup-scala-for-java-refugees)
*   [Scala School](http://twitter.github.com/scala_school/)
*   [Scala Tutorials](http://scalatutorials.com/tour)
*   [Scala Tour](http://www.scala-tour.com)
*   [Scala for the Impatient](http://horstmann.com/scala/) (first part available for free at [http://typesafe.com/resources/free-books](http://typesafe.com/resources/free-books))

# Stack Overflow Scala Tutorial

1.  Introduction to Scala
    *   [What's so great about Scala?](http://stackoverflow.com/questions/727078/whats-so-great-about-scala)
2.  Variables/values
    *   [Difference between `val` and `var`](http://stackoverflow.com/questions/1791408/what-is-the-difference-between-a-var-and-val-definition-in-scala)
    *   [val-mutable versus var-immutable](http://stackoverflow.com/questions/11386559/val-mutable-versus-var-immutable-in-scala)
    *   [How to assign vals correctly?](http://stackoverflow.com/questions/4026564/scala-assigning-vals/4031369#4031369)
    *   [Multiple variable declarations](http://stackoverflow.com/questions/1981748/declaring-multiple-variables-in-scala)
    *   Lazy vals
        *   [What do they do?](http://stackoverflow.com/questions/7484928/what-does-a-lazy-val-do)
        *   [How are they implemented?](http://stackoverflow.com/questions/3041253/whats-the-hidden-cost-of-lazy-val-scala)
    *   [Identifier rules](http://stackoverflow.com/questions/7656937/valid-identifier-characters-in-scala)
3.  Methods
    *   [Equal sign in methods](http://stackoverflow.com/questions/944111/when-to-use-the-equals-sign-in-a-scala-method-declaration)
    *   [Operator notation](http://stackoverflow.com/questions/1006967/scala-which-characters-can-i-omit/1014972#1014972) and [the rules](http://stackoverflow.com/questions/1181533/what-are-the-precise-rules-for-when-you-can-omit-parenthesis-dots-braces-fu)
    *   [Multiple ways to define a method/function](http://stackoverflow.com/questions/8303817/scala-9-ways-to-define-a-method) ([leave parentheses in method calls](http://stackoverflow.com/questions/6643030/what-is-the-rule-for-parenthesis-in-scala-method-invocation))
    *   [Unary operators](http://stackoverflow.com/questions/1991240/scala-method-operator-overloading)
    *   [Multiple parameter lists](http://stackoverflow.com/questions/4915027/two-ways-of-currying-in-scala-whats-the-use-case-for-each/4916606#4916606)
    *   [Right-associative method names](http://stackoverflow.com/questions/2827293/scala-operator-how-it-works)
    *   Side effect free methods
        *   Missing parentheses at methods
        *   [Why no i++ in Scala?](http://stackoverflow.com/questions/4520463/why-no-i-in-scala)
    *   [How to mix punctuation with alphanumeric characters in method names?](http://stackoverflow.com/questions/3096517/do-methods-ending-with-have-a-special-meaning-in-scala)
    *   [Shortcut methods (`+=`, `-=`, `*=`, ...)](http://stackoverflow.com/questions/5074179/val-or-var-mutable-or-immutable)
    *   [List of "magic method" names](http://stackoverflow.com/questions/1483212/list-of-scalas-magic-functions) ([apply](http://stackoverflow.com/questions/1223834/how-does-scalas-apply-method-magic-work), unapply/unapplySeq, update)
    *   Named arguments / optional parameters
    *   [Type inference in return type](http://stackoverflow.com/questions/2209179/type-inference-on-method-return-type)
    *   [Difference between `##` and `hashCode`](http://stackoverflow.com/questions/9068154/what-is-the-difference-between-and-hashcode)
4.  Literals, statements and blocks
    *   Difference between block and statement
    *   [Weak conformance](http://stackoverflow.com/questions/3094380/what-is-the-concept-of-weak-conformance-in-scala)
    *   [Symbols](http://stackoverflow.com/questions/1324466/practical-examples-of-using-symbols-in-scala)
    *   [Difference between braces and parentheses](http://stackoverflow.com/questions/4386127/what-is-the-formal-difference-in-scala-between-braces-and-parentheses-and-when-s)
    *   [Dereference keyword (backtick usage)](http://stackoverflow.com/questions/1793984/using-java-lib-with-scala-reserved-words)
    *   [Local definitions](http://stackoverflow.com/questions/1284325/scala-equivalent-to-haskells-where-clauses/1284361#1284361)
    *   [Uses of an underscore](http://stackoverflow.com/questions/8000903/what-are-all-the-uses-of-an-underscore-in-scala)
    *   [Identifier rules](http://stackoverflow.com/questions/7656937/valid-identifier-characters-in-scala)
    *   [Punctuation (operator) overview](http://stackoverflow.com/questions/7888944/scala-punctuation-aka-symbols-operators)
5.  Loops/recursion
    *   Loop
        *   [Simple loop](http://stackoverflow.com/questions/6741787/how-would-i-translate-the-following-java-backward-counting-loop-into-scala)
        *   [Break out of a loop](http://stackoverflow.com/questions/2742719/how-do-i-break-out-of-a-loop-in-scala)
        *   [How to call a function x times](http://stackoverflow.com/questions/7530194/how-to-call-a-function-x-times-in-scala)
    *   Tail recursion
        *   [What is tail recursion?](http://stackoverflow.com/questions/1677419/does-scala-support-tail-recursion-optimization)
        *   [How to write tail recursive code?](http://stackoverflow.com/questions/3678569/how-to-recognize-what-is-and-what-is-not-tail-recursion)
        *   [Performance](http://stackoverflow.com/questions/1373144/scala-list-recursion-performance)
        *   [Optimization rules](http://stackoverflow.com/questions/4785502/why-wont-the-scala-compiler-apply-tail-call-optimization-unless-a-method-is-fina)
    *   [Trampolining](http://stackoverflow.com/questions/1025181/hidden-features-of-scala/2853836#2853836)
6.  Data structures / Collections
    *   [Collections design tutorial](http://stackoverflow.com/questions/1722137/scala-2-8-collections-design-tutorial)
    *   [Collection standard practice](http://stackoverflow.com/questions/675381/scala-collection-standard-practice)
    *   Immutable Collections
        *   [List](http://stackoverflow.com/questions/1241166/preferred-way-to-create-a-scala-list)
        *   [Vector](http://stackoverflow.com/questions/6928327/when-should-i-choose-vector-in-scala)
        *   [Range](http://stackoverflow.com/questions/2617513/scala-downwards-or-decreasing-for-loop)
        *   [Tuple](http://stackoverflow.com/questions/6884298/why-is-scalas-syntax-for-tuples-so-unusual)
        *   Map
        *   Set
    *   Mutable Collections
        *   [Array](http://stackoverflow.com/questions/2481149/why-does-array0-1-2-array0-1-2-not-return-the-expected-result) and [multi-dimensional Arrays](http://stackoverflow.com/questions/2381908/how-to-create-and-use-a-multi-dimensional-array-in-scala-2-8)
        *   [Buffer](http://stackoverflow.com/questions/3368888/whats-the-best-way-to-create-a-dynamically-growing-a-array-in-scala)
        *   [How to use mutable Collections?](http://stackoverflow.com/questions/6909783/how-to-use-mutable-collections-in-scala)
        *   [Mutating a mutable collection using map?](http://stackoverflow.com/questions/7184940/mutating-a-mutable-collection-using-map)
    *   Lazy Collections
        *   [Why are they needed?](http://stackoverflow.com/questions/4795724/why-is-filter-in-front-of-foldleft-slow-scala)
        *   [View](http://stackoverflow.com/questions/3361478/scala-what-are-views-for-collections-and-when-would-you-want-to-use-them)
        *   [Iterator](http://stackoverflow.com/questions/1527962/difference-between-iterator-and-stream-in-scala)
        *   [Stream](http://stackoverflow.com/questions/2096876/use-cases-for-streams-in-scala)
        *   [Streams vs Views vs Iterators](http://stackoverflow.com/questions/5159000/stream-vs-views-vs-iterators)
        *   [Return a lazy collection](http://stackoverflow.com/questions/4525435/is-it-posible-in-scala-to-use-yield-to-generate-iterator-instead-of-list)
    *   Parallel Collections
        *   [How do they work?](http://stackoverflow.com/questions/6329337/how-are-scala-2-9-parallel-collections-working-behind-the-scenes)
        *   [Is is possible to change their behavior?](http://stackoverflow.com/questions/6039380/how-do-i-replace-the-fork-join-pool-for-a-scala-2-9-parallel-collection)
    *   Conversions
        *   [Casting](http://stackoverflow.com/questions/931463/scala-how-do-i-cast-a-variable) and [ascription](http://stackoverflow.com/questions/3412068/what-are-the-differences-between-asinstanceoft-and-o-t-in-scala)
        *   [Java Collection to Scala Collection and vice versa](http://stackoverflow.com/questions/674713/converting-java-collection-into-scala-collection)
        *   [Convert to another Collections](http://stackoverflow.com/questions/3074118/scala-how-do-i-convert-a-mapint-any-to-a-sortedmap-or-a-treemap)
        *   [breakout](http://stackoverflow.com/questions/1715681/scala-2-8-breakout)
    *   [Memory footprint](http://stackoverflow.com/questions/6243232/scala-collection-memory-footprint-characteristics)
    *   [How are Scala collections able to return the correct collection type from an operation?](http://stackoverflow.com/questions/5200505/how-are-scala-collections-able-to-return-the-correct-collection-type-from-a-map-o)
7.  For-comprehension
    *   [Explanation](http://stackoverflow.com/questions/1052476/can-someone-explain-scalas-yield)
    *   [nested for-expressions](http://stackoverflow.com/questions/2303826/how-can-i-iterate-a-list-of-lists-in-scala)
    *   [Use `for` inside expressions](http://stackoverflow.com/questions/2955370/why-cant-i-call-methods-on-a-for-yield-expression)
8.  Enumeration
    *   [Explanation](http://stackoverflow.com/questions/1321745/scala-doesnt-have-enums-what-to-use-instead-of-an-enum)
9.  Pattern matching
    *   Explanation
    *   [Value binding (`x @ X`)](http://stackoverflow.com/questions/2359014/scala-operator/2359365#2359365) / type binding (`x: X`)
    *   [How to do a multi-match](http://stackoverflow.com/questions/3222691/matching-and-binding-two-exception-classes-in-one-case-statement-in-scala-2-7)
    *   [Guards](http://stackoverflow.com/questions/2266915/does-scala-have-guards)
    *   [How to match variables or values?](http://stackoverflow.com/questions/7078022/why-does-pattern-matching-in-scala-not-work-with-variables)
    *   [How is pattern match implemented under the hood?](http://stackoverflow.com/questions/754166/how-is-pattern-matching-in-scala-implemented-at-bytecode-level)
    *   [Exhaustive pattern](http://stackoverflow.com/questions/4015144/scala-pattern-matching-keep-saying-match-is-not-exhaustive)
    *   [Pattern match in for-expressions](http://stackoverflow.com/questions/4546786/how-to-simplify-this-for-code)
    *   [Ignore cases / no default value](http://stackoverflow.com/questions/5445163/is-there-a-way-to-ignore-a-non-matching-case)
    *   [Conjunction](http://stackoverflow.com/questions/2261358/pattern-matching-with-conjunctions-patterna-and-patternb)
    *   [Pattern match PartialFunctions](http://stackoverflow.com/questions/7168026/how-is-match-word-omitted-in-scala)
    *   [Match Regex](http://stackoverflow.com/questions/4636610/regex-and-pattern-matching-in-scala)
    *   [Pattern matching with more than one match](http://stackoverflow.com/questions/7565599/pattern-matching-with-more-than-one-match)
10.  Classes, objects and types
    *   [Difference between `class` and `object`](http://stackoverflow.com/questions/1755345/scala-difference-between-object-and-class)
    *   [Why is `object` a Singleton?](http://stackoverflow.com/questions/6541393/explanation-of-singleton-objects-in-scala-please)
    *   [Why are singleton objects more object-oriented?](http://stackoverflow.com/questions/4112088/why-are-singleton-objects-more-object-orientated)
    *   [Companion objects](http://stackoverflow.com/questions/609744/what-is-the-rationale-behind-having-companion-objects-in-scala)
    *   [Difference between `class` and `type`](http://stackoverflow.com/questions/5031640/what-is-the-difference-between-a-class-and-a-type-in-scala-and-java)
    *   [What's the difference between a class with a companion object and a class and object with the same name?](http://stackoverflow.com/questions/11604320/whats-the-difference-between-a-class-with-a-companion-object-and-a-class-and-ob)
    *   [Static initializer](http://stackoverflow.com/questions/6265864/why-does-a-small-change-to-this-scala-code-make-such-a-huge-difference-to-perform)
    *   [Constructor overloading](http://stackoverflow.com/questions/1095329/scala-constructor-overload)
    *   [Static data in non-objects](http://stackoverflow.com/questions/1516087/in-scala-how-would-you-declare-static-data-inside-a-function)
    *   [How to get the static/runtime type of a class](http://stackoverflow.com/questions/1135248/scala-equivalent-of-java-java-lang-classt-object)
    *   [Type projection (`A#B`)](http://stackoverflow.com/questions/6676048/why-does-one-select-scala-type-members-with-a-hash-instead-of-a-dot)
11.  Packages, imports and visibility identifiers
    *   Imports
        *   [Multiple imports / import renames / hide imports](http://stackoverflow.com/questions/2871822/how-do-i-exclude-rename-some-classes-from-import-in-scala)
        *   [Shorthand imports](http://stackoverflow.com/questions/11621083/scala-shorthand-to-import-object-foo-and-trait-bar)
        *   Local imports
    *   Packages
        *   [Nested packages](http://stackoverflow.com/questions/2830248/what-are-nested-unnested-packages-in-scala-2-8) / [multiple package definitions](http://stackoverflow.com/questions/3541053/multiple-packages-definition)
        *   [Package objects](http://stackoverflow.com/questions/3400734/package-objects)
    *   Visibility
        *   Explanation
        *   [Private constructors](http://stackoverflow.com/questions/1730536/private-and-protected-constructor-in-scala)
        *   [Private variables](http://stackoverflow.com/questions/6190617/how-can-i-create-a-read-only-class-member-in-scala)
12.  Inheritance
    *   Explanation
    *   [Early initializer](http://stackoverflow.com/questions/4712468/in-scala-what-is-an-early-initializer)
13.  Extractors
    *   [Explanation](http://stackoverflow.com/questions/2662984/what-are-all-the-instances-of-syntactic-sugar-in-scala/2670837#2670837) (Example: [conjunctions](http://stackoverflow.com/questions/4008271/explain-this-pattern-matching-code))
    *   [Infix notation for type parameters](http://stackoverflow.com/questions/1025181/hidden-features-of-scala/4318422#4318422) (`X[A, B]` => `A X B`)
14.  Case classes
    *   [Explanation](http://stackoverflow.com/questions/2312881/what-is-the-difference-between-scalas-case-class-and-class)
    *   [case classes vs. enums](http://stackoverflow.com/questions/1898932/case-classes-vs-enumerations-in-scala)
    *   [What are the disadvantages to declaring Scala case classes](http://stackoverflow.com/questions/4653424/what-are-the-disadvantages-to-declaring-scala-case-classes)
    *   [Compiler generated code for case classes](http://stackoverflow.com/questions/4526706/what-code-is-generated-for-an-equals-hashcode-method-of-a-case-class)
15.  Parameterized types
    *   How to declare them?
    *   [Upper / lower bounds](http://stackoverflow.com/questions/7759361/what-does-b-a-do-in-scala)
    *   [Unify numerics](http://stackoverflow.com/questions/4709571/scala-parameterized-methods-and-arithmetic-operations)
    *   [How to get around type erasure?](http://stackoverflow.com/questions/1094173/how-do-i-get-around-type-erasure-on-scala-or-why-cant-i-get-the-type-parameter)
    *   [Abstract Types vs Generics](http://stackoverflow.com/questions/1154571/scala-abstract-types-vs-generics)
    *   [Variances](http://stackoverflow.com/questions/663254/scala-covariance-contravariance-question)
16.  Traits
    *   [Usage](http://stackoverflow.com/questions/1229743/scala-traits-usage)
    *   [Mixin multiple traits](http://stackoverflow.com/questions/1084572/mixing-multiple-traits-in-scala/1084716#1084716)
    *   [Traits vs abstract classes](http://stackoverflow.com/questions/1991042/scala-traits-vs-abstract-classes)
    *   [What does `trait A <: B` mean?](http://stackoverflow.com/questions/2123663/what-does-trait-a-b-mean)
    *   [Linearization](http://stackoverflow.com/questions/7230808/inheriting-a-trait-twice)
    *   [Mixin a trait with overridden behavior](http://stackoverflow.com/questions/1025181/hidden-features-of-scala/7105405#7105405)
    *   [Dynamic mixins](http://stackoverflow.com/questions/3254232/dynamic-mixin-in-scala-is-it-possible)
    *   [How are they implemented under the hood?](http://stackoverflow.com/questions/2557303/how-are-scala-traits-compiled-into-java-bytecode)
    *   [How to access one of multiple traits of superclass?](http://stackoverflow.com/questions/7526653/how-to-access-one-of-multiple-traits-of-superclass)
17.  Self references
    *   [Unify types](http://stackoverflow.com/questions/932701/scala-two-methods-different-parameter-types-but-same-code-how-to-unify)
    *   [Self reference naming](http://stackoverflow.com/questions/4017357/difference-between-this-and-self-in-self-type-annotations)
    *   [Multiple self references](http://stackoverflow.com/questions/4355060/are-multiple-self-types-possible)
    *   [Difference between self references and subtyping](http://stackoverflow.com/questions/1990948/what-is-the-difference-between-scala-self-types-and-trait-subclasses)
18.  Error handling
    *   Exceptions
        *   Explanation
        *   [Stand-alone try block](http://stackoverflow.com/questions/1547465/what-does-scalas-try-mean-without-either-a-catch-or-finally-block)
        *   [Ignore an exception](http://stackoverflow.com/questions/3960327/how-to-ignore-exception)
        *   [Try-catch-generalization](http://stackoverflow.com/questions/7788803/what-are-the-use-cases-for-scala-2-9s-try-catch-generalization)
    *   Option
        *   [Explanation](http://stackoverflow.com/questions/2079170/why-optiont)
    *   Either
        *   [Explanation](http://stackoverflow.com/questions/1585395/using-comparison-operators-in-scalas-pattern-matching-system)
        *   [How to use them?](http://stackoverflow.com/questions/7131076/whats-the-deal-with-all-the-either-cruft)
    *   [What to use?](http://stackoverflow.com/questions/6891018/better-to-return-none-or-throw-an-exception-when-fetching-url)
19.  Type handling
    *   [Context (`[A : B]`) and view bounds (`[A <% B]`)](http://stackoverflow.com/questions/4465948/what-are-scala-context-and-view-bounds)
    *   Types
        *   [Non-Nullable type](http://stackoverflow.com/questions/1522367/library-support-for-scalas-notnull-trait)
        *   [Existential type](http://stackoverflow.com/questions/1031042/scalas-existential-types)
        *   Structural type ("duck typing")
        *   [Path-dependent type](http://stackoverflow.com/questions/2693067/what-is-meant-by-scalas-path-dependent-types/2694607#2694607)
        *   [Union types (type disjunction)](http://stackoverflow.com/questions/3508077/does-scala-have-type-disjunction-union-types)
        *   [Monad type](http://stackoverflow.com/questions/2322783/how-to-add-tracing-within-a-for-comprehension/4871353#4871353)
        *   [Compound type in structural type](http://stackoverflow.com/questions/1025181/hidden-features-of-scala/4311831#4311831)
        *   [Compound type in self references](http://stackoverflow.com/questions/4355060/are-multiple-self-types-possible)
        *   [Compound type in parameterized type](http://stackoverflow.com/questions/1491283/how-do-i-setup-multiple-type-bounds-in-scala)
    *   [Advantages of Scala's type system](http://stackoverflow.com/questions/3112725/advantages-of-scalas-type-system)
20.  Annotations
    *   [What are they?](http://stackoverflow.com/questions/3079603/scala-annotations-what-actually-is-that)
    *   [How to use them?](http://stackoverflow.com/questions/2265773/how-do-you-define-an-interface-in-scala)
21.  Functions/Function literals
    *   [Explanation](http://stackoverflow.com/questions/2293592/functional-programming-scala-map-and-fold-left/2303291#2303291)
    *   [Functions vs methods](http://stackoverflow.com/questions/2529184/difference-between-method-and-function-in-scala/2530007#2530007)
    *   [Pass functions](http://stackoverflow.com/questions/2934568/why-does-scala-apply-thunks-automatically-sometimes)
    *   [Currying](http://stackoverflow.com/questions/1550821/scala-anonymous-function-syntax)
    *   [PartialFunction](http://stackoverflow.com/questions/930698/why-is-partialfunction-function-in-scala)
    *   [Placeholder syntax](http://stackoverflow.com/questions/1025181/hidden-features-of-scala/1083523#1083523) and [their replacement rules](http://stackoverflow.com/questions/2173373/scala-foreach-strange-behaviour)
    *   [Placeholder syntax with right-associative methods](http://stackoverflow.com/questions/9436119/scala-inverse-result-while-escaping-underscore-with)
    *   [Difference between `=> Type`, `() => Type` and `Unit => Type`](http://stackoverflow.com/questions/4543228/whats-the-difference-between-and-unit)
    *   [Functional Quicksort](http://stackoverflow.com/questions/2341890/step-by-step-explanation-of-scala-syntax-used-in-wikipedia-quick-sort-example)
    *   [Keyword `return` in higher order functions](http://stackoverflow.com/questions/6915701/is-non-local-return-in-scala-new) and [performance problem with that](http://stackoverflow.com/questions/6146182/how-to-optimize-for-comprehensions-and-loops-in-scala)
    *   [Function composition](http://stackoverflow.com/questions/7683362/function-composition-of-methods-functions-and-partially-applied-functions-in-s)
    *   [Closures in Scala](http://stackoverflow.com/questions/9842476/closing-over-the-loop-variable-in-scala)
22.  Type safety
    *   Manifest
        *   [Explanation](http://stackoverflow.com/questions/3213510/what-is-a-manifest-in-scala-and-when-do-you-need-it)
        *   [How do they work?](http://stackoverflow.com/questions/3587286/how-does-scalas-2-8-manifest-work)
        *   [Are Manifests possible in constructors?](http://stackoverflow.com/questions/7294761/why-is-the-manifest-not-available-in-the-constructor)
    *   [Generalized Type Constraints (`<:<`, `<%<`, `=:=`)](http://stackoverflow.com/questions/3427345/what-do-and-mean-in-scala-2-8-and-where-are-they-documented)
    *   [Path-Dependent Types](http://stackoverflow.com/questions/2693067/what-is-meant-by-scalas-path-dependent-types)
    *   [Enforce type difference](http://stackoverflow.com/questions/6909053/enforce-type-difference)
    *   [Enforce no type bounds](http://stackoverflow.com/questions/7781782/type-parameter-does-not-extend-given-type)
23.  Implicits
    *   [Implicit definitions / parameters](http://stackoverflow.com/questions/1025181/hidden-features-of-scala/1093967#1093967)
    *   [Implicit conversions / Monkey patching](http://stackoverflow.com/questions/3119580/scala-equivalent-of-csharps-extension-methods/3119671#3119671)
    *   [Identifier `implicitly`](http://stackoverflow.com/questions/3855595/scala-function-implicitly)
    *   [Where does Scala look for implicits?](http://stackoverflow.com/questions/5598085/where-does-scala-look-for-implicits)
    *   [Should implicits used?](http://stackoverflow.com/questions/1404889/scala-implicit-usage-choices)
    *   [Style of implicits](http://stackoverflow.com/questions/5984720/coding-with-scala-implicits-in-style)
    *   [Convert multiple values with one implicit conversion](http://stackoverflow.com/questions/7235328/is-there-any-usage-of-implicit-function-with-several-parameters-in-scala)
    *   [Chaining implicits](http://stackoverflow.com/questions/5332801/how-can-i-chain-implicits-in-scala)
24.  Reflection
    *   [What is a TypeTag and how do I use it?](http://stackoverflow.com/questions/12218641/scala-2-10-what-is-a-typetag-and-how-do-i-use-it)
    *   How to work with Reflection?
25.  Enrich-my-library pattern (formerly known as pimp-my-library)
    *   [Explanation](http://stackoverflow.com/questions/5410846/how-do-i-apply-the-pimp-my-library-pattern-to-scala-collections/5411133#5411133)
    *   [CanBuildFrom](http://stackoverflow.com/questions/1721356/scala-2-8-canbuildfrom)
    *   [Returning original types while extending the Collection API](http://stackoverflow.com/questions/10019529/function-which-generically-takes-a-type-and-returns-the-same-type)
26.  [Concurrency overview](http://stackoverflow.com/questions/7969557/how-are-message-passing-concurrent-languages-better-than-shared-memory-concurren)
27.  Actors
    *   [Differences between Actor implementations](http://stackoverflow.com/questions/5997018/whats-the-difference-between-the-different-actors-implementation-in-scala)
    *   [Design Patterns](http://stackoverflow.com/questions/3931994/design-patterns-best-practice-for-building-actor-based-system)
    *   [Worst practices](http://stackoverflow.com/questions/1549251/scala-actors-worst-practices)
28.  Use Java from Scala and vice versa
    *   [Iterate over Java collection](http://stackoverflow.com/questions/2708990/whats-the-new-way-to-iterate-over-a-java-map-in-scala-2-8-0)
    *   [Migrate Java to Scala](http://stackoverflow.com/questions/3967683/migrating-java-to-scala)
    *   [Transparent conversions useful?](http://stackoverflow.com/questions/1519838/java-scala-interop-transparent-list-and-map-conversion)
    *   [Using Scala traits with implemented methods in Java](http://stackoverflow.com/questions/7637752/using-scala-traits-with-implemented-methods-in-java)
    *   [How to work with javap for Scala/Java interop?](http://stackoverflow.com/questions/9350528/how-to-work-with-javap-for-scala-java-interop)
    *   [Scala signatures](http://stackoverflow.com/questions/5587460/why-does-running-javap-on-a-compiled-scala-class-show-weird-entries-in-the-const)
    *   [How does `abstract override` work internally?](http://stackoverflow.com/questions/9476126/can-somebody-explain-how-abstract-override-works-in-terms-of-java-code)
29.  XML literals
    *   Explanation
30.  Scala Swing
    *   Explanation
    *   [Examples](http://stackoverflow.com/questions/4515008/are-there-a-good-examples-of-using-scala-swing)
31.  Type Programming
    *   [Overview](http://stackoverflow.com/questions/4415511/scala-type-programming-resources)
32.  Functional Scala
    *   [Is immutability expensive?](http://stackoverflow.com/questions/4101924/functional-programming-is-immutability-expensive)
    *   [Is Scala functional programming slower than traditional coding?](http://stackoverflow.com/questions/2794823/is-scala-functional-programming-slower-than-traditional-coding)
    *   [OOP in a purely FP context?](http://stackoverflow.com/questions/4113138/oop-in-a-purely-fp-context)
    *   Continuations
        *   [Explanation](http://stackoverflow.com/questions/1512930/what-are-scala-continuations-and-why-use-them)
        *   [How to activate them?](http://stackoverflow.com/questions/2683195/how-do-i-enable-continuations-on-scala-2-8-and-beyond)
    *   [Design patterns for functional-oo hybrid languages?](http://stackoverflow.com/questions/3084546/design-patterns-for-functional-oo-hybrid-languages)
    *   [Type programming](http://stackoverflow.com/questions/4415511/scala-type-programming-resources)
    *   [Higher kinded types](http://stackoverflow.com/questions/6246719/what-is-a-higher-kinded-type-in-scala)
    *   [Type lambdas (`SomeType[({type λ[α] = Either[A, α]})#λ]`)](http://stackoverflow.com/questions/6246719/what-is-a-higher-kinded-type-in-scala)
    *   [Virtual Classes](http://stackoverflow.com/questions/3035807/what-can-i-do-with-virtual-classes)
    *   [`forall` in Scala](http://stackoverflow.com/questions/7213676/forall-in-scala)

## Further learning

1.  Learning Resources
    *   [How can I learn more about Scala's type relationships?](http://stackoverflow.com/questions/7782286/how-can-i-learn-more-about-scalas-type-relationships)
    *   [Scala Cheat Sheet](http://docs.scala-lang.org/cheatsheets/)
    *   [Good examples of idiomatic scala code?](http://stackoverflow.com/questions/11359784/good-examples-of-idiomatic-scala-code)
    *   [Solidifying Scala knowledge](http://stackoverflow.com/questions/6525547/scala-example-to-help-solidify-book-knowledge)
2.  REPL
    *   [How does it work behind the scenes?](http://stackoverflow.com/questions/7655165/what-really-happens-behind-the-scala-runtime-repl-when-running-a-scala-program)
3.  Working with `scalac` and `scala`
    *   [Show syntax trees](http://stackoverflow.com/questions/9999664/how-to-examine-implicit-rich-conversions-and-implemented-traits-in-the-repl)
    *   [Meaning of `!#` (bang-pound) in a shell script?](http://stackoverflow.com/questions/10060419/what-is-the-meaning-of-bang-pound-in-a-sh-bash-shell-script)
4.  Operator precedence
    *   [Specification rules](http://stackoverflow.com/questions/2922347/operator-precedence-in-scala)
    *   [Actual scalac precedence implementation](http://stackoverflow.com/questions/7618923/actual-precedence-for-infix-operators-in-scala)
    *   [Understanding precedence rules in practice](http://stackoverflow.com/questions/8266401/the-method-execution-puzzle-in-scala)
5.  [Scala blogs to follow](http://stackoverflow.com/questions/1445003/what-scala-blogs-do-you-regularly-follow)
6.  Scala style
    *   [Scala Style Guide](http://stackoverflow.com/questions/3718674/scala-coding-styles-and-conventions)
    *   [Elements of Scala Style](http://stackoverflow.com/questions/1281977/elements-of-scala-style)
    *   [Effective Scala](http://twitter.github.com/effectivescala/)
7.  [Functional Programming Principles in Scala](https://www.coursera.org/course/progfun), a free functional programming course on Coursera taught by Martin Odersky, the creator of Scala
8.  [Principles of Reactive Programming](https://www.coursera.org/course/reactive), a free reactive functional programming course on Coursera taught by Martin Odersky, Erik Meijer, Roland Kuhn.

  lang-scala