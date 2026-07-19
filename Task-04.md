## Task 4: Network Configuration and Diagnostics

**Overview:** Understanding how networks are configured helps you diagnose issues and understand attack surfaces.

**Why it matters:** You can't secure or test what you don't understand. Knowing how devices get IP addresses, how DNS resolves names, and how traffic routes between networks gives you a mental map of where an attacker could intercept, redirect, or block communication. This diagnostic skill is also what you'll rely on constantly when a scan or exploit doesn't work as expected — nine times out of ten the issue turns out to be a network configuration problem, not a tool problem.

**Key Concepts:**
- IP addressing, subnetting, and DNS basics
- Checking connectivity and routes
- Interface configuration

**Common Tools & Commands:**
```bash
ip a                 # view network interfaces
ping google.com       # test connectivity
traceroute google.com # trace network path
netstat -tulnp        # view open ports/connections
dig example.com       # DNS lookup
```

**Note:** Knowing your own network layout (gateway, subnet, DNS) is the first step before scanning anything else.

---

