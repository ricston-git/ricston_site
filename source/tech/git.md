## About git

Git is an open-source distributed version control system (DVCS).

[Git](http://git-scm.com/) is an open-source [distributed version control system](http://stackoverflow.com/tags/dvcs/info) (DVCS) with an emphasis on speed. [git](http://stackoverflow.com/questions/tagged/git "show questions tagged 'git'") was initially designed and developed by [Linus Torvalds](http://en.wikipedia.org/wiki/Linus_Torvalds) for [linux](http://stackoverflow.com/questions/tagged/linux "show questions tagged 'linux'") kernel development, now it is maintained by [Junio Hamano](http://git-blame.blogspot.com/). Every Git working directory contains a full-fledged repository with complete history and full revision tracking capabilities, not dependent on network access or a central server.

There are many resources and tutorials available free online for Git beginners; see the bottom of this page for links to some of these resources.

# Characteristics

*   Strong support for non-linear development
*   Distributed development
*   Compatibility with existing systems/protocols
*   Efficient handling of large projects
*   Cryptographic authentication of history
*   Toolkit-based design
*   Pluggable merge strategies
*   Garbage accumulates unless collected
*   Periodic explicit object packing

# Data structures

![git - data workflow](http://i.stack.imgur.com/GEGy5.png)

# External Links

*   [Pro Git by Scott Chacon](http://git-scm.com/book) (free)
    *   Recommended chapters for beginners: 1-3, 6-6.5.
*   [Git Pocket Guide](http://chimera.labs.oreilly.com/books/1230000000561/index.html) (free)
*   [Official Git Tutorial](http://git-scm.com/docs/gittutorial)
*   [Official Git Wiki](https://git.wiki.kernel.org/)
*   **[Jan Krüger's mirror of the official Git documentation](http://jk.gs/git.html).**
    *   This is currently **the most complete, comprehensive, and up-to-date** online version of the Git documentation.
*   [Git Reference](http://gitref.org/)
*   **[Git Documentation Source Code](https://github.com/git/git/tree/v2.0.1/Documentation)**
    *   This is guaranteed to be up-to-date, and have the most readable formatting.
    *   You can also view these docs using `man git`, `git <command> --help`, or `git help <command>`.
*   [Official Git user manual](https://www.kernel.org/pub/software/scm/git/docs/user-manual.html) (may be outdated)
*   [Git-SCM documentation](http://git-scm.com/documentation)
    *   A simplified, but more up-to-date, copy of [the official reference](https://www.kernel.org/pub/software/scm/git/docs/). Not all documentation is entirely and properly rendered, however.
*   [Git source code](http://git.kernel.org/?p=git/git.git;a=summary)
*   [Git source code mirror on GitHub](https://github.com/git/git)
*   [Git Wikipedia Article](http://en.wikipedia.org/wiki/Git_(software))
*   [A Visual Git Reference](http://marklodato.github.io/visual-git-guide/index-en.html)
*   [Git-SCM Blog](http://git-scm.com/blog)
*   [Atlassian Git Tutorials and Traning](https://www.atlassian.com/git/tutorial)
*   [Git for Computer Scientists](http://eagain.net/articles/git-for-computer-scientists/)

# Internal Links

## Installation/Setup

*   [How to install Git](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide#323764)
*   How do you set up Git? Try to cover Linux, Windows, Mac, think 'client/server' mindset.
*   [Setup GIT Server with Msysgit on Windows](http://stackoverflow.com/questions/1482824/setup-git-server-with-msysgit-on-windows)
*   [How do you create a new project/repository?](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide#320140)
*   [How do you configure it to ignore files (.obj, .user, etc) that are not really part of the codebase?](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide#316062)

## Working with the code

*   [How do you get the latest code?](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide/1350157#1350157)
*   [How do you check out code?](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide#323906)
*   [How do you commit changes?](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide#316055)
*   [How do you see what's uncommitted, or the status of your current codebase?](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide#319465)
*   [How do you destroy unwanted commits?](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide#323898)
*   [How do you compare two revisions of a file, or your current file and a previous revision?](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide/1762631#1762631)
*   [How do you see the history of revisions to a file?](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide/2114836#2114836)
*   [How do you undo (revert or reset) a commit?](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide/323898#323898)

## Tagging, branching, releases, baselines

*   [How do you 'mark' 'tag' or 'release' a particular set of revisions for a particular set of files so you can always pull that one later?](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide#322967)
*   [How do you branch?](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide/816614#816614)
*   [How do you merge branches?](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide/816636#816636)
*   [What is rebasing?](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide/5985070#5985070)
*   [How do I track remote branches?](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide/1590791#1590791)
*   [How can I create a branch on a remote repository?](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide/1590803#1590803)
*   [How do I delete a branch on a remote repository?](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide/5977604#5977604)
*   [Git workflow examples](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide/5968622#5968622)

## Git Clients

*   [msysgit](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide#323559) - Cross platform, included with Git
*   [gitk](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide#323559) - Cross platform history viewer, included with Git
*   [gitnub](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide#323559) - Mac OS X
*   [gitx](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide#323559) - Mac OS X history viewer
*   [smartgit](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide#323559) - Cross platform, commercial, beta
*   [tig](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide/322989#322989) - console GUI for Linux
*   [qgit](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide/644129#644129) - GUI for Windows, Linux
*   [Git Extensions](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide#323559) - package for Windows, includes friendly GUI
*   [SourceTree](http://www.sourcetreeapp.com/) - A free Git & Mercurial client for Windows or Mac
*   [posh-git](http://dahlbyk.github.io/posh-git/) - A Windows PowerShell environment for Git

## Clients that are primarily used for GitHub but also support Git

*   [GitHub Windows](https://windows.github.com)
*   [GitHub Mac](https://mac.github.com)
*   [GitHub Eclipse](https://eclipse.github.com)

### Any other common tasks a beginner should know?

*   [Git Status tells you what you just did, what branch you have, and other useful information](http://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide/319465#319465)

## Other Git beginner's references

*   [Git guide](http://wiki.sourcemage.org/Git_Guide)
*   [Pro Git - book by Scott Chacon](http://git-scm.com/book)
*   [Git magic](http://www-cs-students.stanford.edu/~blynn/gitmagic/)
*   [GitHub video guides](http://www.youtube.com/playlist?list=PLg7s6cbtAD15HBa4C41jhT9YQs5bZumTE)
*   [GitHub guides](http://help.github.com/)
*   [Git - SVN Crash Course](http://git.or.cz/course/svn.html "Git - SVN Crash Course")
*   [Git from the bottom up](http://www.newartisans.com/2008/04/git-from-the-bottom-up/)
*   [Git ready](http://www.gitready.com/)
*   [Git visual cheatsheet](http://www.ndpsoftware.com/git-cheatsheet.html)
*   [Githug](https://github.com/Gazler/githug)
*   [tryGit](http://try.github.com/)
*   [A Visual Git Reference](http://marklodato.github.com/visual-git-guide/index-en.html)
*   [Think Like (a) Git](http://think-like-a-git.net/)
*   [Atlassian Git Tutorials and Traning](https://www.atlassian.com/git/tutorial)
*   [Git for the Lazy](http://wiki.spheredev.org/Git_for_the_lazy)
*   [Learn Git Branch - Interactive Tutorial](http://pcottle.github.io/learnGitBranching/)

There are also good guides if you would like to [understand Git conceptually](http://www.eecs.harvard.edu/~cduan/technical/git/) or if you would like to [compare other revision control software](http://en.wikipedia.org/wiki/Comparison_of_revision_control_software) such as subversion.