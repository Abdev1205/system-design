# HTTP (Hypertext Transfer Protocol)

HTTP is an application layer protocol utilized for accessing and transferring various types of data, including text, images, videos, and multimedia, over the World Wide Web. It operates as a client-server protocol, running on top of the TCP/IP family of protocols, and follows the request/response model.

## Basic Concepts

- **Port Number**: HTTP uses port number 80 for communication.

### Communication Process

1. The client sends a request message to the server.
2. HTTP establishes a TCP connection between the client and the server.
3. The server processes the client's request and collects the requested data.
4. The server sends the data to the client.
5. The connection is terminated.

### Connection Characteristics

- **Connectionless**: After serving a single HTTP request, the client-server connection is closed and not reused.

- **Media Independent**: HTTP can send any data type as long as both the client and server understand how to process it.

- **Stateless**: The client and server only retain knowledge about each other during the current request. Once the connection is closed, both parties forget about each other.

## HTTPS (Hypertext Transfer Protocol Secure)

HTTPS is a secure extension of HTTP, designed to enhance the security of data transmitted over the World Wide Web.

### Security Features

- To encrypt communications, HTTPS employs the Transport Layer Security (TLS) protocol, formerly known as Secure Sockets Layer (SSL).

- HTTPS uses port number 443 for secure data communication.

### Importance

HTTPS is crucial for transmitting sensitive data, such as login credentials, in an encrypted form, ensuring a higher level of security.

🔒 **Security**: HTTPS provides a secure environment for data transmission.

🔑 **Encryption**: TLS encryption ensures the confidentiality and integrity of transmitted data.

🌐 **World Wide Web**: HTTP and HTTPS are fundamental protocols for accessing information on the web.

![](https://i.postimg.cc/Vvq4vtR1/image.png)