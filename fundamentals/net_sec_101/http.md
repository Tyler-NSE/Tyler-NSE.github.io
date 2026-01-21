---
layout: default
---

# HTTP

***

- [What is HTTP](#what-is-http)
- [What is HTTPS](#what-is-https)
- [Understanding URLs](#understanding-urls)
- [HTTP Requests](#http-requests)
- [HTTP Responses](#http-responses)
- [HTTP Methods](#http-methods)
- [HTTP Status Codes](#http-status-codes)
- [HTTP Headers](#http-headers)
- [Common Request Headers](#common-request-headers)
- [Common Response Headers](#common-response-headers)
- [Cookies](#cookies)


## What is HTTP

The Hypertext Transfer Protocol (HTTP) is used to load webpages using hypertext links. HTTP is an application layer protocol designed to transfer information between networked devices and runs on top of other layers of the network protocol stack. HTTP usually involves a client machine making a request to a server, which then sends a response message.

## What is HTTPS

HTTPS, or HyperText Transfer Protocol Secure, is HTTP with an added layer of security. Data is encrypted using Transport Layer Security (TLS) or its predecessor, Secure Sockets Layer (SSL), which ensures that the information exchanged between the client and server is private and tamper-proof. It also verifies the authenticity of the server, protecting users from man-in-the-middle attacks.

## Understanding URLs

A Uniform Resource Locator (URL) is the address used to locate a resource on the internet.

![Branching](https://tyler-nse.github.io/assets/img/net_sec_101/url.png)

*   Scheme: Specifies the protocol.
*   User: Optional credentials for authentication.
*   Host: The domain name or IP address of the server.
*   Port: The network port for the connection.
*   Path: The specific resource or file location on the server.
*   Query String: Additional parameters sent to the server.
*   Fragment: A reference to a specific section of the page.

## HTTP Requests

An HTTP request is the way Internet communications platforms such as web browsers ask for the information they need to load a website. A HTTP Request usually contains:

*   HTTP version type
*   a URL
*   a HTTP method
*   HTTP request headers
*   Optional HTTP body.

For example:

```
GET / HTTP/1.1
Host: tryhackme.com
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:87.0) Firefox/87.0
Referer: https://tryhackme.com/
```

## HTTP Responses

An HTTP response is the message that a server sends back to a client in response to an HTTP request. It usually consists of a status line, headers, and a message body:

```
HTTP/1.1 200 OK
Server: nginx/1.15.8
Date: Fri, 09 Apr 2021 13:34:03 GMT
Content-Type: text/html
Content-Length: 98

<html>
<head>
    <title>TryHackMe</title>
</head>
<body>
    Welcome To TryHackMe.com
</body>
</html>
```

## HTTP Methods

The request method tells the server what kind of action the client wants the server to take. The most common methods are:

*  HEAD:	Asks the server for status (size, availability) of a resource.
*  GET:	Asks the server to retrieve a resource.
*  POST:	Asks the server to create a new resource.
*  PUT:	Asks the server to edit/update an existing resource.
*  DELETE:	Asks the server to delete a resource.

## HTTP Status Codes

Status codes are returned in the server's response to indicate the outcome of the request.



## HTTP Headers

HTTP headers contain text information stored in key-value pairs, and they are included in every HTTP request and response. These headers communicate core information, such as what browser the client is using and what data is being requested.

## Common Request Headers

*  Host: Specifies the domain (e.g., tryhackme.com) to distinguish between multiple sites on the same server.
*  User-Agent: Identifies the client software and version for compatibility.
*  Content-Length: Indicates the size of the request body (e.g., form data).
*  Accept-Encoding: Lists compression methods the client supports (e.g., gzip, deflate).
*  Cookie: Sends stored cookie data to the server.

## Common Response Headers

*  Set-Cookie: Instructs the client to store cookie data.
*  Cache-Control: Specifies how long to cache the response.
*  Content-Type: Defines the type of data being returned (e.g., text/html, image/png).
*  Content-Encoding: Indicates the compression method used (e.g., gzip).

## Cookies

Cookies are small pieces of data stored on the client’s device by the browser, typically set via the Set-Cookie response header. They allow websites to maintain state across requests, as HTTP is stateless. Cookies are often used for:

*  Authentication: Storing session tokens to keep users logged in.
*  Personalization: Saving user preferences or settings.
*  Tracking: Monitoring user behavior across sessions.

[back](/fundamentals/networks_and_security.html)