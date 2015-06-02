## About css

CSS (Cascading Style Sheets) is a style sheet language used for describing the look and formatting of HTML (Hyper Text Markup Language) and XML (Extensible Markup Language) documents including (but not limited to) colors, layout, and fonts.

[**CSS**](http://en.wikipedia.org/wiki/Cascading_Style_Sheets), short for **Cascading Style Sheets**, is a language used to control the visual presentation of documents written in a markup language, including [html](http://stackoverflow.com/questions/tagged/html "show questions tagged 'html'"), [xml](http://stackoverflow.com/questions/tagged/xml "show questions tagged 'xml'"), [xhtml](http://stackoverflow.com/questions/tagged/xhtml "show questions tagged 'xhtml'"), [svg](http://stackoverflow.com/questions/tagged/svg "show questions tagged 'svg'") and [xul](http://stackoverflow.com/questions/tagged/xul "show questions tagged 'xul'"). In early days, the visual presentation was defined by HTML attributes; then CSS was introduced to separate the control of the visual presentation from the content.

A basic CSS document is made of rule sets. Each rule set starts with a [**selector**](http://www.w3.org/TR/css3-selectors/) (a pattern that matches elements in an **HTML** or **XML** document) and is followed by a block of one or more property declarations that define the presentation of the matching elements. For example:

    /* This is a comment */ 

    a {                             /* Find all <a> elements(HTML links), */
        color: orange;              /* change their text color to orange, */
        background-color: pink;     /* their background color to pink, */
        text-decoration: none;      /* and remove the underline. */
    }

    a:hover {                       /* But when you hover over an <a> element */
        color: red;                 /* change the color to red */
        text-decoration: underline; /* and add an underline again */
    }

The simple example above also illustrates why they are called _cascading_ style sheets. When you hover over a link (i.e., an `<a>` element) in [an HTML page with this style sheet applied to it](http://www.htmldog.com/guides/cssbeginner/applyingcss/), _both_ rules apply. So, the link will have a pink background. But, since the `a:hover` selector is more specific, its `color` and `text-decoration` properties override those from the `<a>` rule set.

The [cascading order](http://www.w3.org/TR/CSS2/cascade.html#cascade) defines how [specificity](http://www.stuffandnonsense.co.uk/archives/css_specificity_wars.html) and other factors determine which property value is applied to an element.

Some more CSS, continuing from the example above:

    /* Selectors with greater Specificity override less specific ones */
    #article a.tag {
        color: #F00;
    }

    /* Complex selectors can be created from joining multiple simple ones together */
    #sidebar > h3 + p a:first-child {
        border-bottom: 1px solid #333;
        font-style: italic;
    }

    /* It is also possible to style elements depending on an attribute */
    div[id] a[target="_blank"] {
        color: white;
    }

## Selector precedence

Each component of a CSS selector can be based on one of three possible attributes of an HTML element:

1.  The element's ID (from the `id` attribute)
2.  The name of one of the element's classes (in the `class` attribute)
3.  The element's tag name

Selectors using an ID selector have higher priority than selectors using class names, and selectors using a class name have higher priority than selectors using tag names. This is called selector precedence. `!important` can be used to override the selector precedence. Whenever possible though, higher specificity should always be used instead of `!important`, in order to prevent overrides on any other styles that might need to be added.

For example:

    <!-- Creates an anchor with a class of class1 and an ID of anchor1 -->
    <a class="class1" id="anchor1">Sample</a>

    a {                 /* anchor element */
        color: orange;
    }

    .class1 {           /* any element with class name class1 */
        color: red;
    }    

    #anchor1 {          /* the element with id anchor1 */
        color: green;
    }

In the above example, the color of the string "Sample" will be green.

Repeated occurrences of the same selector also increase specificity, as noted in the [Selectors Level 3 W3C Recomendation](http://www.w3.org/TR/css3-selectors/#specificity).

    .class1.class1 {    /* repeated class selector */
        font-weight: bold;
    }

    .class1 {
        font-weight: normal;
    }

Here the repeated selector has higher specificity than the singular selector and the `font-weight` of our sample string will be bold.

### Important Notice:

For questions related to CSS, always, try to demonstrate your code in a reproducible manner [using either Stack Exchange's Stack Snippets](http://blog.stackoverflow.com/2014/09/introducing-runnable-javascript-css-and-html-code-snippets/) or alternatively any online editor that allows running and sharing code such as [jsbin](http://stackoverflow.com/questions/tagged/jsbin "show questions tagged 'jsbin'") or [jsfiddle](http://stackoverflow.com/questions/tagged/jsfiddle "show questions tagged 'jsfiddle'") (though be sure to always include relevant code _in_ the question).

* * *

### References

*   [W3C CSS2.1 Specification](http://www.w3.org/TR/CSS2/)
*   [W3C CSS3 Selectors Specification](http://www.w3.org/TR/css3-selectors/)
*   [W3C CSS3 Media Queries Specification](http://www.w3.org/TR/css3-mediaqueries/)
*   [W3C Cascading Style Sheets home page](http://www.w3.org/Style/CSS/)
*   [Way2Tutorial CSS Tutorial](http://way2tutorial.com/css/tutorial.php)
*   [SitePoint CSS Reference](http://reference.sitepoint.com/css)
*   [HTML Dog: HTML and CSS Tutorials](http://htmldog.com/)
*   [Cascading Style Sheets on the Web Standards Curriculum](http://dev.opera.com/articles/view/27-css-basics/)
*   [The 30 CSS Selectors you Must Memorize](http://net.tutsplus.com/tutorials/html-css-techniques/the-30-css-selectors-you-must-memorize/)
*   [W3C Web Content Accessibility Guidelines](http://www.w3.org/TR/WCAG20/)
*   [DocHub Instant Documentation Search](http://dochub.io/#css/)
*   [DevDocs - Documentation Searching Service](http://devdocs.io/css/)
*   [W3Schools CSS Tutorials](http://www.w3schools.com/css/default.asp "w3schools CSS Tutorials")
*   [Learn CSS Layouts](http://learnlayout.com)
*   [Demonstration of all combination of css selectors by w3schools](http://www.w3schools.com/cssref/trysel.asp)

    ### CSS Pseudo Selector

*   [CSS Pseudo Class Selector](http://way2tutorial.com/css/css_pseudo_class_selector.php)

*   [Pseudo Element](http://www.w3schools.com/css/css_pseudo_elements.asp)

### Validation

*   [W3C CSS Validation Service](http://jigsaw.w3.org/css-validator/)
*   [CSS Lint](http://csslint.net/)
*   [CSS Portal](http://www.cssportal.com/css-validator/)

### Browser Support

*   [MDN: Mozilla CSS support chart](https://developer.mozilla.org/en/Mozilla_CSS_support_chart)
*   [MSDN: CSS Compatibility and Internet Explorer](http://msdn.microsoft.com/en-us/library/cc351024%28v=vs.85%29.aspx)
*   [Opera web specification support pages](http://www.opera.com/docs/specs/presto29/#opsupport)
*   [Konqueror CSS support](http://www.konqueror.org/css/)
*   [QuirksMode CSS](http://www.quirksmode.org/css/contents.html)
*   [When can I use... Compatibility tables for CSS3 and more](http://caniuse.com/)
*   [CSS3 Selectors Test](http://www.css3.info/selectors-test/)
*   [Wikipedia: Comparison of layout engines](http://en.wikipedia.org/wiki/Comparison_of_layout_engines_(Cascading_Style_Sheets))

### CSS Pre-processors

*   [LessCSS](http://lesscss.org)
*   [SASS](http://sass-lang.com)
*   [Stylus](http://learnboost.github.com/stylus/)
*   [Examples](http://csspre.com)

### Reset Stylesheets

*   [Eric Meyer's reset.css](http://meyerweb.com/eric/tools/css/reset/)
*   [HTML5 Reset Stylesheet](http://html5doctor.com/html-5-reset-stylesheet/)
*   [CSS Wizardry Reset restarted](http://csswizardry.com/2011/10/reset-restarted/)
*   [Normalize.css](http://necolas.github.com/normalize.css/)

### CSS Frameworks

*   [Blueprint](http://blueprintcss.org/) [blueprint-css](http://stackoverflow.com/questions/tagged/blueprint-css "show questions tagged 'blueprint-css'")
*   [960 CSS Framework](http://960.gs/) [960.gs](http://stackoverflow.com/questions/tagged/960.gs "show questions tagged '960.gs'")
*   [jQuery UI CSS Framework](http://docs.jquery.com/UI/Theming/API#The_jQuery_UI_CSS_Framework) [jquery-ui-css-framework](http://stackoverflow.com/questions/tagged/jquery-ui-css-framework "show questions tagged 'jquery-ui-css-framework'")
*   [YAML](http://www.yaml.de/en/) [yaml](http://stackoverflow.com/questions/tagged/yaml "show questions tagged 'yaml'")
*   [YUI CSS Grids](http://yuilibrary.com/) [yui](http://stackoverflow.com/questions/tagged/yui "show questions tagged 'yui'")
*   [Twitter Bootstrap](http://getbootstrap.com/) [twitter-bootstrap](http://stackoverflow.com/questions/tagged/twitter-bootstrap "show questions tagged 'twitter-bootstrap'")
*   [HTML5 ★ BOILERPLATE](http://html5boilerplate.com//) [html5boilerplate](http://stackoverflow.com/questions/tagged/html5boilerplate "show questions tagged 'html5boilerplate'")
*   [Zurb's Foundation](http://foundation.zurb.com/) [zurb-foundation](http://stackoverflow.com/questions/tagged/zurb-foundation "show questions tagged 'zurb-foundation'")
*   [Skeleton](http://getskeleton.com/) [skeleton-css-boilerplate](http://stackoverflow.com/questions/tagged/skeleton-css-boilerplate "show questions tagged 'skeleton-css-boilerplate'")
*   [inuit.css](http://inuitcss.com/) [inuit.css](http://stackoverflow.com/questions/tagged/inuit.css "show questions tagged 'inuit.css'")
*   [Jeet Grid System](http://jeet.gs/) [jeet-grid](http://stackoverflow.com/questions/tagged/jeet-grid "show questions tagged 'jeet-grid'")
*   [Gumby](http://gumbyframework.com/) [gumby-framework](http://stackoverflow.com/questions/tagged/gumby-framework "show questions tagged 'gumby-framework'")

### Actual Version

*   [CSS3](http://en.wikipedia.org/wiki/Cascading_Style_Sheets#CSS_3) (CSS3 is the latest standard for CSS)

### The Future

The following currently have very little (if any) browser support and are still a work in-progress:

*   [W3C Selectors Level 4 Draft](http://www.w3.org/TR/selectors4/)
*   [W3C Custom Properties (CSS Variables) Draft](http://www.w3.org/TR/css-variables/)

### Chat Room

Chat about CSS (and HTML / DOM) with other Stack Overflow users:

*   [HTML / CSS / DOM & web design](http://chat.stackoverflow.com/rooms/29074/html-css-dom-web-design)

Code Language (used for [syntax highlighting](http://google-code-prettify.googlecode.com/svn/trunk/README.html)): default

  default