# Message Queues

## Review, Researh, and Discussion

### What does it mean that web sockets are bidirectional? Why is this useful?

Bidirectional is a communications mode that is capable of transmitting data in both directions (send and receive), but not at the same time.
It is useful to know so we can track events that are happening at the same time.

### Does socket.io use HTTP? Why?

Yes, a socket.io server will attach itself to a HTTP server so it can serve its own client code.

### What happens when a client emits an event?

The server recieves the event and triggers an event if its listening to said event.

### What happens when a server emits an event?

The client receives the event and triggers corresponding event.

### What happens if a client “misses” an event?

It disappears unless you have a way to store the event.

### How can we mitigate this?

Create a queue that holds on to events that was not received.

## Vocab Term

- Socket - software structure within a network node of a computer network that serves as an endpoint for sending and receiving data across the network.
- Web Scoket -  a computer communications protocol, providing full-duplex communication channels over a single TCP connection.
- Socket.io - is a library that enables real-time, bidirectional and event-based communication between the browser and the server.
- Client - an application that will request to connect with a socket.io server,
- Server - a central hub that manages all client connections and passed down events to necessary clients.
- OSI Model - designed to describe the functions of the communication system by dividing the communication procedure into smaller and simpler components
- TCP Model - concise version of the OSI model.
- TCP - (Transmission Control Protocol) is a standard that defines how to establish and maintain a network conversation through which application programs can exchange data.
- UDP - (User Datagram Protocol) is a communications protocol that is primarily used for establishing low-latency and loss-tolerating connections between applications on the internet.
- Packets - formatted unit of data, consisting of control information and user data; the latter is also known as the payload.
