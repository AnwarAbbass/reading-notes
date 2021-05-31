#  Socket.io
## Review, Research, and Discussion
* What is the benefit of transforming data into packets?
  * to meet the demands of pervasive data-centric applications and services.

* UDP is often refereed to as a connectionless protocol. Why is this?
  * because it is analogous to sending a letter where you don't acknowledge receipt.
  
![](https://cdn.educba.com/academy/wp-content/uploads/2019/07/User-Datagram-Protocol-3.png)

* Can a socket server application have multiple socket connections?
  * yes it can  handel 65535 socket connections.


* Can a socket connection application be connected to multiple socket servers?
  *  Yes, a socket connection application can connect to multiple socket server Theoretically but it is not practical.

* Can an application be both a socket server and a socket connection?
  *   Yes, it can be applied.



## Vocabulary Terms

### Observer Pattern :
* The observer pattern is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods. 
### Listener :
* waits for an event to occur.
### Event Handler :
* code to be executed when an event occurs.

### Event Driven Programming :
* where the execution of the code depends on events occurrence.
### Event Loop :
* way of handling the execution of the code.
### Event Queue :
* a queue of events waiting to be executed.
### Call Stack :
* rganizing the code in the order of its execution.
### Emit/Raise/Trigger :
* to fire an event.
### Subscribe :
* a function that defines how to obtain or generate values or messages to be published.
### database :
* a collection of data that enable the programmer to CRUD.


## WebSocket

![](https://miro.medium.com/max/800/1*_6Zt1h5jopuP9syi-VDoMg.jpeg)

* it is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.
* WebSocket is distinct from HTTP. Both protocols are located at layer 7 in the OSI model and depend on TCP at layer 4.
![](https://portswigger.net/web-security/images/websockets.svg)
* WebSocket remains open all the time.
*  enables interaction between a web browser (or other client application) and a web server with lower overhead than half-duplex alternatives such as HTTP polling.

![](https://www.websocket.org/img/websocket-architecture.jpg)
* by providing a standardized way for the server to send content to the client without being first requested by the client.

* allowing messages to be passed back and forth while keeping the connection open.

* a two-way ongoing conversation can take place between the client and the server.

* Socket.IO is a library that enables real-time and full-duplex communication between the Client and the Web servers. 
* It uses the WebSocket protocol to provide the interface, it is divided into two parts; `both WebSocket` vs `Socket.io` are ***event-driven*** libraries.

![](https://miro.medium.com/max/2534/1*cvfhvyBIwTSvr5kG6jXHZQ.png)

****************************