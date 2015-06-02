## About bash

The Bourne-again shell (Bash) is a Bourne shell (sh) implementation with numerous additions. Bash is the default shell in many Linux distributions and on Mac OS X. It is available on most modern operating systems, and has been ported to Windows.

# About Bash

There are a variety of interpreters that receive commands either interactively or as a sequence of commands from a file. The [Bourne-again shell](http://en.wikipedia.org/wiki/Bash_%28Unix_shell%29) (Bash) is one such interpreter. Bash implements the standard [Bourne Shell](http://en.wikipedia.org/wiki/Bourne_shell) (sh), and offers numerous additions.

From the Free Software Foundation's [Bash page](http://www.gnu.org/software/bash/):

> Bash is an sh-compatible shell that incorporates useful features from the KornShell (ksh) and C shell (csh). It is intended to conform to the IEEE POSIX P1003.2/ISO 9945.2 Shell and Tools standard. It offers functional improvements over sh for both programming and interactive use. In addition, most sh scripts can be run by Bash without modification.

Read the [Bash manual](http://www.gnu.org/software/bash/manual/) for technical details.

# Before asking about problematic code

To help the kind people who assist you, to ensure that future readers can benefit from your question, and to help ensure your question is voted up as useful for that lovely karma, please make your question as simple and universal as possible:

1.  **Check whether your script or data has DOS style end-of-line characters**

    *   Use `cat -v yourfile` or `echo "$yourvariable" | cat -v` .

        DOS carriage returns will show up as `^M` after each line.

        If you find them, delete them using `dos2unix` (a.k.a. `fromdos`) or `tr -d '\r'`

2.  **Make sure you run the script with `bash`, not `sh`**

    *   The first line in the script must be `#!/bin/bash` or `#!/usr/bin/env bash`.

        It **must not** be `#!/bin/sh`

    *   Run the script with `./yourscript` or `bash yourscript`.

        **Do not** run it with `sh yourscript`.

    This applies even when `sh` is a symlink to `bash`.

3.  **Find a [small, self-contained example](http://www.sscce.org/).**

    *   Don't include sections and commands unrelated to your problem.
    *   Avoid complex commands that just serve to produce a value (include the value directly).
    *   Avoid relying on external files. Create the files on the fly, include the data directly, or post a small example of a file in your question.
4.  **Test your example.** Make sure it runs and still shows the problem. _Do not brush this off_.

    *   Reformatting for clarity often sidesteps pitfalls related to spacing and naming.
    *   Refactoring for simplicity often sidesteps pitfalls related to subshells.
    *   Mocking out files and data often sidesteps problems related to special characters.
    *   Hours spent trying multiple things often leads to posting code from one version and errors from another.
5.  **Check the example for common problems**

    *   Run your example through [shellcheck](http://www.shellcheck.net) to automatically check for common mistakes.
    *   Browse [Bash pitfalls](http://mywiki.wooledge.org/BashPitfalls) and [Bash beginner's mistakes](http://wiki.bash-hackers.org/scripting/newbie_traps) for checklists of common issues.
    *   Check your data for special characters, using `cat -v yourfile` or `cat -v <<< "$yourvar"`. Be especially careful with carriage returns (shown as `^M`).
6.  **Please avoid tagging questions that are solely about external commands.** The `bash` tag should be reserved for Bash-related problems, not any CLI problem you might have.

# How to turn a bad script into a good question

For example, let's say you have a script for alerting you when a server is idle, but it keeps alerting even when the machine is not idle:

    # Avoid code like this when asking about a problem
    # It has irrelevant code and external dependencies, and is hard to read and run

    while true
    do
      load=$(wget -O - "http://$1/load.php" | grep "^load:" | cut -d: -f 2)
      if [[ $load=="0" ]]
      then 
        mailx -s "System is idle" user@example.com <<< "The server is idle"
        break
      else
        echo "Waiting..."
        sleep 60
      fi
    done

1.  The problem still occurs without the loop: Remove the loop from your question.
2.  The problem still occurs if you skip asking the server: Hard code the response (e.g. `load=42`)
3.  The problem still occurs without emailing: Use `echo "Why does this run?"`
4.  The problem still occurs when removing the else branch. Shorten it

We're now left with this **small, self-contained example**:

    # Prefer code like this when asking about a problem
    # It's small, simple and self contained, making it easy to read and run.

    load=42
    if [[ $load=="0" ]]
    then
      echo "Why does this run?"
    fi

**Thanks for making your question simple and useful! Enjoy your upvotes!**

(However, note that this example is simple to compare against the relevant entry in [Bash pitfalls](http://mywiki.wooledge.org/BashPitfalls#pf10) and the error is automatically caught by [shellcheck](http://www.shellcheck.net), so now you don't actually need to ask!)

# Popular Questions

Some frequently asked Bash questions include:

*   [In the shell, what is " 2>&1 "?](http://stackoverflow.com/questions/818255/in-the-bash-shell-what-is-21)
*   [How to debug a bash script?](http://stackoverflow.com/questions/951336/how-to-debug-a-bash-script)
*   [How do I iterate over a range of numbers defined by variables in bash?](http://stackoverflow.com/questions/169511/how-do-i-iterate-over-a-range-of-numbers-defined-by-variables-in-bash)
*   [Can a Bash script tell what directory it's stored in?](http://stackoverflow.com/questions/59895/can-a-bash-script-tell-what-directory-its-stored-in)
*   [How do I tell if a regular file does not exist in bash?](http://stackoverflow.com/questions/638975/how-do-i-tell-if-a-file-does-not-exist-in-bash)
*   [How can I concatenate string variables in Bash?](http://stackoverflow.com/questions/4181703/how-can-i-concatenate-string-variables-in-bash)
*   [Check if a directory exists in a shell script](http://stackoverflow.com/questions/59838/how-to-check-if-a-directory-exists-in-a-bash-shell-script)
*   [Extract filename and extension in Bash](http://stackoverflow.com/questions/965053/extract-filename-and-extension-in-bash)
*   [Why does /bin/sh behave differently to /bin/bash even if one points to the other?](http://stackoverflow.com/questions/26717870/why-does-bin-sh-behave-differently-to-bin-bash-even-if-one-points-to-the-other)
*   [I just assigned a variable, but echo $variable shows something else](http://stackoverflow.com/questions/29378566/i-just-assigned-a-variable-but-echo-variable-shows-something-else)

# Books and Resources

Additional reading materials include:

*   [Bash manual](http://www.gnu.org/software/bash/manual/)
*   [Bash FAQ](http://tiswww.case.edu/php/chet/bash/FAQ) by the current primary maintainer, [Chet Ramey](http://tiswww.case.edu/php/chet/).
*   [Bash FAQ](http://mywiki.wooledge.org/BashFAQ) by Lhunath
*   [Bash pitfalls](http://mywiki.wooledge.org/BashPitfalls)
*   [Bash beginner's mistakes](http://wiki.bash-hackers.org/scripting/newbie_traps)
*   [Bash hackers](http://wiki.bash-hackers.org/doku.php)
*   [Bash Guide](http://mywiki.wooledge.org/BashGuide) by Lhunath
*   [Advanced Bash-Scripting Guide](http://tldp.org/LDP/abs/html/)
*   [Bash Guide for Beginners](http://www.tldp.org/LDP/Bash-Beginners-Guide/html/) by Machtelt Garrels
*   [The Command Line Crash Course](http://learncodethehardway.org/cli/book/) (also a Powershell reference)

Tools:

*   [ShellCheck](http://www.shellcheck.net), an online/offline static analysis tool that detects common mistakes

Code Language (used for [syntax highlighting](http://google-code-prettify.googlecode.com/svn/trunk/README.html)): lang-sh

  lang-sh