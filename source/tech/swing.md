## About swing

Swing is the primary user-interface toolkit in Java and is shipped with the standard Java SDK. It is contained within the package javax.swing.

Swing is the GUI toolkit packaged with the standard Java SDK (since 1.2).

**General information**

*   [Swing Architecture Overview](http://www.oracle.com/technetwork/java/architecture-142923.html)
*   [Javadoc](http://docs.oracle.com/javase/8/docs/api/javax/swing/package-summary.html) (JDK8)
*   [Wikipedia on Swing](http://en.wikipedia.org/wiki/Swing_%28Java%29)
*   [The Swing tutorial](http://docs.oracle.com/javase/tutorial/uiswing/)

**Specialized articles**

*   [Painting in AWT and Swing: The Paint Methods](http://www.oracle.com/technetwork/java/painting-140037.html)
*   [Troubleshooting Swing](http://www.oracle.com/technetwork/java/javase/swing-135905.html)

**Essential topics in Swing programming**

_Layout managers_: [Layout managers](http://docs.oracle.com/javase/7/docs/api/java/awt/LayoutManager.html) are responsible for determining the size and position of components in a `Container`.

*   [Layout manager tutorial](http://docs.oracle.com/javase/tutorial/uiswing/layout/): complete tutorial on how to use layout managers
*   [Visual guide to layout managers](http://docs.oracle.com/javase/tutorial/uiswing/layout/visual.html): overview of the different layout managers and their main features
*   [Nesting layouts](http://stackoverflow.com/questions/5621338/about-swing-and-jtable/5630271#5630271): allows to design almost any UI

_Swing threading rules_: Swing is single threaded and any access to Swing components should happen on the Swing thread (the Event Dispatch Thread or EDT).

*   Start with the [Concurrency in Swing](http://docs.oracle.com/javase/tutorial/uiswing/concurrency/) tutorial
*   Detect EDT violations using one of the approaches cited [here](http://stackoverflow.com/q/7787998/230513)
*   Use [`SwingWorker`](http://stackoverflow.com/questions/8916721/java-swing-update-label/8917565#8917565) to perform lengthy operations in the background and update the UI on the `EDT`
*   Use a [Swing `Timer`](http://stackoverflow.com/questions/9849950) for animation

Code Language (used for [syntax highlighting](http://google-code-prettify.googlecode.com/svn/trunk/README.html)): default

  default