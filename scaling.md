# Scaling in System Design

## Definition

Scaling is the process of increasing system capacity to handle 
more traffic, more users, or more data without performance degradation.

Goal:
Maintain low latency, high availability, and reliability under load.

---

# Types of Scaling

## 1. Vertical Scaling (Scale Up)

Definition:
Increase resources of a single machine.

Example:
- Add more RAM
- Add more CPU cores
- Upgrade SSD

Example Scenario:
Upgrade server from 8GB RAM → 32GB RAM

### Advantages
- Simple to implement
- No code change required
- No distributed system complexity

### Limitations
- Hardware limit exists
- Expensive at high capacity
- Single point of failure remains

---

## 2. Horizontal Scaling (Scale Out)

Definition:
Add more machines instead of upgrading one.

Example:
1 server → 5 servers behind load balancer

### Advantages
- High availability
- Better fault tolerance
- Virtually unlimited scaling

### Challenges
- Requires distributed system design
- Data synchronization issues
- Session management problems

---

# Load Balancer

Used in horizontal scaling.

Role:
- Distribute incoming requests
- Prevent single server overload
- Improve availability

Common Algorithms:
- Round Robin
- Least Connections
- IP Hash

---

# Database Scaling

## 1. Read Replicas

Primary DB handles writes.
Replica DB handles reads.

Improves read performance.

## 2. Sharding

Split database based on key.

Example:
User ID 1-1000 → Server A
User ID 1001-2000 → Server B

Used in very large systems.

---

# Caching for Scaling

Caching reduces load on backend.

Example:
Store frequent queries in Redis.

Benefits:
- Reduced DB load
- Faster response time
- Lower latency

Cache Strategies:
- Cache Aside
- Write Through
- Write Back

---

# Stateless vs Stateful Services

For horizontal scaling:

Stateless services are easier to scale.

Store sessions in:
- Redis
- Database
- JWT tokens

Avoid in-memory session storage.

---

# Auto Scaling (Cloud Perspective)

In cloud platforms:

- Automatically add servers when CPU usage > threshold
- Remove servers when traffic reduces

Improves cost efficiency.

---

# Real-World Scaling Strategy

Step 1: Optimize code
Step 2: Add caching
Step 3: Add load balancer
Step 4: Add horizontal scaling
Step 5: Scale database
Step 6: Introduce microservices (if required)

---

# Bottlenecks in Scaling

- Database
- Network latency
- Disk I/O
- CPU usage
- Lock contention

Always identify bottleneck before scaling.

---

# Interview-Level Insight (20 LPA Perspective)

Scaling is not just adding servers.

It involves:

- Performance monitoring
- Identifying bottlenecks
- Distributed architecture decisions
- CAP theorem tradeoffs
- Observability (logs, metrics, tracing)

Companies expect engineers to think:

"Where will system break at 10x traffic?"

Not:
"Add more RAM."

---

# Horizontal vs Vertical Quick Comparison

| Feature | Vertical Scaling | Horizontal Scaling |
|----------|------------------|-------------------|
| Complexity | Low | High |
| Cost Efficiency | Low at scale | High at scale |
| Fault Tolerance | Low | High |
| Limit | Hardware bound | Practically unlimited |

---

# Key Takeaway

Good scalable architecture:

- Stateless services
- Load balancer
- Caching layer
- Database replication
- Monitoring
- Auto scaling

Scaling is about removing bottlenecks efficiently,
not blindly increasing infrastructure.
