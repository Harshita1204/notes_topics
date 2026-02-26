# Web Crawler

---

# Definition

A Web Crawler (also called a Spider or Bot) is a system that 
automatically browses the internet and collects web page data.

It starts from seed URLs and recursively discovers new links.

Used by:
- Search engines
- SEO tools
- Data aggregators
- Price comparison systems

---

# Basic Working Flow

1. Start with seed URLs
2. Fetch page content
3. Parse HTML
4. Extract links
5. Add new links to queue
6. Repeat

---

# Core Components

1. URL Frontier (Queue)
2. Fetcher
3. Parser
4. Storage System
5. Duplicate Detector
6. Scheduler

---

# Architecture Overview

User Input → Seed URLs
          ↓
      URL Queue
          ↓
      Fetcher (HTTP Client)
          ↓
        Parser
          ↓
  Extract Links + Store Data
          ↓
   Add new URLs to Queue

---

# Important Problems to Solve

## 1. Duplicate URLs

Same page may appear multiple times.

Solution:
- Use Hashing
- Use Bloom Filter
- Maintain Visited Set

---

## 2. Infinite Crawling

Pages can generate infinite URLs.

Solution:
- Depth limit
- Domain limit
- URL pattern filtering

---

## 3. Politeness Policy

Avoid overwhelming servers.

Solution:
- Respect robots.txt
- Rate limiting
- Delay between requests

---

## 4. Scalability

Single machine crawler is limited.

Large-scale crawlers use:

- Distributed workers
- Message queues
- Distributed storage

---

# Distributed Web Crawler Design

Master Node:
- Assign URLs
- Track visited links

Worker Nodes:
- Fetch pages
- Parse content
- Send new links back

Use:
- Message Queue (Kafka / RabbitMQ)
- Distributed DB (NoSQL)
- Object Storage

---

# Data Storage

Options:

- Store raw HTML
- Store parsed structured data
- Store metadata only

Common storage:
- NoSQL database
- Distributed file system

---

# Handling Failures

Crawler must handle:

- Timeout
- 404 errors
- Redirect loops
- Network failures

Implement:
- Retry mechanism
- Backoff strategy
- Status tracking

---

# Rate Limiting Strategy

Per-domain rate limit:

Example:
Max 1 request per second per domain.

Prevents IP banning.

---

# SEO Perspective

Search engines use crawlers to:

- Index pages
- Rank content
- Update search database

Crawler efficiency directly affects search freshness.

---

# System Design Interview Insight (20 LPA Level)

If asked:

"Design a web crawler for billions of pages"

You must discuss:

1. URL deduplication strategy
2. Distributed crawling
3. Storage optimization
4. Rate limiting
5. Monitoring and logging
6. Fault tolerance
7. Scalability plan

Do NOT just explain fetching pages.

---

# Scaling Strategy

Phase 1:
Single-threaded crawler

Phase 2:
Multi-threaded crawler

Phase 3:
Distributed crawler with:
- Load balancer
- Queue system
- Worker pool

---

# Advanced Concepts

- Breadth-First vs Depth-First crawling
- Priority-based crawling
- Focused crawling (domain-specific)
- Incremental crawling
- Event-driven crawling

---

# Real-World Example

Search engines like Google use highly distributed crawlers
running across thousands of machines.

Crawler architecture must be:

- Fault tolerant
- Scalable
- Polite
- Efficient
- Consistent

---

# Key Takeaway

A Web Crawler is a distributed system problem.

Main challenges:

- Scale
- Deduplication
- Rate limiting
- Storage
- Network reliability

Understanding these makes you ready 
for system design interviews.