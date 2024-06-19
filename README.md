<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents** 

- [STATUS CODES](#status-codes)
  - [1xx : Informational](#1xx--informational)
  - [2xx : Success](#2xx--success)
  - [3xx : Redirection](#3xx--redirection)
  - [4xx : Client Errors](#4xx--client-errors)
  - [5xx : Server Errors](#5xx--server-errors)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->


# STATUS CODES

Status codes are standardized codes that are used by web servers to communicate the outcome of a client's request to the server. They are an essential part of the HTTP protocol and help both clients and servers understand the result of a request. Here is an overview of the various classes of HTTP status codes:

## 1xx : Informational
These codes indicate that the request was received and understood, and the server is continuing the process.

**100 Continue:**
The initial part of a request has been received and the client should continue.

**101 Switching Protocols:**
 The server is switching protocols as requested by the client.

**102 Processing:**
The server has received and is processing the request, but no response is available yet.

**103 Early Hints:**
This status code is primarily intended to be used with the Link header, letting the user agent start preloading resources while the server prepares a response or preconnect to an origin from which the page will need resources.


 ## 2xx : Success
These codes indicate that the request was successfully received, understood, and accepted.

**200 OK:** 
The request has succeeded.

**201 Created:** The request has been fulfilled and a new resource has been created.

**202 Accepted:** The request has been accepted for processing, but the processing is not complete.

**203 Non-Authoritative Information:** The request was successful but the information may be from another source.

**204 No Content:** The server successfully processed the request, but is not returning any content.

**205 Reset Content:** The server successfully processed the request, but is not returning any content and requires the requester to reset the document view.

**206 Partial Content:** The server is delivering only part of the resource due to a range header sent by the client.


## 3xx : Redirection
These codes indicate that further action needs to be taken by the user agent to fulfill the request.

**300 Multiple Choices:** There are multiple options that the client can follow.

**301 Moved Permanently:** The resource has been moved to a new URL permanently.

**302 Found:** The resource is temporarily under a different URL.

**303 See Other:** The response can be found under a different URL and should be retrieved using a GET method.

**304 Not Modified:** The resource has not been modified since the version specified by the request headers.

**305 Use Proxy:** The requested resource is available only through a proxy.

**307 Temporary Redirect:** The resource is temporarily under a different URL and the same method should be used.

**308 Permanent Redirect:** The resource is permanently under a different URL and the same method should be used.

## 4xx : Client Errors
These codes indicate that the client made an error in the request.

**400 Bad Request:** The server could not understand the request due to invalid syntax.

**401 Unauthorized:** The client must authenticate itself to get the requested response.

**402 Payment Required:** This code is reserved for future use.

**403 Forbidden:** The client does not have access rights to the content.

**404 Not Found:** The server cannot find the requested resource.

**405 Method Not Allowed:** The method specified in the request is not allowed for the resource.

**406 Not Acceptable:** The requested resource is capable of generating only content not acceptable according to the Accept headers.

**407 Proxy Authentication Required:** The client must authenticate with the proxy.

**408 Request Timeout:** The server timed out waiting for the request.

**409 Conflict:** The request could not be processed because of a conflict.

**410 Gone:** The resource is no longer available and will not be available again.

**411 Length Required:** The request did not specify the length of its content, which is required by the resource.

**412 Precondition Failed:** The server does not meet one of the preconditions that the requester put on the request.

**413 Payload Too Large:** The request is larger than the server is willing or able to process.

**414 URI Too Long:** The URI provided was too long for the server to process.

**415 Unsupported Media Type:** The media format of the requested data is not supported by the server.

**416 Range Not Satisfiable:** The range specified by the Range header field in the request cannot be fulfilled.

**417 Expectation Failed:** The expectation given in the request's Expect header could not be met.

**418 I'm a teapot:** This code was defined in 1998 as one of the traditional IETF April Fools' jokes, but is not expected to be implemented by actual HTTP servers.

**421 Misdirected Request:** The request was directed at a server that is not able to produce a response.

**422 Unprocessable Entity:** The request was well-formed but was unable to be followed due to semantic errors.

**423 Locked:** The resource that is being accessed is locked.

**424 Failed Dependency:** The request failed due to failure of a previous request.

**426 Upgrade Required:** The client should switch to a different protocol.

**428 Precondition Required:** The server requires the request to be conditional.

**429 Too Many Requests:** The user has sent too many requests in a given amount of time.

**431 Request Header Fields Too Large:** The server is unwilling to process the request because its header fields are too large.

**451 Unavailable For Legal Reasons:** The user-requested resource is unavailable due to legal reasons.

## 5xx : Server Errors
These codes indicate that the server failed to fulfill a valid request.

**500 Internal Server Error:** The server has encountered a situation it doesn't know how to handle.

**501 Not Implemented:** The request method is not supported by the server and cannot be handled.

**502 Bad Gateway:** The server, while working as a gateway to get a response needed to handle the request, got an invalid response.

**503 Service Unavailable:** The server is not ready to handle the request.

**504 Gateway Timeout:** The server is acting as a gateway and cannot get a response in time.

**505 HTTP Version Not Supported:** The HTTP version used in the request is not supported by the server.

**506 Variant Also Negotiates:** Transparent content negotiation for the request results in a circular reference.

**507 Insufficient Storage:** The server is unable to store the representation needed to complete the request.

**508 Loop Detected:** The server detected an infinite loop while processing the request.

**510 Not Extended:** Further extensions to the request are required for the server to fulfill it.

**511 Network Authentication Required:** The client needs to authenticate to gain network access.