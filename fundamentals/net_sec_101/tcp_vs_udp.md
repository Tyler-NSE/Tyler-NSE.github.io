---
layout: default
---

# TCP vs UDP

***

- [TCP](#tcp)
- [UDP](#udp)
- [Differences Between TCP and UDP](#differences-between-tcp-and-udp)


TCP (Transmission Control Protocol) and UDP (User Datagram Protocol) are two core protocols of the Transport Layer of the OSI and TCP/IP models. Both are responsible for end-to-end communication between applications, but they differ significantly in terms of reliability, speed, and use cases. Understanding the difference between TCP and UDP is essential for designing efficient and reliable networked systems.

## TCP

TCP is a reliable, connection-oriented transport protocol that ensures accurate and ordered data delivery. It uses control mechanisms to guarantee data correctness, which makes it slower but dependable.

*   Connection-oriented protocol
*   Reliable and ordered data delivery
*   Higher overhead but high accuracy

## UDP

UDP is a fast, connectionless transport protocol that sends data without reliability guarantees. It is efficient for applications where speed is more important than accuracy.

*   Connectionless and lightweight
*   No guarantee of delivery or order
*   Low overhead and high speed

## Differences Between TCP and UDP

|       TCP (Transmission Control Protocol)       |      UDP (User Datagram Protocol)      |
|:-----------------------------------------------:|:--------------------------------------:|
| Connection-oriented; uses a three-way handshake |      Connectionless; no handshake      |
|        Guarantees reliable data delivery        |       Does not guarantee delivery      |
|           Uses acknowledgements (ACKs)          |           No acknowledgements          |
|     Supports retransmission of lost packets     |        No retransmission support       |
|      Ensures packets are delivered in order     |        Does not ensure ordering        |
|   Provides flow control and congestion control  |      No flow or congestion control     |
|          Slower due to higher overhead          |      Faster with minimal overhead      |
|        Variable header size (20–60 bytes)       |       Fixed header size (8 bytes)      |
|     Treats data as a continuous byte stream     |   Treats data as independent messages  |
|  Does not support broadcasting or multicasting  | Supports broadcasting and multicasting |
|          Used by HTTP, HTTPS, FTP, SMTP         |   Used by DNS, DHCP, VoIP, Streaming   |

[back](/fundamentals/networks_and_security.html)