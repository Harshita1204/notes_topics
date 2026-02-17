TOPIC: SERIALIZATION


1. Definition
------------------------------------------------------------
Serialization is the process of converting an object
or data structure into a format that can be stored
or transmitted.

Common formats:
- JSON
- XML
- Binary

It converts in-memory data into a transferable format.


2. Why Serialization Is Needed
------------------------------------------------------------
- To send data over a network.
- To store data in files.
- To save objects in databases.
- To cache objects.

Computers cannot directly send memory objects,
so they must be converted into a structured format.


3. Example
------------------------------------------------------------
JavaScript Object:

{
  name: "Rupinder",
  age: 25
}

After Serialization (JSON string):

"{\"name\":\"Rupinder\",\"age\":25}"

In JavaScript:
JSON.stringify(object) → Serialization


4. Where It Is Used
------------------------------------------------------------
- API communication
- Saving session data
- Storing configuration
- Distributed systems


5. Important Concept
------------------------------------------------------------
Serialization converts:
Object → String (or storable format)

The reverse process is called Deserialization.


