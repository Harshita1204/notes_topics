TOPIC: CAP THEOREM


1. Definition
------------------------------------------------------------
CAP Theorem states that a distributed system can only
guarantee two out of the following three properties:

- Consistency
- Availability
- Partition Tolerance

It is a fundamental concept in distributed databases.


2. The Three Components
------------------------------------------------------------
1. Consistency (C)
   Every read receives the most recent write.
   All nodes see the same data at the same time.

2. Availability (A)
   Every request receives a response,
   even if some nodes fail.

3. Partition Tolerance (P)
   The system continues to operate even if
   there is a network failure between nodes.


3. Why It Matters
------------------------------------------------------------
In distributed systems, network failures can happen.
When a partition occurs, the system must choose between:

- Consistency
or
- Availability

It cannot guarantee both at the same time.


4. Types of Systems Based on CAP
------------------------------------------------------------
CP (Consistency + Partition Tolerance)
- Prioritizes accurate data.
- May reject requests during failure.

AP (Availability + Partition Tolerance)
- Always responds.
- Data may be temporarily inconsistent.

CA (Consistency + Availability)
- Works only when no partition occurs.
- Rare in distributed systems.


5. Example
------------------------------------------------------------
In a distributed database:

If one server cannot communicate with another,
the system must choose:

- Stop responding (to maintain consistency), or
- Continue responding with possibly outdated data.


