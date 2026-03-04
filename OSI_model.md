# OSI Model (Open Systems Interconnection)

## Definition

The OSI Model is a conceptual framework used to understand how
network communication works between systems.

It divides networking into **7 layers**, where each layer has a specific role.

---

# 7 Layers of OSI Model

| Layer | Name | Function |
|-----|-----|-----|
| 7 | Application | User-facing network services |
| 6 | Presentation | Data formatting, encryption |
| 5 | Session | Session management |
| 4 | Transport | Reliable data delivery |
| 3 | Network | Routing packets |
| 2 | Data Link | Node-to-node communication |
| 1 | Physical | Transmission of bits |

---

# Layer Explanation

## 7. Application Layer
Closest to the user.

Protocols:
- HTTP
- FTP
- SMTP
- DNS

---

## 6. Presentation Layer

Responsible for:
- Encryption
- Compression
- Data translation

Example:
SSL/TLS encryption.

---

## 5. Session Layer

Manages connections between applications.

Responsibilities:
- Session establishment
- Session maintenance
- Session termination

---

## 4. Transport Layer

Responsible for reliable data transmission.

Protocols:
- TCP
- UDP

Functions:
- Error detection
- Flow control
- Segmentation

---

## 3. Network Layer

Responsible for packet routing.

Protocol:
- IP (Internet Protocol)

Devices:
- Routers

---

## 2. Data Link Layer

Handles communication between devices in the same network.

Functions:
- MAC addressing
- Error detection

Devices:
- Switches

---

## 1. Physical Layer

Handles transmission of raw bits over medium.

Examples:
- Ethernet cables
- Fiber optic cables
