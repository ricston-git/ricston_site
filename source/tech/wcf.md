## About wcf

Windows Communication Foundation is a part of the .NET Framework that provides a unified programming model for rapidly building service-oriented applications.

According to the Microsoft [Developer Center](http://msdn.microsoft.com/wcf):

> Windows Communication Foundation (WCF) is a part of the .NET Framework that provides a unified programming model for rapidly building service-oriented applications that communicate across the web and the enterprise.

## WCF Resources

*   The [WCF Developer Center](http://msdn.microsoft.com/wcf)
*   [Beginner's Guide to Windows Communication Foundation](http://msdn.microsoft.com/en-us/netframework/first-steps-with-wcf.aspx)
*   [Resources and Community](http://msdn.microsoft.com/en-us/netframework/dd939788.aspx)
*   [Introducing Windows Communication Foundation in .NET Framework 4](http://msdn.microsoft.com/library/ee958158.aspx)
*   [A Developer's Introduction to Windows Communication Foundation 4 (Aaron Skonnard)](http://msdn.microsoft.com/en-us/library/ee354381.aspx)
*   [WCF Client Overview](http://msdn.microsoft.com/en-us/library/ms735103.aspx)
*   [WCF Tracing](http://msdn.microsoft.com/en-us/library/ms730342.aspx)
*   [Configuring WCF Services in Code](http://msdn.microsoft.com/en-us/library/hh205277.aspx)

WCF is a tool often used to implement and deploy a service-oriented architecture (SOA). It is designed using service-oriented architecture principles to support distributed computing where services have remote consumers. Clients can consume multiple services; services can be consumed by multiple clients. Services are loosely coupled to each other. Services typically have a WSDL interface (Web Services Description Language) that any WCF client can use to consume the service, regardless of which platform the service is hosted on. WCF implements many advanced Web services (WS) standards such as WS-Addressing, WS-ReliableMessaging and WS-Security. With the release of .NET Framework 4.0, WCF also provides RSS Syndication Services, WS-Discovery, routing and better support for REST services.

## WCF Features

*   Create and consume traditional SOAP-based web services
*   Create and consume services that use the international WS-* standards
*   Create and consume services using other transports:
    *   TCP/IP with binary instead of text-based XML
    *   Named Pipes
    *   Microsoft Message Queue (MSMQ)
*   Host a WCF Service in any application, not just in IIS
*   Host a service in IIS with any transport, not just HTTP/HTTPS
*   Create services based on Windows Workflow Foundation workflows

## Important WCF Questions on Stack Overflow

*   [Web Services — WCF vs. Standard](http://stackoverflow.com/questions/6666/web-services-wcf-vs-standard)
*   [Can a service have multiple endpoints?](http://stackoverflow.com/questions/46283/can-a-service-have-multiple-endpoints)
*   [How many ServiceContracts can a WCF service have?](http://stackoverflow.com/questions/31790/how-many-servicecontracts-can-a-wcf-service-have)
*   [Closing and Disposing a WCF Service](http://stackoverflow.com/questions/23867/closing-and-disposing-a-wcf-service)
*   [WCF - Faults / Exceptions versus Messages](http://stackoverflow.com/questions/81306/wcf-faults-exceptions-versus-messages)
*   [What is WCF in simple terms?](http://stackoverflow.com/questions/42740/what-is-wcf)
*   [Why is WCF so important and in what cases is it used?](http://stackoverflow.com/questions/611183/why-is-wcf-so-important-and-in-what-cases-is-it-used)

Code Language (used for [syntax highlighting](http://google-code-prettify.googlecode.com/svn/trunk/README.html)): default

  default