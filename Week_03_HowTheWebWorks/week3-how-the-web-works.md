# Week 3 – How the Web Works (TryHackMe)

> Room: *How the Web Works*  
> Platform: TryHackMe

---

## 1. DNS – Domain Name System

### What DNS Is
- DNS translates **domain names ↔ IP addresses**.
- IPv4 example: `104.26.10.229`
- Users remember names like `tryhackme.com`, not numbers.

### Domain Hierarchy
- **TLD (Top Level Domain):** `.com`, `.org`, `.edu`, `.gov`, `.cz`, `.co.uk`
- **Second-level domain:** `tryhackme` in `tryhackme.com`
- **Subdomain:** `admin.tryhackme.com`, `store.tryhackme.com`

### Common DNS Record Types
- `A` – IPv4 address  
- `AAAA` – IPv6 address  
- `CNAME` – alias to another domain  
- `MX` – mail servers for the domain  
- `TXT` – arbitrary text (verification, SPF, DKIM, etc.)

### How a DNS Query Works (Simplified)
1. Computer checks **local DNS cache**.  
2. Asks a **recursive DNS resolver** (often from ISP).  
3. Resolver contacts **root servers**.  
4. Root servers direct it to the correct **TLD server**.  
5. TLD server points to the **authoritative nameserver**.  
6. Authoritative server returns the exact record.  
7. Result is cached for the duration of **TTL**.

---

## 2. HTTP and HTTPS

### HTTP vs HTTPS
- **HTTP** – protocol for transferring web content.  
- **HTTPS** – encrypted HTTP:  
  - prevents eavesdropping  
  - verifies authenticity of the server  

### Structure of a URL
Example:  
`https://user:pass@www.example.com:443/blog?id=1#comments`
- **Scheme:** `https`  
- **Credentials:** `user:pass` (rarely used today)  
- **Host:** `www.example.com`  
- **Port:** `443` (HTTPS), `80` (HTTP)  
- **Path:** `/blog`  
- **Query string:** `?id=1`  
- **Fragment:** `#comments`  

### Example HTTP Request
```http
GET / HTTP/1.1
Host: tryhackme.com
User-Agent: Mozilla/5.0 Firefox/87.0
Referer: https://tryhackme.com/
