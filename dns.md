# DNS (Domain Name System)

## Definition

DNS translates human-readable domain names into IP addresses.

Example:

google.com → 142.250.190.78

Without DNS, users would need to remember IP addresses.

---

# DNS Resolution Process

1. Browser checks cache
2. OS checks local cache
3. Query sent to DNS resolver
4. Resolver queries root server
5. Root server directs to TLD server
6. TLD server directs to authoritative server
7. IP address returned

---

# DNS Hierarchy

1. Root servers
2. TLD servers (.com, .org)
3. Authoritative servers

---

# DNS Caching

To improve performance, DNS responses are cached at:

- Browser
- OS
- ISP
- DNS resolver

