TOPIC: VECTOR DATABASE


1. Definition
------------------------------------------------------------
A vector database is a type of database designed to
store and manage data in the form of numerical vectors.

It is mainly used in AI and machine learning systems
for similarity search.


2. What is a Vector
------------------------------------------------------------
A vector is a list of numbers that represents data.

For example:
Text, image, or audio is converted into numbers
(embeddings) using an AI model.

Example:
"Hello world" → [0.23, -0.91, 0.77, ...]

These numbers capture the meaning of the content.


3. Why Vector Database Is Needed
------------------------------------------------------------
- To perform similarity search.
- To support AI-powered applications.
- To retrieve data based on meaning, not exact match.
- To handle high-dimensional embeddings efficiently.


4. How It Works
------------------------------------------------------------
Step 1: Data is converted into vector embeddings.
Step 2: Vectors are stored in the database.
Step 3: When a query comes, it is also converted to a vector.
Step 4: Database finds the closest matching vectors.

This is called nearest neighbor search.


5. Common Use Cases
------------------------------------------------------------
- Semantic search engines.
- Chatbots with memory.
- Recommendation systems.
- Image similarity search.


6. Examples of Vector Databases
------------------------------------------------------------
- Pinecone
- Milvus
- Weaviate
- FAISS (library-based)


