# Cyber Security Basics
**CZ:** Základy kyberbezpečnosti  
**Platform:** TryHackMe  
**Date completed:** 2025-11-05  

---

## Summary
This room introduces the fundamental principles of cybersecurity — how to protect systems, networks, and data from digital attacks.  
It explains the CIA Triad (Confidentiality, Integrity, Availability), the difference between offensive and defensive security, and key security roles.

---

## Key Concepts Learned

### What is Cyber Security
Cyber Security means protecting digital systems, networks, and data from unauthorized access, damage, or misuse.  
Common attack types include:
- **Data Breach** – stealing sensitive information  
- **Ransomware** – encrypting data for ransom  
- **Phishing** – tricking users into giving away credentials  
- **Malware** – malicious software  
- **DoS/DDoS** – flooding a system to make it unavailable  

---

### The CIA Triad – Confidentiality, Integrity, Availability
| Principle | Meaning | Example |
|------------|----------|---------|
| **Confidentiality** | Only authorized users can access the data | Only doctors can see medical records |
| **Integrity** | Data remains accurate and unmodified | Invoice numbers cannot be changed |
| **Availability** | Systems must be available when needed | The website must run 24/7 |

 If one of these principles is broken → it becomes a **security incident**.

---

### Offensive vs. Defensive Security
Cybersecurity has two main branches:

#### Offensive Security
Think like a hacker — find vulnerabilities before attackers do.  
Examples:
- **Penetration Testing** – simulate attacks to test defenses  
- **Exploiting Vulnerabilities** – testing what happens if a weakness is abused  
- **Reverse Engineering** – analyzing how applications work  

 *Example:*  
In the TryHackMe **FakeBank** exercise, we used the `dirb` tool to brute-force hidden URLs on a website.

#### Defensive Security
Protect systems and detect malicious activity early.  
Typical activities:
- **Network Monitoring**  
- **Log Analysis**  
- **Incident Response**  
- **Security Policy Development**

 Teams are often called:
- **Blue Team** → defense  
- **Red Team** → offense (testing the defenses)

---

### Security Roles
| Role | Description |
|------|--------------|
| **Penetration Tester / Ethical Hacker** | Finds vulnerabilities and tests systems legally |
| **SOC Analyst** | Monitors networks, detects and investigates attacks |
| **Security Engineer** | Designs and maintains security systems |
| **Digital Forensic Examiner** | Analyzes digital evidence and incidents |

 In practice, these roles work together:  
A SOC Analyst detects an anomaly → a Forensic Examiner investigates → a Security Engineer fixes the issue.

---

### Key Security Terms
| Term | Meaning | Description |
|------|----------|-------------|
| **Threat** | Hrozba | Potential danger to a system |
| **Vulnerability** | Zranitelnost | Weak point that can be exploited |
| **Exploit** | Zneužití | Method to use a vulnerability |
| **Patch** | Záplata | Update that fixes a security issue |
| **Incident** | Událost | Security breach or attempt |
| **Phishing** | Podvod | Fake messages used to steal information |
| **Malware** | Škodlivý software | Software designed to harm a system |
| **Firewall** | Síťová brána | Filters network traffic by rules |
| **SIEM** | Security Information and Event Management | Collects and correlates security events |

---

## Real-world Relevance (SOC / Cyber Analyst)
Understanding the CIA triad and security principles is essential for every SOC analyst.  
It helps recognize the *type of incident* (Confidentiality → Data Breach, Availability → DDoS).  
Knowledge of both Red and Blue Team operations builds better defensive thinking.

---

## Personal Reflection
This introduction gave me a clear picture of what cybersecurity means in practice.  
I now understand how offensive and defensive roles work together, and why the CIA triad forms the foundation of all security decisions.
