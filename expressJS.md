TOPIC: EXPRESS JS


1. Definition
------------------------------------------------------------
Express.js is a fast and lightweight web framework 
built on top of Node.js.

It is mainly used to build web servers and REST APIs 
in a simple and structured way.

In simple terms:
Express.js helps developers create backend applications 
easily using JavaScript.


2. Why Express.js is Needed
------------------------------------------------------------
Node.js can create servers, but it requires more manual coding.

Express.js simplifies:
- Routing
- Handling requests and responses
- Middleware usage
- API creation

It reduces code complexity and speeds up development.


3. How Express.js Works
------------------------------------------------------------
Express follows the Request–Response model.

Step 1: Client sends a request.
Step 2: Express server receives the request.
Step 3: Server processes it.
Step 4: Server sends a response.

Example:
If user visits:
http://localhost:3000/

Express handles the request and returns a response.


4. Key Features
------------------------------------------------------------

1. Routing
   Allows handling different URLs and HTTP methods.

2. Middleware
   Functions that execute during request processing.

3. REST API Support
   Easy creation of GET, POST, PUT, DELETE routes.

4. Template Engine Support
   Can render dynamic HTML pages.


5. Basic Example
------------------------------------------------------------

const express = require('express');
const app = express();

app.get('/', (req, res) => {
    res.send('Hello World');
});

app.listen(3000);

Explanation:
- express() creates the server
- app.get() defines a route
- res.send() sends response
- app.listen() starts the server


6. Common HTTP Methods in Express
------------------------------------------------------------

app.get()      → Retrieve data
app.post()     → Send data
app.put()      → Update data
app.delete()   → Delete data

These are commonly used to build REST APIs.


7. Where Express.js Is Used
------------------------------------------------------------
- Backend development
- REST API development
- Web applications
- Real-time applications (with sockets)
- Microservices


8. Express vs Node.js
------------------------------------------------------------

Node.js:
- Runtime environment
- Executes JavaScript outside browser

Express.js:
- Framework built on Node.js
- Simplifies server and API development


9. Interview Explanation (Short Answer)
------------------------------------------------------------
Express.js is a minimal and flexible web framework for Node.js 
used to build web applications and REST APIs. It simplifies 
routing, request handling, and middleware management.
