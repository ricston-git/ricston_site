## About xml

Extensible Markup Language (XML) is a flexible, structured document format that defines human- and machine-readable encoding rules.

# Extensible Markup Language

[Wikipedia](http://en.wikipedia.org/wiki/XML) defines XML as follows:

> **XML** (Extensible Markup Language) is a set of rules for encoding documents in both human-readable and machine-readable form. It is defined in the XML 1.0 Specification produced by the [W3C](http://www.w3.org/), and several other related specifications, all gratis open standards.
> 
> **Extensible** - XML is extensible. It lets you define your own tags.
> 
> **Markup** - The most attractive feature of XML has to be its ability to allow its user to create their own tags. The tags that can be created will be similar to tags in HTML. But with XML you are afforded the opportunity to define your own tags.
> 
> **Language** - XML is a language that is very similar to HTML. But it’s much more flexible because it allows to create custom tags. In this way XML acts like a meta-language: a language that allows us to create or define other languages. For example, with XML we can create other languages, such as RSS.

In short, XML is:

*   designed to transport and store data; and
*   a flexible text format derived from SGML (ISO 8879).
*   a markup language much like HTML
*   designed to be self-descriptive

The design goals of XML emphasize simplicity, generality, and usability over the Internet. It is a textual data format with strong support via Unicode for the languages of the world. Although the design of XML focuses on documents, it is widely used for the representation of arbitrary data structures – for example in web services, configuration/settings, and GUI, workflow, and task definition.

Many application programming interfaces (APIs) have been developed to aid software developers with processing XML data, and several [schema languages](https://en.wikipedia.org/wiki/XML_schema_languages) exist to aid in the definition of XML-based languages. Schemas are usually defined with an external namespace, but XML also allows you to define tags within the document itself.

**XML Technologies**

*   [xquery](http://stackoverflow.com/questions/tagged/xquery "show questions tagged 'xquery'") ([the XML Query language](https://en.wikipedia.org/wiki/XQuery)) is a language for querying XML documents much like querying relational databases.
*   [xpath](http://stackoverflow.com/questions/tagged/xpath "show questions tagged 'xpath'") ([the XML Path language](https://en.wikipedia.org/wiki/XPath)) is a language for finding information in an XML document; it is a subset of of XQuery.
*   [xslt](http://stackoverflow.com/questions/tagged/xslt "show questions tagged 'xslt'") ([eXtensible Stylesheet Language Transformations](https://developer.mozilla.org/en-US/docs/Glossary/XSLT)) is used to transform XML documents.
*   [xlink](http://stackoverflow.com/questions/tagged/xlink "show questions tagged 'xlink'") ([the XML Linking language](https://en.wikipedia.org/wiki/XLink)) defines methods for creating links within XML documents.
*   [xpointer](http://stackoverflow.com/questions/tagged/xpointer "show questions tagged 'xpointer'") ([the XML Pointer language](https://en.wikipedia.org/wiki/XPointer)) allows hyperlinks to point to specific parts (fragments) of XML documents.

## Example Document

The following text is defined using [XHTML](https://www.w3.org/TR/xhtml1/) and [entity references](http://www.w3.org/TR/xml/#dt-entref); the text serves as an example of XML syntax and structure:

    <?xml version="1.0" encoding="UTF-8" ?>
    <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
      "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd" [
      <!ENTITY hello "Hello, World!">
    ]>
    <html xmlns="http://www.w3.org/1999/xhtml">
      <head>
        <meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
        <title>&hello;</title>
      </head>
      <body>
        <div>&hello;</div>
      </body>
    </html>

## Resources

The following links provide additional information to learn about XML:

*   [W3C's XML overview](http://www.w3.org/XML/)
*   [W3C's XML specification](http://www.w3.org/TR/xml/)
*   [_XML namespace_ on Wikipedia](https://en.wikipedia.org/wiki/Xml_namespace)
*   [XML resources on IBM developerWorks](https://www.ibm.com/developerworks/xml/)
*   [XML in the Mozilla Developer Network (MDN) Glossary](https://developer.mozilla.org/en-US/docs/Glossary/XML)
*   [James Clark's XML Resources](http://www.jclark.com/xml/)
*   [XML DTD XSLT XPath Tutorial on way2tutorial](http://www.way2tutorial.com/xml/xml_dtd_xslt_xpath_tutorials.php)

Code Language (used for [syntax highlighting](http://google-code-prettify.googlecode.com/svn/trunk/README.html)): lang-xml

  lang-xml