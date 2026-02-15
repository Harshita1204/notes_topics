TOPIC: PORT


1. Definition
------------------------------------------------------------
A port is a logical communication endpoint used by a 
computer to identify a specific application or service 
running on it.

In simple terms:
A port helps the computer know which application 
should receive the incoming data.


2. Why Port Is Needed
------------------------------------------------------------
A single computer can run multiple applications at 
the same time.

For example:
- Web server
- Database server
- Email service

The IP address identifies the device.
The port number identifies the specific application 
on that device.

Without ports, the system would not know where to send 
the incoming request.


3. How Port Works
------------------------------------------------------------
When data is sent over the internet, it contains:

- IP Address (identifies the device)
- Port Number (identifies the application)
- Protocol (TCP or UDP)

Example:
If you open a website:
The request goes to:
IP address + Port 80 (HTTP)

The server knows the request is for the web service.


4. Common Port Numbers
------------------------------------------------------------

Port 80    → HTTP (Web traffic)
Port 443   → HTTPS (Secure web traffic)
Port 21    → FTP (File transfer)
Port 22    → SSH (Secure remote access)
Port 25    → SMTP (Email sending)
Port 3306  → MySQL database
Port 3000  → Commonly used for development servers


5. Port Range
------------------------------------------------------------
Port numbers range from 0 to 65535.

They are divided into:

1. Well-known ports (0–1023)
   Used by common services like HTTP, HTTPS.

2. Registered ports (1024–49151)
   Used by specific applications.

3. Dynamic/Private ports (49152–65535)
   Used temporarily by client applications.


6. Real-Life Analogy
------------------------------------------------------------
Think of an apartment building.

IP address = Building address
Port number = Apartment number

Mail reaches the building (IP).
The apartment number (port) decides which person 
receives the mail.

