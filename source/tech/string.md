## About string

A string is a finite sequence of symbols, commonly used for text, though sometimes for arbitrary data.

A string is a finite sequence of symbols, commonly used for text, though sometimes for arbitrary data.

Most programming languages provide a dedicated string data type or more general facilities and conventions for handling strings; as well as providing a way to denote string literals. In some programming languages [everything is a string](http://wiki.tcl.tk/3018), for example in Tcl. A dedicated support library of differing sophistication is mostly provided as well.

String representations vary widely in the features they offer; the right string type can easily decrease the order of algorithms, while the wrong one might not even be able to accommodate your string data at all.

The following are some hand-picked representatives:

*   Zero-terminated Strings (aka. C-strings, ASCIZ, sz) are arrays of non-null elements, terminated by a special, null element (variants using a different terminating symbol are mostly restricted to old systems, e.g. DOS supported `$`).
*   Counted String (aka Pascal Strings) are arrays of arbitrary bytes, prefixed by a length indicator. Nowadays, the size for counted strings is restricted by available address space, though it was quite common to use a single byte for length (implying maximum length of 255).
*   Ropes, which are lists of segments (for example length + pointers into modifiable and non-modifiable buffers), for efficient insertion and deletion.

Many (especially functional) languages support strings as a list of base symbols.

For [unicode](http://stackoverflow.com/questions/tagged/unicode "show questions tagged 'unicode'") support, a special string of the strings type is getting common, as Unicode characters can be of arbitrary length, even in [utf32](http://stackoverflow.com/questions/tagged/utf32 "show questions tagged 'utf32'"). This enables efficient character-indexing by pushing the complexities of the character set into the string type.

In most languages, strings can be iterated over, similar to lists/arrays. In some high-level languages (in which strings are a data type unto themselves), strings are immutable, so string operations create new strings.

For text strings, many encodings are in used, though modern usage is converging on [unicode](http://stackoverflow.com/questions/tagged/unicode "show questions tagged 'unicode'"), using [utf-8](http://stackoverflow.com/questions/tagged/utf-8 "show questions tagged 'utf-8'") (some early adopters of Unicode instead transitioned form [ucs2](http://stackoverflow.com/questions/tagged/ucs2 "show questions tagged 'ucs2'") to [utf-16](http://stackoverflow.com/questions/tagged/utf-16 "show questions tagged 'utf-16'") as a persistence format).

Windows software often adopts the WinAPI convention of using UTF-16 internally, converting for external data and persistence instead of system calls.

When a string appears literally in source code, it is known as a string literal and has a representation that denotes it as such.

### Useful Links:

*   [Wikipedia entry on String](http://en.wikipedia.org/wiki/String_(computer_science))
*   [String Handling](http://en.wikipedia.org/wiki/C_string_handling)