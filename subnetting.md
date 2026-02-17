TOPIC: SUBNETTING


1. Definition
------------------------------------------------------------
Subnetting is the process of dividing a large network
into smaller logical networks called subnets.

It helps organize and manage IP addresses efficiently.


2. Why Subnetting Is Needed
------------------------------------------------------------
- Reduces network congestion.
- Improves security by isolating groups.
- Better IP address utilization.
- Easier network management.


3. How Subnetting Works
------------------------------------------------------------
Subnetting uses a Subnet Mask or CIDR notation
(e.g., /24) to divide the IP address into:

- Network portion
- Host portion

By adjusting the subnet mask, you control how many
subnets and hosts are created.


4. Example
------------------------------------------------------------
If a company has IP range:

192.168.1.0/24

It can divide it into smaller subnets like:

192.168.1.0/26
192.168.1.64/26
192.168.1.128/26
192.168.1.192/26

Each subnet will have fewer host devices.


5. Key Terms
------------------------------------------------------------
IP Address → Identifies device.
Subnet Mask → Divides network and host.
CIDR → Slash notation like /24.
Broadcast Address → Used to send to all hosts.


6. Benefits
------------------------------------------------------------
- Improves performance.
- Enhances security.
- Reduces broadcast traffic.
- Scales better in large organizations.



