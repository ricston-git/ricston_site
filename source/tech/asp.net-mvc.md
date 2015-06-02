## About asp.net-mvc

The ASP.NET MVC Framework is an open source web application framework and tooling that implements a version of the model-view-controller (MVC) pattern tailored towards web applications and built upon an ASP.NET technology foundation.

The Microsoft [ASP.NET MVC Framework](http://www.asp.net/mvc) is an [open source](http://aspnetwebstack.codeplex.com/) web application framework and tooling that implements a version of the model-view-controller (MVC) pattern tailored towards web applications.

The ASP.NET MVC framework provides an alternative to the ASP.NET WebForms Framework for creating Web applications, and is a more lightweight and testable framework than its WebForms cousin, even though they are both built upon the same base ASP.NET foundation. It uses existing ASP.NET features, and in more recent versions has become more unified with WebForms via Microsoft's "One ASP.NET" initiative. The MVC framework is defined in the `System.Web.Mvc` assembly.

ASP.NET MVC releases also tend to package additional technologies, such as the Razor View Engine, Web Optimization Framework, ASP.NET WebAPI, along with tooling such as Scaffolding, and integration into Visual Studio.

The Model-View-Controller architectural pattern, upon which ASP.NET MVC is based separates an application into three main components: the model, the view, and the controller. The reason for this separation is to provide a cleaner overall architecture, while improving maintainability. This concept is often referred to as a "Seperation of Concerns".

A model represents the state of a particular aspect of the application. Frequently, a model maps to a database table with the entries in the table representing the state of the application. A controller handles interactions and updates the model to reflect a change in state of the application, and then passes information to the view. A view accepts necessary information from the controller and renders a user interface to display that.

Since the ASP.NET MVC 4 release, Microsoft has shipped the framework both with a specific release of Visual Studio, as well as via the [Nuget](http://nuget.codeplex.com/) package management system. This package management method allows for easier "out of band" releases (versions not tied to a specific version of Visual Studio), along with a more module release so that sub-components can be chosen to be included or not (ASP.NET WebApi for example).

The latest announcements from Microsoft regarding ASP.NET MVC usually come from the [.NET Web Development and Tools Blog](http://blogs.msdn.com/b/webdev/), [Visual Studio Blog](http://blogs.msdn.com/b/visualstudio/) or [.NET Framework Blog](http://blogs.msdn.com/b/dotnet/). Other notable blogs relating to MVC are [Scott Guthrie's Blog](http://weblogs.asp.net/scottgu/), [ASP.NET by Scott Hanselman](http://hanselman.com), and [Imran Baloch's Blog](http://weblogs.asp.net/imranbaloch).

Unless you have a good reason not to, try to keep your MVC version current. There are bug fixes in newer versions, as well as new features. It makes little sense to create new projects using older versions of MVC today. The first thing you should do after creating a new project is open up the NuGet package manager and apply all updates (with the possible exception of jQuery 2.x. If you need compatibility with older browsers stay with the latest version jQuery 1.x, which is feature compatible with the 2.x line).

**Versions shipped with Visual Studio**

*   Visual Studio 2008 - None (MVC was released after 2008 was)
*   Visual Studio 2010 - ASP.NET MVC 2 (no point releases)
*   Visual Studio 2012 - ASP.NET MVC 5.0.0
*   Visual Studio 2013 - ASP.NET MVC 5.1.0
*   Visual Studio 2015 (aka "14") - ASP.NET MVC 6.x (Preview Release)

**Requirements by version**

*   MVC 1 - Visual Studio 2008 - CLR 2.0
*   MVC 2 - Visual Studio 2008 - CLR 2.0
*   MVC 3 - Visual Studio 2010 - CLR 4.0 - Framework 4.0
*   MVC 4 - Visual Studio 2010 - CLR 4.0 - Framework 4.0
*   MVC 5.x - Visual Studio 2012 - CLR 4.0 - Framework 4.5
*   MVC 6.x - Visual Studio 2015 (aka "14") - (Preview release)

**Current Releases** (Available through NuGet)

*   [Stable release 5.2.3](http://www.nuget.org/packages/Microsoft.AspNet.Mvc/5.2.3) (February 9, 2015)
*   [Beta Release 6.0.0-beta4](http://www.asp.net/vnext/overview/aspnet-vnext/overview) (April 24, 2015)

**References**

*   [ASP.NET MVC Framework](http://en.wikipedia.org/wiki/ASP.NET_MVC_Framework) Wikipedia Article
*   [ASP.NET Source Code Stack](https://aspnetwebstack.codeplex.com/) (including MVC)
*   [ASP.NET 5 Source Code](https://github.com/aspnet/home)

### Frequently Asked Questions (FAQ)

Please note that most questions that may refer to a specific version of ASP.NET MVC will likely apply to newer versions as well. So if the question says MVC3, it likely also applies to MVC4 and MVC5.x, etc.

*   [How do you handle multiple submit buttons in ASP.NET MVC Framework?](http://stackoverflow.com/questions/442704/how-do-you-handle-multiple-submit-buttons-in-asp-net-mvc-framework)
*   [How do you create a dropdownlist from an enum in ASP.NET MVC?](http://stackoverflow.com/questions/388483/how-do-you-create-a-dropdownlist-from-an-enum-in-asp-net-mvc)
*   [Cascading drop-downs in MVC 3 Razor view](http://stackoverflow.com/questions/4458970/cascading-drop-downs-in-mvc-3-razor-view)
*   [How do I bind a collection on postback?](http://stackoverflow.com/a/25365806/61164)
*   [Why does my page not render the contents of my model?](http://stackoverflow.com/questions/25792697/is-this-a-bug-in-the-mvc-framework)

### Tutorials (High quality external articles on Frequently asked topics)

*   [Getting Started with ASP.NET MVC 5](http://www.asp.net/mvc/tutorials/mvc-5/introduction/getting-started)
*   [NerdDinner Walkthrough](http://weblogs.asp.net/scottgu/archive/2009/03/10/free-asp-net-mvc-ebook-tutorial.aspx)
*   [Using simple Drop Down Lists in ASP.NET MVC](http://nimblegecko.com/using-simple-drop-down-lists-in-ASP-NET-MVC/)

Code Language (used for [syntax highlighting](http://google-code-prettify.googlecode.com/svn/trunk/README.html)): default

  default