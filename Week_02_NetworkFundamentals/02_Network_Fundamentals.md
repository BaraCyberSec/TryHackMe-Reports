# Network Fundamentals
**CZ:** Základy sítí  
**Platform:** TryHackMe  
**Date completed:** 2025-11-06  

---

## Summary
This room introduces how computer networks work — how devices communicate, what IP addresses are, and how data travels across networks.  
It explains the OSI and TCP/IP models, ARP, DHCP, and common networking tools.

---

## Key Concepts Learned

### What is a Network
A network is a group of connected devices (computers, routers, switches) that share data.  
Networks enable communication between systems using specific rules called **protocols**.

---

### IP and MAC Addresses
- **IP address** identifies a device on the network (like your home address).  
- **MAC address** is a unique hardware identifier of the network card.  
 IP changes over time, MAC never changes (it’s “burned” into the device).

**Private IP ranges:**  
`192.168.0.0/16`, `10.0.0.0/8`, `172.16.0.0/12`  
**Public IPs:** used on the Internet.

---

### ARP and DHCP
- **ARP (Address Resolution Protocol)** – translates IP to MAC address.  
- **DHCP (Dynamic Host Configuration Protocol)** – assigns IP addresses automatically to devices in a LAN.

```bash
arp -a
ipconfig /all
```

---

### OSI Model
The **OSI model** (Open Systems Interconnection) describes how data travels through 7 layers.  

| Layer | Name | Description | Example |
|-------|------|--------------|----------|
| 7 | Application | End-user interface | HTTP, DNS |
| 6 | Presentation | Data formatting/encryption | SSL/TLS |
| 5 | Session | Manages communication sessions | RDP, NetBIOS |
| 4 | Transport | Reliable delivery of data | TCP, UDP |
| 3 | Network | Logical addressing, routing | IP |
| 2 | Data Link | MAC addressing | Ethernet |
| 1 | Physical | Cables, Wi-Fi, hardware | Fiber, copper |

Remember: **"Please Do Not Throw Sausage Pizza Away"**  
(Physical → Application) – a funny way to memorize OSI layers.

---

### TCP/IP Model
A simplified, practical version of the OSI model used in real networks.  

| Layer | Function | Example |
|--------|-----------|----------|
| Application | User interaction | HTTP, DNS |
| Transport | Delivery | TCP, UDP |
| Internet | Routing | IP |
| Network Access | Hardware communication | Ethernet, Wi-Fi |

---

### Ports and Protocols
Communication happens via **ports** — like doors used by specific services.

| Protocol | Port | Description |
|-----------|------|-------------|
| HTTP | 80 | Web traffic |
| HTTPS | 443 | Secure web traffic |
| FTP | 21 | File transfer |
| SSH | 22 | Secure remote login |
| DNS | 53 | Name resolution |
| SMTP | 25 | Email sending |
| RDP | 3389 | Remote desktop |

```bash
netstat -ano
```

---

## Tools / Commands Practiced
- `ping` – test network connectivity  
- `tracert` / `traceroute` – show path to target  
- `ipconfig` / `ifconfig` – view network configuration  
- `arp -a` – display ARP table  

```bash
ping 8.8.8.8
tracert tryhackme.com
```

---

## Real-world Relevance (SOC / Cyber Analyst)
Networking knowledge is essential for any SOC Analyst.  
Understanding IPs, ports, and protocols helps identify:
- suspicious traffic in SIEM logs,  
- lateral movement between systems,  
- unusual open ports or data exfiltration.

SOC analysts must be able to read network logs and recognize when something doesn’t “look right”.

---

## Personal Reflection
Networking fundamentals helped me understand how data actually moves between computers.  
I can now read IPs, identify protocols, and visualize how traffic flows through each OSI layer —  
a crucial skill for detecting real-world cyber threats.




