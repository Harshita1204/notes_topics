TOPIC: LOOPBACK


1. Definition
------------------------------------------------------------
Loopback is a network mechanism that allows a device
to send network traffic to itself.

It is used for testing and internal communication
within the same machine.


2. Loopback Address
------------------------------------------------------------
The most common loopback IP address is:

127.0.0.1

Any request sent to this address does not leave
the computer. It returns back to the same system.


3. Purpose of Loopback
------------------------------------------------------------
- Testing network applications locally.
- Verifying that TCP/IP is working properly.
- Running local servers.
- Debugging network services.

Example:
When you access http://127.0.0.1:3000,
the request is handled by your own machine.


4. How It Works
------------------------------------------------------------
When a request is sent to the loopback address:
- The operating system detects it.
- The request is redirected internally.
- No external network communication occurs.


5. Loopback vs Localhost
------------------------------------------------------------
Loopback:
- Technical networking concept.
- Refers to the IP address 127.0.0.1.

Localhost:
- Hostname mapped to 127.0.0.1.
- More user-friendly term.

Both refer to the same internal communication.


