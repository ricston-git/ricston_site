## About exception

An exception is a rarely occurring (exceptional!) condition that requires deviation from the program's normal flow. Normally, an exception should not result in total failure, but instead be attended by an exception handler. Exception handling is a built-in construct in many programming languages. Usually, exceptions are handled by unwinding the stack, thus rolling back to a defined state outside the exception's scope, and then invoking a handler routine.

## General

[Exception handling](http://en.wikipedia.org/wiki/Exception_handling) is a programming language construct or computer hardware mechanism designed to handle the occurrence of exceptions, special conditions that change the normal flow of program execution. When such conditions occur the programmer can decide to "throw" or "raise" an exception. The thrown exception will propagate up the stack until it's "caught" by an appropriate language construct, which usually contains code that deals with the situation. Unhandled exceptions usually lead to a "crash", i.e. abnormal termination.

Programming languages differ considerably in their support for exception handling (as distinct from error checking; which is normal program flow that codes for responses to contingencies such as unsuccessful termination of invoked operations). In some programming languages there are functions which cannot be safely called on invalid input data or functions which return values which cannot be distinguished from exceptions. For example, in [c](http://stackoverflow.com/questions/tagged/c "show questions tagged 'c'") the `atoi` (ASCII to integer conversion) function may return 0 (zero) for any input that cannot be parsed into a valid value. In such languages, the programmer must either perform error checking (possibly through some auxiliary global variable such as C's `errno`) or input validation (perhaps using regular expressions) or both.

## Exception safety

[Exception safety](http://en.wikipedia.org/wiki/Exception_safety) guarantees, as formalised by David Abrahams, offer a set of contract guidelines that an interface (or operation) offer w.r.t. the state of the program when (or if) an exception occurs.

1.  No-throw guarantee; the operation is guaranteed not to fail
2.  Strong exception safety; if the operation fails, the state will be as it was prior to the failure (rollback semantics)
3.  Basic exception safety; no leaks will occur, and data is left in a valid state (but possibly changed)
4.  No exception safety; no guarantees are made.

## Automated exception handling

Automated exception handling is a computing term referring to the computerized handling of errors. Runtime engines such as those for the Java language or Microsoft .NET lend themselves to an automated mode of exception or error handling. In these environments software errors do not "crash" the operating system or the runtime engine but rather generate exceptions. Recent advances in these runtime engines enables specialized runtime-engine add-on products to provide automated exception handling that is independent of the source code and provides root-cause information for every exception of interest.

* * *

## References

*   [Exception handling syntax](http://en.wikipedia.org/wiki/Exception_handling_syntax)