# HTTP - Hypertext Transfer Protocol

HTTP is a protocol which allows for communication between servers and clients. The message sent by the client, usually a web browser, is the **request**, and the message sent in return by the server is the **response**.

HTTP was developed in the early 1990s and designed to be extensible. Initially used to fetch HTML, it was extended to allow it to fetch other content, such as images and videos, and also to send content to the server.

## HTTP is stateless

Every request is completely independent. The server does not keep any data (or state) between two requests. Other methods, such as localStorage, cookies and sessions are needed for that.

## HTTPS - Hypertext Transfer Protocol Secure

HTTPS is an extension of HTTP which encrypts the data being sent using either TLS (Transport Layer Security) or SSL (Secure Sockets Layer).

The broswer knows to use the encryption due to the presence of a certificate on the web host.

## HTTP Methods

HTTP methods indicate the action you want to perform on the resource you've identified.

The most common methods are:

- GET - Retrieves data from the server
- POST - Submits data to the server
- PUT - Updates data already on the server
- DELETE - Deletes data from the server

## HTTP Header Fields

HTTP message headers are used to describe the resource being accessed, the behaviour of the server, or the behaviour of the client.

| General         | Response       | Request        |
| --------------- | -------------- | -------------- |
| Request URL     | Server         | Cookies        |
| Request Method  | Set-Cookie     | Accept-xxx     |
| Status Code     | Content-Type   | Content-Type   |
| Remote Address  | Content-Length | Content-Length |
| Referrer Policy | Date           | Authorization  |
|                 |                | User-Agent     |
|                 |                | Referrer       |

## HTTP Status Codes

- 1xx - Informational: Request received/processing
- 2xx - Success: Request successfully received, understood and accepted
- 3xx - Redirect: Further action must be taken
- 4xx - Client Error: Request does not have what it needs from the client
- 5xx - Server Error: Server failed to fulfil an apparently valid request

### Common Status Codes

- 200 - Ok
- 201 - Ok, something was created
- 301 - Moved to new URL
- 304 - Not modified (cached version)
- 400 - Bad request
- 401 - Unauthorized
- 404 - Not found
- 500 - Internal server error

## HTTP/2

HTTP/2 is a major revision of HTTP, implemented in major browsers since 2015.

HTTP/2 left most of HTTP/1.1's syntax the same but changed how data was framed and transported between the client and the server.

HTTP/2 redueced latency by enabling full request and response multiplexing (combining multiple requests/responses into one).
