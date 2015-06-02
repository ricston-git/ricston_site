## About javascript

JavaScript (not to be confused with Java) is a dynamic, weakly-typed language typically used for client-side scripting. Use this tag for questions regarding ECMAScript and its various dialects/implementations (excluding ActionScript). Unless a tag for a framework/library is also included, a pure JavaScript answer is expected.

**[JavaScript](https://en.wikipedia.org/wiki/JavaScript)** is a dynamic, object-based, prototype-based, weakly typed language commonly used for client-side scripting in web browsers. Despite the name, it is unrelated to the **[Java programming language](https://en.wikipedia.org/wiki/Java_programming_language)** and shares only superficial similarities.

Unless a tag for a framework or library is also included, a pure JavaScript answer is expected for questions with the [javascript](http://stackoverflow.com/questions/tagged/javascript "show questions tagged 'javascript'") tag.

JavaScript runs on nearly every Operating System, and an engine is included in almost every mainstream web browser. Developed in 1995 by [Brendan Eich](https://en.wikipedia.org/wiki/Brendan_Eich) at Netscape Communications, it was originally called [LiveScript](http://livescript.net/) but was renamed to JavaScript due to Netscape's friendly relationship with [Sun Microsystems](https://en.wikipedia.org/wiki/Sun_Microsystems) at the time.

Standalone JavaScript engines or interpreters are available as well, including:

*   Mozilla's [spidermonkey](http://stackoverflow.com/questions/tagged/spidermonkey "show questions tagged 'spidermonkey'"), the first JavaScript engine ever written, currently used in Mozilla Firefox.
*   [v8](http://stackoverflow.com/questions/tagged/v8 "show questions tagged 'v8'"), Google's JavaScript interpreter, used in Google Chrome.
*   [node.js](http://stackoverflow.com/questions/tagged/node.js "show questions tagged 'node.js'"), a platform which enables server-side applications to be written in JavaScript. Also see [io.js](http://stackoverflow.com/questions/tagged/io.js "show questions tagged 'io.js'"), a community fork of node.js.
*   Windows includes [jscript](http://stackoverflow.com/questions/tagged/jscript "show questions tagged 'jscript'"), a JavaScript variant in [Windows Script Host](http://en.wikipedia.org/wiki/Windows_Script_Host).
*   Mozilla also offers [rhino](http://stackoverflow.com/questions/tagged/rhino "show questions tagged 'rhino'"), an implementation of JavaScript built in Java, typically embedded into Java applications to provide scripting to end users.
*   [webkit](http://stackoverflow.com/questions/tagged/webkit "show questions tagged 'webkit'") (except for the Chromium project) implements the [javascriptcore](http://stackoverflow.com/questions/tagged/javascriptcore "show questions tagged 'javascriptcore'") engine.
*   [actionscript](http://stackoverflow.com/questions/tagged/actionscript "show questions tagged 'actionscript'") (originally derived from [HyperTalk](https://en.wikipedia.org/wiki/HyperTalk)) is now an ECMAScript dialect and uses a lot of ECMAScript APIs.
*   [duktape](http://stackoverflow.com/questions/tagged/duktape "show questions tagged 'duktape'") Embeddable, portable ECMAScript engine in C with small memory footprint.

The [Mozilla Developer Network](http://developer.mozilla.org/) contains high-quality [documentation on JavaScript](https://developer.mozilla.org/en/JavaScript).

JavaScript is typically used to manipulate the [Document Object Model](http://www.w3.org/DOM/DOMTR.html) (DOM) and [Cascading Style Sheets](https://en.wikipedia.org/wiki/Cascading_Style_Sheets) (CSS) within the browser, offering user interface scripting, animation, automation, client-side validation, and much more.

However, with the recent emergence of platforms such as [Node.js](http://nodejs.org/), JavaScript can now be used to write server-side applications. In addition, it is also used in environments that aren't Web-based, like PDF documents, site-specific browsers, desktop widgets etc.

## Nomenclature

Although it was developed under the name **Mocha**, the language was officially called LiveScript when it first shipped in beta releases of `Netscape Navigator 2.0` in September 1995, but it was renamed JavaScript when it was deployed in the Netscape browser version 2.0B3.

**The change of name from LiveScript to JavaScript roughly coincided with Netscape adding support for Java technology in its Netscape Navigator web browser**. The final choice of name caused confusion, giving the impression that the language was a spin-off of the Java programming language, and the choice has been characterized as a marketing ploy by Netscape to give JavaScript the cachet of what was then the hot new web programming language

People often use the term _JavaScript_ informally. The language and the term originated from [Netscape](https://en.wikipedia.org/wiki/Netscape). ECMAScript, JavaScript, and JScript are terms that are easy to confuse.

**[ECMAScript](https://en.wikipedia.org/wiki/ECMAScript)** was developed as a standardization of Netscape's [JavaScript](https://en.wikipedia.org/wiki/JavaScript) and Microsoft's independently-developed [JScript](http://msdn.microsoft.com/en-us/library/yek4tbz0.aspx). The canonical reference is the [ECMA-262 Language Specification](http://www.ecma-international.org/publications/standards/Ecma-262.htm). While JavaScript and JScript aim to be compatible with ECMAScript, they also provide additional features (and [other deviations](http://wiki.ecmascript.org/lib/exe/fetch.php?id=resources:resources&cache=cache&media=resources:jscriptdeviationsfromes3.pdf)) not described in the ECMA specifications. [Other implementations](https://en.wikipedia.org/wiki/ECMAScript#Dialects) of ECMAScript also exist.

The differences today for those who use JavaScript are negligible; people generally do not distinguish the JavaScript and JScript variations from ECMAScript.

### ECMAScript versions

Most modern browsers implement JavaScript based on the [ecmascript-5](http://stackoverflow.com/questions/tagged/ecmascript-5 "show questions tagged 'ecmascript-5'") specification. However, older browsers such as Internet Explorer 8 implement the ECMAScript 3 specification, which does not contain functions such as `Function.prototype.bind` and even `JSON.parse`, amongst others.

The current version of ECMAScript is version 5, however there have been [numerous draft versions](http://wiki.ecmascript.org/doku.php?id=harmony:specification_drafts) of the upcoming [ecmascript-6](http://stackoverflow.com/questions/tagged/ecmascript-6 "show questions tagged 'ecmascript-6'") specification, which will add numerous new features to JavaScript implementations, such as arrow functions and class syntax.

* * *

### When asking a JavaScript question, you should:

1.  Debug your JavaScript code (see [Creativebloq](http://www.creativebloq.com/javascript/javascript-debugging-beginners-3122820), [MDN](https://developer.mozilla.org/en-US/docs/Tools/Debugger), & [Google](https://developers.google.com/chrome-developer-tools/docs/javascript-debugging)).
2.  Isolate the problematic code and reproduce it in a [**Stackoverflow code snippet**](http://blog.stackoverflow.com/2014/09/introducing-runnable-javascript-css-and-html-code-snippets/) or an external online environment such as [**JSFiddle**](http://jsfiddle.net/) or [**JS Bin**](http://jsbin.com/) (remember to also include the code in the question itself).
3.  If a library or framework is used, then tag the question with the appropriate tags: [jquery](http://stackoverflow.com/questions/tagged/jquery "show questions tagged 'jquery'") for jQuery, [prototypejs](http://stackoverflow.com/questions/tagged/prototypejs "show questions tagged 'prototypejs'") for Prototype, [mootools](http://stackoverflow.com/questions/tagged/mootools "show questions tagged 'mootools'") for MooTools, and so on. However, if a framework is not used or necessary, do not include these tags.
4.  Mention which browser the code is having problems on, and what error messages, if any, were thrown by the browser. If the question is browser-specific, use tags [![](//i.stack.imgur.com/WcBXc.png)firefox](http://stackoverflow.com/questions/tagged/firefox "show questions tagged 'firefox'"), [![](//i.stack.imgur.com/EdUwb.png)google-chrome](http://stackoverflow.com/questions/tagged/google-chrome "show questions tagged 'google-chrome'"), [![](//i.stack.imgur.com/BfCOt.png)internet-explorer](http://stackoverflow.com/questions/tagged/internet-explorer "show questions tagged 'internet-explorer'"), [opera](http://stackoverflow.com/questions/tagged/opera "show questions tagged 'opera'"), [safari](http://stackoverflow.com/questions/tagged/safari "show questions tagged 'safari'"), etc.
5.  Only tag the question as [css](http://stackoverflow.com/questions/tagged/css "show questions tagged 'css'") or [html](http://stackoverflow.com/questions/tagged/html "show questions tagged 'html'") if you are asking about an issue that concerns the combination of one of those with JavaScript and could only be answered with information specifically regarding either of those subjects.

* * *

### Learning JavaScript

*   [Eloquent JavaScript](http://eloquentjavascript.net/): A Modern Introduction to Programming
*   [The MDN JavaScript Guide](https://developer.mozilla.org/en/JavaScript/Guide): A Comprehensive JavaScript Guide at the Mozilla Developer Network
*   [quirksmode.org - JavaScript](http://quirksmode.org/js/contents.html): Good introduction to JavaScript and other technologies used in the browser (e.g. DOM).
*   [JavaScript Tutorial](http://javascript.info/): A pure JavaScript book that covers _nearly_ everything.
*   [JavaScript Core Skills](http://dev.opera.com/articles/view/programming-the-real-basics/) from [the Web Standards Curriculum](https://dev.opera.com/blog/the-web-standards-curriculum-is-dead-long-live-webplatform-org/)
*   [quirksmode.org | Introduction to Events](http://www.quirksmode.org/js/introevents.html): A comprehensive description of the various types of event handling. Includes overview of different ways to attach event handlers and points out quirks between different browsers. A must-read if you want to understand event handling.
*   [W3C Wiki | JavaScript basics, DOM](http://www.w3.org/wiki/Category:Tutorials): [Programming - the real basics](http://www.w3.org/wiki/Programming_-_the_real_basics), [Creating and modifying HTML](http://www.w3.org/wiki/Creating_and_modifying_HTML), [Handling events with JavaScript](http://www.w3.org/wiki/Handling_events_with_JavaScript).
*   [JavaScript Debugging for Beginners](http://www.creativebloq.com/javascript/javascript-debugging-beginners-3122820): A good introduction to debugging JavaScript. A must-read!
*   [Modern JavaScript: Develop and Design](http://www.larryullman.com/books/modern-javascript-develop-and-design/): A modern guide to learning JavaScript using practical examples and approaches that should be used today.
*   [Learning Advanced JavaScript](http://ejohn.org/apps/learn/): A set of interactive exercises that guide you through some of the fundamental concepts of JavaScript.

### Useful Tools

*   [Firebug](https://getfirebug.com/) Add-on for Firefox
*   [Firefox Developer Tools](https://developer.mozilla.org/en-US/docs/Tools) for Firefox
*   [Developer Tools](http://www.microsoft.com/en-us/download/details.aspx?id=18359) for IE
*   [Chrome Developer Tools](https://developer.chrome.com/devtools/index) for Chrome
*   [Web Inspector](https://developer.apple.com/safari/tools/) for Safari

### Interactive JavaScript learning

*   [Codecademy | JavaScript](http://www.codecademy.com/en/tracks/javascript): Learn the fundamentals of JavaScript and dynamic programming.
*   [Udacity | Programming Languages](https://www.udacity.com/course/cs262): Key concepts include specifying and processing valid strings, sentences and program structures.

### Wisdom from the Stack

*   [What should every JavaScript programmer know?](http://stackoverflow.com/questions/2628672/what-should-every-javascript-programmer-know)
*   [Hidden Features of JavaScript?](http://stackoverflow.com/questions/61088/hidden-features-of-javascript)
*   [How do JavaScript closures work?](http://stackoverflow.com/questions/111102/how-do-javascript-closures-work)
*   [Return value from function with an Ajax call](http://stackoverflow.com/questions/562412/return-value-from-function-with-an-ajax-call)
*   [var functionName = function() {} vs function functionName() {}](http://stackoverflow.com/questions/336859/javascript-var-functionname-function-vs-function-functionname)
*   [How does the (function() {})() construct work and why do people use it?](http://stackoverflow.com/questions/1639180/how-does-the-function-construct-work-and-why-do-people-use-it)
*   [What is the scope of variables in JavaScript?](http://stackoverflow.com/questions/500431/what-is-the-scope-of-variables-in-javascript)
*   [What does this symbol mean in JavaScript?](http://stackoverflow.com/questions/9549780/what-does-this-symbol-mean-in-javascript)

### Useful links

*   [MDN JavaScript Reference](https://developer.mozilla.org/en-US/docs/JavaScript/Reference)
*   [W3C DOM Core](http://www.quirksmode.org/dom/w3c_core.html), [HTML](http://www.quirksmode.org/dom/w3c_html.html), [events](http://www.quirksmode.org/dom/events/index.html) and [CSS](http://www.quirksmode.org/dom/w3c_css.html) compatibility tables from [http://www.quirksmode.org](http://www.quirksmode.org)
*   [JSLint](http://www.jslint.com) Code Quality Tool by [Douglas Crockford](http://www.crockford.com/) (and [JSHint](http://jshint.com), a community-driven branch of the original)
*   Code minifiers/obfuscators: [/packer/](http://dean.edwards.name/packer/), [YUI Compressor](http://developer.yahoo.com/yui/compressor/), [Google Closure Compiler](http://closure-compiler.appspot.com/home), [UglifyJS](https://github.com/mishoo/UglifyJS/#readme)
*   Code formatter/deobfuscator: [JSBeautifier](http://jsbeautifier.org/)
*   Idioms and Gotchas: [Rounding](http://www.merlyn.demon.co.uk/js-round.htm), [Date Object](http://www.merlyn.demon.co.uk/js-date8.htm), [Number Object](http://www.hunlock.com/blogs/The_Complete_Javascript_Number_Reference), [Scope Chain](http://dmitrysoshnikov.com/ecmascript/chapter-4-scope-chain/), [Namespacing](http://michaux.ca/articles/javascript-namespacing)
*   [JavaScript Garden](http://bonsaiden.github.com/JavaScript-Garden)
*   [comp.lang.javascript FAQ](http://www.fortybelow.ca/hosted/comp-lang-javascript/faq/): Very extensive guide on JavaScript quirks created by Usenet's [comp.lang.javascript](https://groups.google.com/group/comp.lang.javascript/topics)
*   [ECMA 262-5 Online](http://www.ecma-international.org/ecma-262/5.1/): HTML version of the ECMAScript 5 specification.
*   [Annotated ES5](http://es5.github.com/): Annotated and hyperlinked HTML derivative of the ECMAScript 5 specification.
*   [Unofficial ES6 draft spec](http://people.mozilla.org/~jorendorff/es6-draft.html).
*   [ECMAScript Support Matrix](http://pointedears.de/scripts/test/es-matrix/): In-depth feature list for ECMAScript implementations.
*   [ES6 compatibility table](http://kangax.github.io/es5-compat-table/es6/)
*   [JavaScript Weekly](http://www.javascriptweekly.com): A free, weekly newsletter curated by Peter Cooper

### Free JavaScript Programming Books

*   [Crockford's JavaScript](http://www.crockford.com/javascript/)
*   [Eloquent JavaScript](http://eloquentjavascript.net/)
*   [Essential JavaScript & jQuery Design Patterns for Beginners](http://www.addyosmani.com/resources/essentialjsdesignpatterns/book/)
*   [JavaScript Essentials](http://www.techotopia.com/index.php/JavaScript_Essentials)
*   [jQuery Fundamentals](http://jqfundamentals.com/legacy/) (starts with JavaScript basics)
*   [Mozilla Developer Network's JavaScript Guide](https://developer.mozilla.org/en/JavaScript/Guide)
*   [Enterprise Web Development: From Desktop to Mobile](http://enterprisewebbook.com/)

### Videos

*   [YUI Library](https://www.youtube.com/user/yuilibrary/playlists)
*   [AngularJS Channel](https://www.youtube.com/user/angularjs/playlists)
*   [LearnCode.academy](https://www.youtube.com/user/learncodeacademy/playlists)
*   [JavaScript Planet](https://www.youtube.com/channel/UCzVnCG4ItKitN1SCBM7-AbA/playlists)
*   [Google Chrome Developer Tools](https://developer.chrome.com/devtools/docs/videos)

* * *

## Example JavaScript code

This script displays "Hello World" on your screen.

    window.onload = function() {
       alert('Hello World!');
    }

[Demo!](http://jsfiddle.net/YSQ56/)

* * *

## Frequently Asked Questions

Find some answers to some of the more frequently asked questions about JavaScript and related technology below.

**Q:** I have this JSON structure, how can I access property `x.y.z`?  
 **A:** [Access / process (nested) objects, arrays or JSON](http://stackoverflow.com/q/11922383)

**Q:** I'm adding events in a for loop but all handlers do the same thing, why?  
 **A:** [JavaScript closure inside loops – simple practical example](http://stackoverflow.com/questions/750486/javascript-closure-inside-loops-simple-practical-example)

**Q:** I want to compare something against multiple values, is there an easy way to do it?  
 **A:** [Concise way to compare against multiple values](http://stackoverflow.com/questions/13737091/concise-way-to-compare-against-multiple-values)

**Q:** How can I pass a PHP array to JavaScript?  
 **A:** [Pass a PHP array to a JavaScript function](http://stackoverflow.com/questions/4885737/pass-php-array-to-javascript-function)

**Q:** How to set up proper inheritance?  
 **A:** [Objects don't inherit prototyped functions](http://stackoverflow.com/questions/11072556/objects-dont-inherit-prototyped-functions/11072626)

**Q:** How do JavaScript closures work?  
 **A:** [How do JavaScript closures work?](http://stackoverflow.com/questions/111102/how-do-javascript-closures-work/)

**Q:** Why does `setTimeout()` inside a `for` loop always use the latest value?  
 **A:** [setTimeout in for-loop does not print consecutive values](http://stackoverflow.com/questions/5226285)

**Q:** How to return the response from an AJAX call from a function?  
 **A:** [How to return the response from an asynchronous call?](http://stackoverflow.com/questions/14220321)

**Q:** Why don't my handlers hooked up in a loop work correctly, and what can I do about it?  
 **A:** [Javascript: generate dynamically handler](http://stackoverflow.com/questions/16794707/javascript-generate-dynamically-handler/16794762#16794762)

**Q:** How can I get query string values?  
 **A:** [How can I get query string values in JavaScript?](http://stackoverflow.com/questions/901115)

**Q:** What does “use strict” do in JavaScript?  
 **A:** [What does "use strict" do in JavaScript, and what is the reasoning behind it?](http://stackoverflow.com/questions/1335851/what-does-use-strict-do-in-javascript-and-what-is-the-reasoning-behind-it)

**Q:** How can I make a redirect page in jQuery/JavaScript?  
 **A:** [How can I make a redirect page using jQuery?](http://stackoverflow.com/questions/503093/how-can-i-make-a-redirect-page-in-jquery-javascript)

**Q:** How to sort an array of objects by a property value?  
 **A:** [Sort array of objects by property value in JavaScript](http://stackoverflow.com/questions/1129216/sorting-objects-in-an-array-by-a-field-value-in-javascript)

**Q:** I'm adding elements with JavaScript or jQuery at a later point and adding events but they're not firing, why?  
 **A:** You might want [event delegation](http://stackoverflow.com/questions/1687296/what-is-dom-event-delegation).

**Q:** How can I only keep items of an array that match a certain condition?  
 **A:** [How can I only keep items of an array that match a certain condition?](http://stackoverflow.com/questions/27131984/how-can-i-only-keep-items-of-an-array-that-match-a-certain-condition)

## More information:

*   [Wikipedia on JavaScript](http://en.wikipedia.org/wiki/JavaScript)
*   [MDN - Learn JavaScript](https://developer.mozilla.org/en-US/learn/javascript)
*   [Creator of JavaScript, Brendan Eich, explains the origin](http://www.youtube.com/watch?feature=player_embedded&v=IPxQ9kEaF8c)

## Chat Room

*   [Stack Overflow chat room for JavaScript](http://chat.stackoverflow.com/rooms/17/javascript)

Code Language (used for [syntax highlighting](http://google-code-prettify.googlecode.com/svn/trunk/README.html)): default

  default