# Readings: Message Queues
## Review, Research, and Discussion
1. What does it mean that web sockets are bidirectional? Why is this useful?
    - WebSockets allow for full-duplex bidirectional communication. This enables the server to send real-time updates asynchronously, without requiring the client to submit a request each time. [source](https://www.amx.com/en/site_elements/benefits-and-applications-of-websockets#:~:text=BIDIRECTIONAL.,submit%20a%20request%20each%20time.)
2. Does socket.io use HTTP? Why?
    - The socket API supports different protocols from the transport layer and down. That means that if you would like to use TCP you use sockets. But you can also use sockets to communicate using HTTP, but then you have to decode/encode messages according to the HTTP specification  [source](https://stackoverflow.com/questions/15108139/difference-between-socket-programming-and-http-programming)
3. What happens when a client emits an event?
    - when the client emit an enent it reaches the srever which in its role has a listnere and call back function the triggered once we emit .
4. What happens when a server emits an event?
    - it reaches the client where there is a listener for this event and callback function.
5. What happens if a client “misses” an event?
    - if there is no queues in this case the client will lose the call back function
6. How can we mitigate this?
    - by using message queues in the server that will allow client to rehave the messages once he backs.

## DOCUMENTATION:
Socket
:  A socket is one endpoint of a two-way communication link between two programs running on the network. A socket is bound to a port number so that the TCP layer can identify the application that data is destined to be sent to Every TCP connection can be uniquely identified by its two endpoints.

Web Socket
:  WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection

Socket.io
:   is a JavaScript library for realtime web applications. It enables realtime, bi-directional communication between web clients and servers

Client
:  a desktop computer or workstation that is capable of obtaining information and applications from a server

Server
:  A server is a computer or system that provides resources, data, services, or programs to other computers

OSI Model
:  The OSI Model (Open Systems Interconnection Model) is a conceptual framework used to describe the functions of a networking system. The OSI model characterizes computing functions into a universal set of rules and requirements in order to support interoperability between different products and software.
![img](https://cdn.educba.com/academy/wp-content/uploads/2019/07/OSI-Model.png)

TCP Model
:  The Internet protocol suite, commonly known as TCP/IP, is the set of communications protocols used in the Internet and similar computer networks. The current foundational protocols in the suite are the Transmission Control Protocol and the Internet Protocol.

TCP
:  The Transmission Control Protocol is one of the main protocols of the Internet protocol suite. It originated in the initial network implementation in which it complemented the Internet Protocol.

UDP
:  User Datagram Protocol (UDP) is a communications protocol that is primarily used to establish low-latency and loss-tolerating connections between applications on the internet. UDP speeds up transmissions by enabling the transfer of data before an agreement is provided by the receiving party.
![img](https://sergeyzhuk.me/assets/images/posts/reactphp/tcpvsudp.jpg)

Packets 
:  A packet is the unit of data routed between an origin and a destination on the internet or other packet-switched network -- or networks that ship data around in small packets.    


## REVIEW :

- Socket IO installation
> npm i socket.io
- require socket.io
> const io= require('socket.io)
- connect to the port
> const io= require('socket.io)(port || process.env.PORT)
- Create a namespace:
> io.on('connection',payload=>{ console.log('cnnected to nameSpace)})
