## About regex

Regular expressions (often shortened to "regex") are expressions written in a declarative language used for matching patterns within strings. General reference: http://stackoverflow.com/q/22937618 Remember to include a tag specifying the programming language or tool you are using.

# Regular and Irregular Expressions

[Regular expression](http://en.wikipedia.org/wiki/Regular_expression) is a powerful form of [declarative programming languages](http://en.wikipedia.org/wiki/Declarative_programming), mainly used for pattern-matching within strings. Its corresponding machine model is the [finite automaton](http://en.wikipedia.org/wiki/Finite-state_machine).

There are many different dialects (also called **flavors**) of regular expressions, all subtly different. Therefore, when asking questions, **_always_ include the tag for the specific programming language or tool** (_e.g.,_ Perl, Ruby, Python, Java, JavaScript, vi, Emacs, sed, Lex, grep, _etc._) you are using. Otherwise, you may get answers that won't work for you. See below for a short outline of different dialects.

Depending on which flavor you’re using, modern regular expression engines can support advanced features like [backreferences](http://www.regular-expressions.info/backref.html), [conditional subpatterns](http://www.regular-expressions.info/conditional.html), regular expression [subroutines](http://www.regular-expressions.info/subroutine.html), [code callouts](http://www.regular-expressions.info/pcre.html#callout), positive and negative [lookahead/lookbehind assertions](http://www.regular-expressions.info/lookaround.html), and even [recursion](http://www.regular-expressions.info/recurse.html). This rich feature-set allows them to parse far more than the [strictly regular languages](http://en.wikipedia.org/wiki/Regular_language) for which they were originally named.

Today, we still call these pattern-matching languages _regular expressions_ (or _regexes_ for short), even if they may no longer be _regular_ in the computer scientific sense.

Regular expressions are used for two purposes: input validation and data extraction. Regular expressions for input validation must accept _all_ input allowed by standard (if any) or requirement and reject everything else, and it must do so correctly on arbitrary input string, without any assumption. Such regular expressions can be very complex, but their strictness makes them full-fledged parsers capable of extracting data. On the other hand, regular expression for data extraction only needs to work correctly on a certain input domain, which may or may not be well-defined. Such regular expression usually comes with assumptions on certain features of the data, which makes it fragile and subject to breakage on unexpected change in the input domain.

# _Fools Rush in Where Angels Fear to Tread_

The tremendous power and expressiveness of modern regular expressions can seduce the gullible — or the foolhardy — into trying to use regular expressions on every string-related task they come across. This is a bad idea in general, and a _very_ bad idea in one particular area. Although it is perfectly appropriate to use regular expressions on [_specific_ XML or HTML of known characteristics](http://stackoverflow.com/q/1732348/3622940), attempting to fully and correctly parse _arbitrary_ XML or HTML using regular expressions alone has been known to [induce madness](http://stackoverflow.com/a/1732454/3622940) in those attempting this [Herculean](http://en.wiktionary.org/wiki/Herculean#Adjective) and [Sisyphean](http://en.wiktionary.org/wiki/Sisyphean#Adjective) task.

For **general parsing of arbitrary XML or HTML,** it is therefore always better to use a dedicated parser — like an [event-driven SAX parser](http://en.wikipedia.org/wiki/Simple_API_for_XML#XML_processing_with_SAX) or a [DOM parser](http://en.wikipedia.org/wiki/Document_Object_Model) — than it is to use regular expressions.

# **How to ask regex-based questions**

*   Different languages have different regex implementations. So it's wise to mention the language in which you want your regex to work. If you are not specific about the language, do mention it.

*   Regex questions are better explained with examples than elaborate sentences. Give us examples of what needs to be matched and what shouldn't.

*   Even if you are not well versed in regexes, it's better to show us what you've tried than simply asking the community to solve your problem.

*   Use online tools like [Regex101](http://regex101.com/), [RegExr](http://gskinner.com/RegExr/), and [RegexPal](http://regexpal.com/) to verify your regex patterns. You can even paste links from these sites to show us what you tried and what are the results. See below for more sites you can try.

*   Ensure your question is a regular expression and not a filename expansion (tag: [glob](http://stackoverflow.com/questions/tagged/glob "show questions tagged 'glob'")) often used on command lines to match files to pass as parameters to a command.

* * *

# Regular Expression Patterns

> The examples below use slashes as delimiters around the regular expressions. This is a moderately common convention, and some languages (like JavaScript) use it to delimit regex [literals](https://en.wikipedia.org/wiki/Literal_%28computer_programming%29), but not part of the regular expression syntax proper.

## Escaping

*   `\` Escapes special characters to literal and literal characters to special.

> **eg:** `/\[\.\]/` matches the literal string "[.]", whereas without the middle backslash, it would match any character between square brackets, and without any backslashes, it would only match exactly one literal dot.
> 
> **eg:** `/\(s\)/` matches '(s)' while `/(\s)/` matches any whitespace and captures the match... _in some dialects._

## Quantifiers

Quantifiers match the preceding sub-pattern a certain number of times. The sub-pattern can be a single character, an escape sequence, a pattern enclosed by parentheses or a character set.

*   `{n}` matches exactly n times.
*   `{n,}` matches n or more times.
*   `{n,m}` matches n to m times.
*   `*` is short for `{0,}`. Matches zero or more times.
*   `+` is short for `{1,}`. Matches one or more times.
*   `?` is short for `{0,1}`. Matches zero or one time.

> **eg:** `/o{1,3}/` matches 'oo' in "tooth" and 'o' in "nose".

`*` is universally supported. Traditional `grep` did not support the other quantifiers; they were introduced with extended regular expressions (i.e. `egrep`).

## Pattern delimiters

Matches entire contained pattern.

*   `(pattern)` captures match.
*   `(?:pattern)` doesn't capture match

> **eg:** `/(d).\1/` matches 'dad' and captures 'd' in "abcdadef" while `/(?:.d){2}/` matches but doesn't capture 'cdad'.

Traditional `grep` did not support grouping or capturing; it was introduced with extended regular expressions (i.e. `egrep`).

Non-capturing matches were introduced in Perl 5 and are only supported in relatively modern regular expression implementations.

## Lookahead

A lookahead matches only if the preceding subexpression is followed by the pattern, but the pattern is not part of the match. The subexpression is the part of the regular expression which will be matched.

*   `(?=pattern)` matches only if there is a following pattern in input.
*   `(?!pattern)` matches only if there is not a following pattern in input.

> **eg:** `/Win(?=98)/` matches 'Win' only if 'Win' is followed by '98'.

Lookaheads were introduced in Perl 5 and are only supported in relatively modern regular expression implementations.

## Alternation

*   `|` Alternation matches content on either side of the alternation character.

> **eg:** `/(a|b)a/` matches 'aa' in "dseaas" and 'ba' in "acbab".

Traditional `grep` did not support alternation; it was introduced with extended regular expressions (i.e. `egrep`).

## Character classes

Matches any one of the contained characters. A range of characters may be defined by using a hyphen.

*   `[characters]` matches any one of the contained characters.
*   `[^characters]` negates the character set and matches one character which is not (newline or) one of the contained characters

> **eg:** `/[abcd]/` matches one character which can be any of the characters 'a', 'b', 'c', or 'd' and may be abbreviated to `/[a-d]/`. Ranges must be in ascending order, otherwise they will throw an error. (**eg:** `/[d-a]/` will throw an error.) `/[^0-9]/` matches all characters but digits. **note:** Most special characters are automatically escaped to their literal meaning in character sets.

## Special characters

Special characters are characters that match something else than what they appear as.

*   `^` matches beginning of input (or new line with m flag).
*   `$` matches end of input (or end of line with m flag).
*   `.` matches any character except a newline.
*   `?` directly following a quantifier makes the quantifier non-greedy (makes it match minimum instead of maximum of the interval defined).

> **eg:** `/(.)*?/` matches nothing or `''` in all strings.  
>  **note:** Non-greedy matches are not supported in older browsers such as Netscape Navigator 4 or Microsoft Internet Explorer 5.0.

Non-greedy matching was introduced in Perl 5 and is only supported in relatively modern regular expression implementations.

## Literal characters

All characters except those with special meaning. Mapped directly to the corresponding character.

> **eg:** `/a/` matches 'a' in **Any ancestor**.

## Back references

*   `\n` Back references are references to the same thing as a previously captured match. n is a positive nonzero integer telling the browser which captured match to reference to.

*   `/(\S)\1(\1)+/g` matches all occurrences of three equal non-whitespace characters following each other.

*   `/<(\S+).*>(.*)<\/\1>/` matches any tag.

> **eg:** `/<(\S+).*>(.*)<\/\1>/` matches `<div id="me">text</div>` in text `<div id=\"me\">text</div>`.

Traditional `grep` did not support back references; they were introduced with extended regular expressions (i.e. `egrep`).

## Character Escapes

*   `\f` matches form-feed.
*   `\r` matches carriage return.
*   `\n` matches linefeed.
*   `\t` matches horizontal tab.
*   `\v` matches vertical tab.
*   `\0` matches `NUL` character.
*   `[\b]` matches backspace.
*   `\s` matches whitespace (short for `[\f\n\r\t\v\u00A0\u2028\u2029]`).
*   `\S` matches anything but a whitespace (short for `[^\f\n\r\t\v\u00A0\u2028\u2029]`).
*   `\w` matches any alphanumerical character (word characters) including underscore (short for `[a-zA-Z0-9_]`).
*   `\W` matches any non-word characters (short for `[^a-zA-Z0-9_]`).
*   `\d` matches any digit (short for `[0-9]`).
*   `\D` matches any non-digit (short for `[^0-9]`).
*   `\b` matches a word boundary (the position between a word and a space).
*   `\B` matches a non-word boundary (short for `[^\b]`).
*   `\cX` matches a control character. (**eg:** `\cm` matches control-M).
*   `\xhh` matches the character with two characters of hexadecimal code `hh`.
*   `\uhhhh` matches the Unicode character with four characters of hexadecimal code `hhhh`.

Many of these escapes were introduced in Perl and are only available in relatively modern regular expression implementations.

* * *

## Main Dialects

[The first implementation of regular expressions](http://dl.acm.org/citation.cfm?doid=363347.363387) was [Ken Thompson's](http://en.wikipedia.org/wiki/Ken_Thompson) for [`ed`](http://en.wikipedia.org/wiki/Ken_Thompson) and then [`grep`](http://en.wikipedia.org/wiki/Ed_%28text_editor%29) in 1968. This basically only implemented character classes, `^`, `$`, `.`, and `*` as well as backslash escapes.

This was later formalized into POSIX **Basic Regular Expressions** (BRE) with numerous additions, many of which -- somewhat bewilderingly, for reasons of backwards compatibility -- use the backslash to produce a metacharacter out of a regular character, rather than the other way around.

Later, an _extended_ `grep` aka `egrep` was introduced by [Alfred V. Aho](http://en.wikipedia.org/wiki/Alfred_Aho) which significantly expanded the repertoire of metacharacters. Although many additions were mere convenience, the extensions included grouping, alteration, and back references, which significantly extend the expressive power of the formalism.

These extensions were later formalized into POSIX **Extended Regular Expressions**.

POSIX also unified the tool, specifying that plain `grep` accepts basic regular expressions, while `grep -E` accepts extended regular expressions. Also, `grep -F` is provided as a replacement for `fgrep`, also originally by Aho, which performs search on literal strings, not regular expressions.

The [Perl programming language](http://en.wikipedia.org/wiki/Perl) featured a significantly modified and enhanced version of [Henry Spencer's](http://en.wikipedia.org/wiki/Henry_Spencer) regular expression library. With the release of Perl v5, further enhancements including lookaheads, lookbehinds, non-committing matches, non-capturing groups etc. were introduced. Through [Philip Hazel's](http://en.wikipedia.org/wiki/Philip_Hazel) library reimplementation [PCRE](http://pcre.org/), these capabilities were made available in many other programming languages, including, but not limited to, PHP, Python, and R. Hence, **Perl-Compatible Regular Expressions** are the third main dialect of regular expressions in widespread use.

Many tools have their own regular expression implementations which fall between these categories. For example many text editors implement their own dialects. [JavaScript](http://www.regular-expressions.info/javascript.html) also does this, and codifies its own dialect as part of the [ECMA-262 standard](http://en.wikipedia.org/wiki/ECMAScript).

* * *

## Useful links

### Learning regular expressions

*   [Learn Regex The Hard Way (Online book)](http://regex.learncodethehardway.org/book/)
*   [Text2Re – Generate Regular expressions based on a string](http://txt2re.com/)
*   [Basic concept of how RegularExpression parsing works](http://swtch.com/~rsc/regexp/regexp1.html)
*   [Wikipedia entry on regular expressions](http://en.wikipedia.org/wiki/Regular_expression)
*   [O'Reilly – Mastering Regular Expressions (e-book)](http://shop.oreilly.com/product/9780596528126.do)
*   [O'Reilly – Regular Expressions Cookbook (e-book)](http://shop.oreilly.com/product/0636920023630.do)
*   [O'Reilly – Regular Expression Pocket Reference (e-book)](http://shop.oreilly.com/product/9780596514273.do)
*   [A Tao Of Regular Expressions (e-book)](http://www.cs.colorado.edu/~schenkc/UNIX_Regular_Expressions.pdf) (pdf link)
*   [Regular-Expressions.info](http://www.regular-expressions.info/) (informative website for learning regular expressions)
*   [RexEgg](http://www.rexegg.com/) (a regular expressions tutorial that goes deep into advanced features)
*   [RegexOne](http://regexone.com/) ("learn regular expressions with simple, interactive examples")

### Documentation for JavaScript

*   [Mozilla Developer Network](https://developer.mozilla.org/en/docs/Web/JavaScript/Guide/Regular_Expressions)
*   [Microsoft Developer Network](http://msdn.microsoft.com/en-US/library/9dthzd08(v=vs.94).aspx)

### Online sandboxes (for testing and publishing regexes online)

*   [RegexPlanet](http://www.regexplanet.com/) (supports a variety of flavors to choose from)
*   [Regexpal](http://regexpal.com/) (ECMAScript flavor, as implemented by JavaScript)
*   [Regexhero](http://regexhero.net/tester/) (.NET flavor)
*   [RegExr](http://gskinner.com/RegExr/) (gskinner.com – ECMAScript flavor, as implemented by Adobe Flash)
*   [reFiddle](http://refiddle.com/) (in JavaScript, à la jsFiddle)
*   [Rubular](http://rubular.com/) (Ruby flavor)
*   [myregexp.com](http://myregexp.com/) (Java-applet with source code)
*   [regexe.com](http://www.regexe.com/) (German; probably Java flavor)
*   [regex101](http://regex101.com/) (in JavaScript, Python, PCRE-compatible, generates explanation of pattern)
*   [regexper.com](http://regexper.com/) (generates graphical representation for ECMAScript flavor)
*   [debuggex](http://debuggex.com/) (generates graphical representation and shows processing of pattern – JavaScript, Python, and PCRE-compatible)

### Other links

*   [pcre](http://stackoverflow.com/questions/tagged/pcre "show questions tagged 'pcre'") – [Perl Compatible Regular Expressions (PCRE)](http://pcre.org/) is a commonly used open source C library inspired by Perl's regular expressions.
*   [Regular Expression Library](http://regexlib.com/) – a searchable library of pre-made regular expressions. If you need to write a commonly-needed regex, searching this library might be more efficient than asking a question here.

Code Language (used for [syntax highlighting](http://google-code-prettify.googlecode.com/svn/trunk/README.html)): default

  default