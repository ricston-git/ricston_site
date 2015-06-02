## About events

An event is a way for a class to provide notifications to listeners when a particular thing happens.

An event is a way for a class to provide notifications to clients of that class when some interesting thing happens to an object. The most familiar use for events is in graphical user interfaces; typically, the classes that represent controls in the interface have events that are notified when the user does something to the control (for example, click a button).

Events, however, need not be used only for graphical interfaces. Events provide a generally useful way for objects to signal state changes that may be useful to clients of that object. Events are an important building block for creating classes that can be reused in a large number of different programs.

Events are declared using delegates. A delegate object encapsulates a method so that it can be called anonymously. An event is a way for a class to allow clients to give it delegates to methods that should be called when the event occurs. When the event occurs, the delegate(s) given to it by its clients are invoked.

* * *

## References

*   [MSDN Events Tutorial (C#)](http://msdn.microsoft.com/en-us/library/aa645739%28v=vs.71%29.aspx)
*   [Event Wikipedia Article](http://en.wikipedia.org/wiki/Event_%28computing%29)
*   [Event-Handling in Java](http://docs.oracle.com/javase/tutorial/uiswing/events/index.html)