TOPIC: CACHING


1. Definition
------------------------------------------------------------
Caching is the process of storing frequently accessed
data in a temporary storage location to improve
retrieval speed.

It reduces the need to repeatedly fetch data from
a slower source like a database.


2. Why Caching Is Used
------------------------------------------------------------
- Improves application performance.
- Reduces database load.
- Decreases response time.
- Enhances user experience.


3. How Caching Works
------------------------------------------------------------
Step 1: User requests data.
Step 2: System checks cache first.
Step 3: If data exists (cache hit), return it.
Step 4: If not (cache miss), fetch from database,
        store in cache, then return.

Cache hit → Fast response  
Cache miss → Slower response


4. Types of Caching
------------------------------------------------------------
- In-memory caching (Redis, Memcached).
- Browser caching.
- CDN caching.
- Application-level caching.


5. Example
------------------------------------------------------------
If a website homepage is accessed frequently,
its data can be stored in Redis cache instead
of querying the database every time.


