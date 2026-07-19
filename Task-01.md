## Task 1: Introduction to Security Tools and Environment Setup

**Overview:** Before performing any security testing, you need a safe, isolated lab environment and the right toolset.

**Why it matters:** Every security professional's work starts here — without a controlled environment, even well-intentioned testing can accidentally damage real systems or cross legal lines. A dedicated lab (usually a set of VMs on an isolated network) lets you break things, experiment, and learn from mistakes without any real-world consequences. This foundation also builds the habit of thinking about scope and permission before touching any system — a mindset that carries through every other topic in this guide.

**Key Concepts:**
- Difference between offensive (red team) and defensive (blue team) security
- Legal and ethical boundaries — always test only on systems you own or have written permission for
- Setting up a security-focused OS (Kali Linux, Parrot OS)

**Common Tools:**
- Kali Linux / Parrot Security OS
- VirtualBox / VMware for isolated labs
- Terminal, package managers (`apt`, `pip`)

**Example:**
```bash
sudo apt update && sudo apt upgrade -y
sudo apt install nmap wireshark hydra -y
```

**Note:** Always work inside an isolated VM network so lab activity never touches production or public networks.

---

