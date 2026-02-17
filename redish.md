TOPIC: REDIS


1. Definition
------------------------------------------------------------
Redis stands for Remote Dictionary Server.

It is an in-memory key-value database used mainly
for caching, session storage, and real-time data.


2. How Redis Works
------------------------------------------------------------
- Stores data in RAM instead of disk.
- Uses key-value pairs.
- Extremely fast data access.
- Can optionally persist data to disk.


3. Key Characteristics
------------------------------------------------------------
- Very low latency (high speed).
- Supports data types like strings, lists, sets, hashes.
- Used for caching and pub/sub messaging.
- Scales well for high-traffic systems.


4. Common Use Cases
------------------------------------------------------------
- Caching database queries.
- Storing user sessions.
- Real-time analytics.
- Message queues.


5. Example
------------------------------------------------------------
Instead of fetching user data from database every time,
store it in Redis cache.

If data is in Redis → fast response.
If not → fetch from database and store in Redis.


6. Redis vs Traditional Database
------------------------------------------------------------
Redis:
- In-memory.
- Extremely fast.
- Mainly for temporary or fast-access data.

Traditional Database:
- Disk-based.
- Slower than Redis.
- Used for permanent storage.


