TOPIC: SOCKET

1. Definition
------------------------------------------------------------
A socket is an endpoint used for communication between 
two computers over a network.

In simple terms:
A socket allows two systems to send and receive data 
over the internet or a network.

It is used in client-server communication.

------------------------------------------------------------

2. Simple Meaning
------------------------------------------------------------
If API is a messenger between applications,
then a socket is the actual communication channel 
through which data travels.

A socket connects:
Client ↔ Server

It enables real-time data transfer.

------------------------------------------------------------

3. Real-Life Analogy
------------------------------------------------------------
Think of a telephone call.

Person A dials a number.
Person B answers.
They talk in real time.

The phone connection between them is like a socket.

Without the connection, communication cannot happen.

------------------------------------------------------------

4. How Socket Works
------------------------------------------------------------
Step 1: Server creates a socket and waits for connections.
Step 2: Client creates a socket and connects to the server.
Step 3: Connection is established.
Step 4: Data is sent and received.
Step 5: Connection is closed.

This is called a TCP connection process.

------------------------------------------------------------

5. Components of a Socket
------------------------------------------------------------
A socket is identified by:

- IP Address (identifies the device)
- Port Number (identifies the application)
- Protocol (TCP or UDP)

Example:
IP: 192.168.1.1
Port: 8080
Protocol: TCP

------------------------------------------------------------

6. Types of Sockets
------------------------------------------------------------

1. TCP Socket
   - Connection-oriented
   - Reliable
   - Data arrives in correct order
   - Used in web browsing, emails

2. UDP Socket
   - Connectionless
   - Faster but less reliable
   - No guarantee of order
   - Used in video streaming, gaming

------------------------------------------------------------

7. Where Sockets Are Used
------------------------------------------------------------
- Chat applications
- Online gaming
- Video conferencing
- Web servers
- Real-time data systems

Whenever continuous communication is required, 
sockets are used.

------------------------------------------------------------

8. Difference Between API and Socket
------------------------------------------------------------

API:
- A set of rules for communication
- Defines how requests and responses happen

Socket:
- The actual communication channel
- Handles data transmission between systems

API uses sockets internally for network communication.




