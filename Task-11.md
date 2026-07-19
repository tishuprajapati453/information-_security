## Task 11: Firewall Configuration and Access Control

**Overview:** Firewalls enforce which traffic is allowed in and out of a network or host — a core defensive control.

**Why it matters:** A firewall is often the first and simplest line of defense between a system and the wider internet, and misconfigured rules are one of the most frequent findings in real audits — either too permissive (exposing services that should be private) or so restrictive that legitimate traffic breaks. Learning to design rulesets around the principle of least privilege (deny by default, allow only what's needed) is a mindset that applies well beyond firewalls, into access control generally.

**Key Concepts:**
- Stateful vs stateless filtering
- Inbound vs outbound rules
- Principle of least privilege in access control

**Common Tools:**
- `iptables`, `ufw` (Linux), pfSense (network appliance)

**Example:**
```bash
# Allow SSH, deny everything else by default
sudo ufw default deny incoming
sudo ufw allow 22/tcp
sudo ufw enable
```

**Note:** Document every rule you add — unmanaged firewall rules are a common audit finding.

---

