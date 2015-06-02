## About xslt

XSLT is a transformation language for XML designed to transform structured documents into other formats (such as XML, HTML, and plain text). Questions should use one of the xslt-1.0, xslt-2.0, or xslt-3.0 tags as appropriate.

# XSLT

Extensible Stylesheet Language Transformations (XSLT) is a programming language for transforming [XML](http://en.wikipedia.org/wiki/XML) documents into other XML documents, text documents, or [HTML](http://en.wikipedia.org/wiki/Html) documents. Other output formats are possible (e.g., [PDF](http://en.wikipedia.org/wiki/Portable_Document_Format) transformations using [XSL-FO](http://en.wikipedia.org/wiki/XSL_Formatting_Objects)).

The original document is not changed; rather, a new document is created based on the content of an existing one. Typically, input documents are XML files, but anything from which the processor can build an XQuery and XPath Data Model can be used, for example relational database tables, or geographical information systems.

A typical transformation is accomplished as follows:

1.  A stylesheet is created (typically a `.xsl` file).
2.  An XML data source is created (such as a `.xml` file).
3.  The XSLT processor is loaded with both the XSL and XML content.
4.  The XML document is parsed into an XPath Data Model ([XDM](http://www.w3.org/TR/xpath-datamodel)) tree (XDM is similar to [DOM](http://en.wikipedia.org/wiki/Document_Object_Model)).
5.  The XDM tree is traversed to produce a resulting document.

XSLT syntax is based on XML, which means that XSL documents also are well-formed XML documents. XSLT, with heavy emphasis on recursion, borrows principles from functional languages, including: declarative programming, pattern matching, and immutable variables.

As XSL is written in an XML format, its verbosity does not make it the first choice for general-purpose programming. When used correctly, XSL transformations produce elegant solutions to complex problems that are harder to solve in imperative languages.

## XSLT Processors and Libraries

Various XSL transformation processors and libraries include:

*   [SAXON](http://www.saxonica.com/)
*   [Xalan-Java](http://xml.apache.org/xalan-j/)
*   [MSXSL](http://msdn.microsoft.com/en-us/library/system.xml.xsl.aspx)
*   [EXSLT](http://www.exslt.org/)
*   [FXSL](http://fxsl.sourceforge.net/)
*   [XSLT Standard Library](http://xsltsl.sourceforge.net/)
*   [Kernow](http://kernowforsaxon.sourceforge.net/)
*   [xslt.js](http://johannburkard.de/software/xsltjs/)

## History

XSLT was proposed by the [W3C](http://www.w3.org/) and has three standards: [1.0](http://www.w3.org/TR/xslt), [2.0](http://www.w3.org/TR/xslt20/) and [3.0](http://www.w3.org/TR/xslt-30/) (This has been recently standardised).

## Question Tags

Questions should use one of the [xslt-1.0](http://stackoverflow.com/questions/tagged/xslt-1.0 "show questions tagged 'xslt-1.0'"), [xslt-2.0](http://stackoverflow.com/questions/tagged/xslt-2.0 "show questions tagged 'xslt-2.0'"), or [xslt-3.0](http://stackoverflow.com/questions/tagged/xslt-3.0 "show questions tagged 'xslt-3.0'") tags as appropriate to clarify what XSLT version the question requires or references.

## Resources

*   [XML Transformation resources on the W3C](http://www.w3.org/standards/xml/transformation)
*   [XSLT on Wikipedia](http://en.wikipedia.org/wiki/XSLT)
*   [XML on Wikipedia](http://en.wikipedia.org/wiki/XML)
*   [Free and reliable online IDE for XSLT 1.0, 2.0 and 3.0](http://xsltransform.net/)

## Online Training Courses

1.  "**[What's New in XSLT 3.0: Part 1](http://www.pluralsight.com/courses/xslt-3-0-whats-new-part1)**" -- A Pluralsight video-course (5.5h), by Dimitre Novatchev

2.  **[Foundations of XSLT 2 and XSLT 1](http://pluralsight.com/training/Courses/TableOfContents/xslt-foundations-part1)** A Pluralsight course by Dimitre Novatchev

3.  [**The Evolution of XPath: What’s New in XPath 3.0**](http://www.pluralsight.com/courses/xpath-3-0-whats-new) -- A Pluralsight video-course (4.5h)

Code Language (used for [syntax highlighting](http://google-code-prettify.googlecode.com/svn/trunk/README.html)): lang-xml

  lang-xml