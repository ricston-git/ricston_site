## About activemq

Apache ActiveMQ is an open source (Apache 2.0 licensed) message broker which fully implements the Java Message Service 1.1 (JMS). It provides "Enterprise Features" like clustering, multiple message stores, and ability to use any database as a JMS persistence provider besides VM, cache, and journal persistency.

Apache **ActiveMQ** is an open source (Apache 2.0 licensed) message broker which fully implements the Java Message Service 1.1 (JMS). It provides [**Enterprise Features**](http://activemq.apache.org/getting-started.html) like clustering, multiple message stores, and ability to use any database as a JMS persistence provider besides VM, cache, and journal persistency.

Apart from Java, ActiveMQ can also be used from .NET, C/C++ or Delphi or from scripting languages like Perl, Python, PHP and Ruby via various "Cross Language Clients" together with connecting to many protocols and platforms. These include several standard wire-level protocols, plus their own protocol called OpenWire.

ActiveMQ is used in enterprise service bus implementations such as Apache ServiceMix, Apache Camel, and Mule.

ActiveMQ is often used with Apache ServiceMix, Apache Camel and Apache CXF in SOA infrastructure projects.

> Coinciding with the release of Apache ActiveMQ 5.3, the world's first results for the SPECjms2007 industry standard benchmark were announced. Four results were submitted to the SPEC and accepted for publication. The results cover different topologies to analyze the scalability of Apache ActiveMQ in two dimensions. <sub>Quoted from: [http://en.wikipedia.org/wiki/Apache_ActiveMQ](http://en.wikipedia.org/wiki/Apache_ActiveMQ)</sub>

**Features:**

*   Supports a variety of Cross Language Clients and Protocols from Java, C, C++, C#, Ruby, Perl, Python, PHP
    *   OpenWire for high performance clients in Java, C, C++, C#
    *   Stomp support so that clients can be written easily in C, Ruby, Perl, Python, PHP, ActionScript/Flash, Smalltalk to talk to ActiveMQ as well as any other popular Message Broker
*   Full support for the [Enterprise Integration Patterns](http://www.enterpriseintegrationpatterns.com/) both in the JMS client and the Message Broker
*   Supports many advanced features such as Message Groups, Virtual Destinations, Wildcards and Composite Destinations
*   Fully supports JMS 1.1 and J2EE 1.4 with support for transient, persistent, transactional and XA messaging
*   Spring Support so that ActiveMQ can be easily embedded into Spring applications and configured using Spring's XML configuration mechanism
*   Tested inside popular J2EE servers such as TomEE, Geronimo, JBoss, GlassFish and WebLogic
    *   Includes JCA 1.5 resource adaptors for inbound & outbound messaging so that ActiveMQ should auto-deploy in any J2EE 1.4 compliant server
*   Supports pluggable transport protocols such as in-VM, TCP, SSL, NIO, UDP, multicast, JGroups and JXTA transports
*   Supports very fast persistence using JDBC along with a high performance journal
*   Designed for high performance clustering, client-server, peer based communication
*   REST API to provide technology agnostic and language neutral web based API to messaging
*   Ajax to support web streaming support to web browsers using pure DHTML, allowing web browsers to be part of the messaging fabric
*   CXF and Axis Support so that ActiveMQ can be easily dropped into either of these web service stacks to provide reliable messaging
*   Can be used as an in memory JMS provider, ideal for unit testing JMS

**Supported Languages:** [java](http://stackoverflow.com/questions/tagged/java "show questions tagged 'java'"), [c](http://stackoverflow.com/questions/tagged/c "show questions tagged 'c'"), [c++](http://stackoverflow.com/questions/tagged/c%2b%2b "show questions tagged 'c++'"), [c#](http://stackoverflow.com/questions/tagged/c%23 "show questions tagged 'c#'"), [ruby](http://stackoverflow.com/questions/tagged/ruby "show questions tagged 'ruby'"), [perl](http://stackoverflow.com/questions/tagged/perl "show questions tagged 'perl'"), [python](http://stackoverflow.com/questions/tagged/python "show questions tagged 'python'"), [php](http://stackoverflow.com/questions/tagged/php "show questions tagged 'php'"), [javascript](http://stackoverflow.com/questions/tagged/javascript "show questions tagged 'javascript'"), [erlang](http://stackoverflow.com/questions/tagged/erlang "show questions tagged 'erlang'"), [actionscript](http://stackoverflow.com/questions/tagged/actionscript "show questions tagged 'actionscript'"), [perl](http://stackoverflow.com/questions/tagged/perl "show questions tagged 'perl'"), [ruby](http://stackoverflow.com/questions/tagged/ruby "show questions tagged 'ruby'")

**Supported Protocols:** [openwire](http://stackoverflow.com/questions/tagged/openwire "show questions tagged 'openwire'"), [rest](http://stackoverflow.com/questions/tagged/rest "show questions tagged 'rest'"), [stomp](http://stackoverflow.com/questions/tagged/stomp "show questions tagged 'stomp'"), [xmpp](http://stackoverflow.com/questions/tagged/xmpp "show questions tagged 'xmpp'"), [amqp](http://stackoverflow.com/questions/tagged/amqp "show questions tagged 'amqp'"), [mqtt](http://stackoverflow.com/questions/tagged/mqtt "show questions tagged 'mqtt'")

**Official Website:** [http://activemq.apache.org/](http://activemq.apache.org/)

**Useful Links:**

*   [Getting Started](http://activemq.apache.org/getting-started.html)
*   [FAQ](http://activemq.apache.org/faq.html)
*   [Articles](http://activemq.apache.org/articles.html)
*   [Books](http://activemq.apache.org/books.html)