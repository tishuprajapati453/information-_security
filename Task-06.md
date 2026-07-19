## Task 6: Network Scanning and Enumeration

**Overview:** Scanning identifies live hosts, open ports, and running services — the reconnaissance phase of security testing.

**Why it matters:** You can't assess or defend a system you don't know exists. Scanning builds the map of "what's actually out there" — which machines are alive, what doors (ports) are open on them, and what software is listening behind those doors. This is the very first practical step in almost any real penetration test or internal security review, and it's equally useful defensively: regularly scanning your own network reveals shadow IT and forgotten services before an attacker finds them first.

**Key Concepts:**
- Host discovery vs port scanning vs service/version detection
- TCP vs UDP scans
- Enumeration = digging deeper into discovered services (shares, users, banners)

**Common Tools:**
- Nmap, Netcat, enum4linux

**Example:**
```bash
# Discover live hosts on a subnet
nmap -sn 192.168.1.0/24

# Scan for open ports + service versions
nmap -sV -p 1-1000 192.168.1.10
```

**Note:** Only scan networks you own or have explicit written authorization for — unauthorized scanning can be illegal.

---

