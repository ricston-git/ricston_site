## About ajax

AJAX (Asynchronous JavaScript and XML) is a technique for creating seamless interactive websites via asynchronous data exchange between client and server. AJAX facilitates communication with the server or partial page updates without a traditional page refresh.

**AJAX** stands for [Asynchronous](https://en.wikipedia.org/wiki/Asynchronous_I/O) [javascript](http://stackoverflow.com/questions/tagged/javascript "show questions tagged 'javascript'") and [xml](http://stackoverflow.com/questions/tagged/xml "show questions tagged 'xml'").

While not a technology in itself, AJAX is a term coined in 2005 by Jesse James Garrett, that describes a "new" approach to using a number of existing technologies together, including: HTML/XHTML, CSS, JavaScript, the DOM, XML, XSLT, and most importantly the [`XMLHttpRequest`](http://www.w3.org/TR/XMLHttpRequest2) object. AJAX uses the [`XMLHttpRequest`](http://www.w3.org/TR/XMLHttpRequest2) (abbreviated XHR) API to manage HTTP requests from inside the code.

When these technologies are combined in the AJAX model, web applications are able to make quick, incremental updates to the user interface without reloading the entire browser page. This makes the application faster and more responsive to user actions.

This communication is performed by [javascript](http://stackoverflow.com/questions/tagged/javascript "show questions tagged 'javascript'") code in the browser. Originally, it was anticipated that the data would be encoded in [xml](http://stackoverflow.com/questions/tagged/xml "show questions tagged 'xml'") form, hence the acronym AJAX. However the term is now used for all browser/server interaction of this type, even when XML is not used.

Although the X in AJAX stands for XML, any type of data can be accessed. [json](http://stackoverflow.com/questions/tagged/json "show questions tagged 'json'") ([JavaScript Object Notation](http://json.org)) is used more than XML nowadays because of its many advantages, including the availability of native methods to handle it, its lightness (compared to XML) and also being a strict subset of JavaScript. Both [json](http://stackoverflow.com/questions/tagged/json "show questions tagged 'json'") and XML can be used for packaging information in the AJAX model. Today, with the help of new `responseType` objects (`ArrayBuffer`, `Blob`, etc), you can even request binary files via [`XMLHttpRequest`](http://www.w3.org/TR/XMLHttpRequest2), and build much stronger and featured web apps.

[`XMLHttpRequest`](http://www.w3.org/TR/XMLHttpRequest2) is the main method of interacting between the [server](http://stackoverflow.com/questions/tagged/server "show questions tagged 'server'") and the [client](http://stackoverflow.com/questions/tagged/client "show questions tagged 'client'"); it is supported by all modern browsers. Early versions of Internet Explorer (IE 5 and 6) don't support the native XHR API, although they do support an ActiveX API which has most of the capabilities of XHR (an example of this is `new ActiveXObject("MSXML2.XMLHTTP.3.0")`).

**AJAX Example**

    var xmlhttp;
    if (window.XMLHttpRequest) { // code for IE7+, Firefox, Chrome, Opera, Safari
        xmlhttp = new XMLHttpRequest();
    } else { // code for IE6, IE5
        xmlhttp = new ActiveXObject("Microsoft.XMLHTTP");
    }
    xmlhttp.onreadystatechange = function() {
        if (xmlhttp.readyState == 4 && xmlhttp.status == 200) {
            //stuff to do with response text (xmlhttp.responseText)
        }
    }
    xmlhttp.open("GET", "url", true);
    xmlhttp.send();

**jQuery AJAX** Example

    $.ajax({
        url: "url",
        context: document.body
    }).done(function() {
        //stuff to do with response text
    });

### Useful links:

*   [AJAX on Wikipedia](https://en.wikipedia.org/wiki/Ajax_%28programming%29)
*   [The XMLHttpRequest Level 2 Working Draft on W3C](http://www.w3.org/TR/XMLHttpRequest2)
*   [Mozilla MDN](https://developer.mozilla.org/en-US/docs/AJAX)
*   [JSON - JavaScript Object Notation](http://json.org)
*   [jQuery.ajax() implementation](https://api.jquery.com/jQuery.ajax)
*   [ProtoypeJS Ajax implementation](http://api.prototypejs.org/ajax)
*   [Dojo Ajax implementation](https://dojotoolkit.org/reference-guide/1.7/quickstart/ajax.html)
*   [Ext JS Ajax implementation](https://www.sencha.com/products/extjs)
*   [Ajax: A new approach to web applications](https://web.archive.org/web/20080702075113/http://www.adaptivepath.com/ideas/essays/archives/000385.php)

Code Language (used for [syntax highlighting](http://google-code-prettify.googlecode.com/svn/trunk/README.html)): default

  default