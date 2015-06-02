## About list

list may refer to: a linked list (an ordered set of nodes, each referencing its successor), or a form of dynamic array. Not to be used for HTML lists, use the "html-lists" tag instead.

**Do not** use this tag for unordered/ordered lists in HTML, use [html-lists](http://stackoverflow.com/questions/tagged/html-lists "show questions tagged 'html-lists'") instead.

* * *

Nearly every programming language provides support for list data structures by incorporating logical operators bitwise operators.

A list is denoted with logical operators. The specific syntax may vary based on the language and system being used. Common operators are [semicolon](http://www.w3.org/TR/MathML2/glyphs/000/U0003B.png) (;), [ampersand](http://www.w3.org/TR/MathML2/glyphs/000/U00026.png) (&), double-ampersand (&&), or [double-vertical-line](http://www.w3.org/TR/MathML2/glyphs/020/U02016.png) (||).

* * *

# Specific Implementations**

**PHP list operator examples**

and Called Logical AND operator. If both the operands are true then then condition becomes true. (A and B) is true. or Called Logical OR Operator. If any of the two operands are non zero then then condition becomes true. (A or B) is true. && Called Logical AND operator. If both the operands are non zero then then condition becomes true. (A && B) is true. || Called Logical OR Operator. If any of the two operands are non zero then then condition becomes true. (A || B) is true. ! Called Logical NOT Operator. Use to reverses the logical state of its operand. If a condition is true then Logical NOT operator will make false. !(A && B) is false.

and denotes if both operat

    | $a and $b | And | True if both $a and $b are true
    | $a && $b  | And | True if both $a and $b are true
    | $a or $b  | Or  | True if either $a or $b is true
    | $a || $b  | Or  | True if either $a or $b is true
    | $a xor $b | Xor | True if either $a or $b is true, but not both
    | !$a       | Not | True if $a is not true

*   **And** operators denote if both operands are true then the condition is true.
*   **Or** operators denote if any of the operands are non-zero then the condition is true.
*   **Xor** operators denote if all of the operands are non zero then the condition is true.
*   **Not** operators reverse the logical state of any operand. If a condition is true then the not operator will make the condition false.

**Shell**

In Shell, list operators are limited to semicolon, ampersand, double-ampersand, and double-vertical-line. Of these list operators, && and || have equal precedence, followed by ; and &, which have equal precedence.

If a command is terminated by the control operator &, the shell executes the command in the background using a subshell. The shell does not wait for the command to finish, and the return status is 0.

Commands separated by a ; are executed sequentially; the shell waits for each command to terminate in turn. The return status is the exit status of the last command executed.

The control operators && and || denote AND lists and OR lists, respectively. An AND list has the form command1 && command2\. Command2 is executed if, and only if, command1 returns an exit status of zero.

An OR list has the form

    command1 || command2

command2 is executed if and only if command1 returns a non-zero exit status. The return status of AND and OR lists is the exit status of the last command executed in the list.

# Performance

The flexibility of linked lists is somewhat offset by the complexity of some operations on lists (accessing an element at index _n_ in the list is _O(n)_, while for arrays it is _O(1)_). In practice, linked lists are a very disadvantageous structure for random-access-based algorithms. Linked lists support quick _O(1)_ appends, dynamic arrays also support _O(1)_ appends however this _O(1)_ runtime is amortized as it must factor in the periodical re-sizing of the dynamic array. The performance of lists and arrays is of the same order (_O_) for operations that deal with every element of the list in order.

# Types

Lists are the canonical recursive (or inductive) data type.

Logical operators such as &, &&, or || are considered short circuit logical-OR operators which means that once it reaches an argument which evaluates to true then any subsequent arguments are not evaluated.

Bitwise operators such as XOR will evaluate all of the arguments supplied to determine the result.

# See also

*   [arrays](http://stackoverflow.com/questions/tagged/arrays "show questions tagged 'arrays'")
*   [linked-list](http://stackoverflow.com/questions/tagged/linked-list "show questions tagged 'linked-list'")
*   [singly-linked-list](http://stackoverflow.com/questions/tagged/singly-linked-list "show questions tagged 'singly-linked-list'")
*   [queue](http://stackoverflow.com/questions/tagged/queue "show questions tagged 'queue'")

# Links

*   [List (Wikipedia)](http://en.wikipedia.org/wiki/List_%28data_structure%29)
*   [C and C++ Operators](https://en.wikipedia.org/wiki/Operators_in_C_and_C%2B%2B)