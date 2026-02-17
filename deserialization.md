TOPIC: DESERIALIZATION


1. Definition
------------------------------------------------------------
Deserialization is the process of converting data from
a stored or transmitted format back into an object
or usable data structure.

It is the reverse of serialization.


2. Why Deserialization Is Needed
------------------------------------------------------------
- To read data received from an API.
- To convert JSON strings back into objects.
- To restore objects from stored files.
- To process network-transmitted data.

Applications cannot directly use string-form data,
so it must be converted back into structured form.


3. Example
------------------------------------------------------------
Serialized JSON string:

"{\"name\":\"Rupinder\",\"age\":25}"

After Deserialization (JavaScript Object):

{
  name: "Rupinder",
  age: 25
}

In JavaScript:
JSON.parse(string) → Deserialization


4. Where It Is Used
------------------------------------------------------------
- Handling API responses.
- Reading configuration files.
- Restoring session data.
- Distributed systems communication.


5. Important Concept
------------------------------------------------------------
Deserialization converts:
String (JSON/XML) → Object

Serialization and deserialization always work together
in data communication.




