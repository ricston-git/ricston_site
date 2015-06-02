## About http

Hypertext Transfer Protocol (HTTP) is an application level network protocol that is used for the transfer of content on the World Wide Web.

[Hypertext Transfer Protocol (HTTP)](http://en.wikipedia.org/wiki/Http) uses a client-request/server-response model. HTTP is a stateless protocol, which means it does not require the server to retain information or status about each user for the duration of multiple requests.

The request is sent with an HTTP method:

*   HEAD - used to retrieve the GET response header without the actual content (or just the metadata in the content).
*   GET - used to retrieve data, the request body should be ignored.
*   POST - used to send data to the server, the body should hold the data

These are all the methods supported by older browsers, but the [HTTP 1.1 specification](http://www.w3.org/Protocols/rfc2616/rfc2616.html) includes a few more: PUT, DELETE, TRACE, OPTIONS, CONNECT and PATCH.

The response is returned with a [status code](http://www.w3.org/Protocols/rfc2616/rfc2616-sec10.html):

*   1xx are informational
*   2xx indicates success, most pages will have a 200 status
*   3xx are used for redirections
*   4xx codes are used for errors with the request, the commonest being 404 for a page not found
*   5xx are used for server errors

Both the request and response are made up of a header and an optional body.

The header contains a list of key-value pairs, separated using new lines and colons. For example, a request may have headers like this:

    Proxy-Connection: keep-alive
    Referer: url
    User-Agent: browser name or client application
    Accept-Encoding: gzip,deflate
    Accept-Language: en-GB

Note that in the example the request is telling the server that the response can be sent with the body compressed with either gzip or DEFLATE encoding.

The request needs a body if it's sending additional data to the server, for instance if sending information entered to a form.

The response headers will include information telling the client how to deal with the response data, for instance whether they can cache the data (and how long for).

The response body will have the requested data, such as the HTML of a web page or image data.

HTTP is used by browsers to retrieve web content, but can also be used for data APIs, for instance, as a [SOAP](http://stackoverflow.com/tags/soap/info) or [REST](http://stackoverflow.com/tags/rest/info) service.