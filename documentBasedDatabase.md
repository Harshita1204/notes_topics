TOPIC: DOCUMENT-BASED DATABASE


1. Definition
------------------------------------------------------------
A document-based database is a type of NoSQL database
that stores data in the form of documents instead of
tables and rows.

These documents are usually stored in JSON-like format.


2. How Data Is Stored
------------------------------------------------------------
Data is stored as independent documents.

Each document:
- Contains key-value pairs.
- Can have nested objects and arrays.
- Does not require a fixed schema.

Example:

{
  "name": "harshu",
  "age": 89,
  "skills": ["Node.js", "SQL"]
}


3. Key Characteristics
------------------------------------------------------------
- Flexible schema (structure can vary per document).
- No strict table structure.
- Easily scalable horizontally.
- Optimized for semi-structured data.


4. Example of Document-Based Databases
------------------------------------------------------------
- MongoDB
- CouchDB
- Firebase Firestore

MongoDB is the most commonly used document database.


5. Difference from Relational Database
------------------------------------------------------------
Relational Database:
- Uses tables with rows and columns.
- Fixed schema.
- Uses SQL.

Document Database:
- Uses JSON-like documents.
- Flexible schema.
- NoSQL-based.


6. When to Use
------------------------------------------------------------
- Applications with changing data structure.
- Rapid development projects.
- Large-scale web applications.
- Content management systems.



