## Task 3: Virtual Machine Setup and Management

**Overview:** Virtual machines (VMs) let you create disposable, isolated test systems for safe experimentation.

**Why it matters:** VMs are what make a personal security lab possible without needing a room full of physical hardware. Because a VM is just a file on your disk, you can copy it, snapshot it, break it, and restore it in seconds — this is what lets you practice attacks and defenses over and over with zero real risk. Understanding VM networking modes is especially important, since a misconfigured network setting is the most common way lab traffic accidentally leaks onto a real network.

**Key Concepts:**
- Type 1 (bare-metal) vs Type 2 (hosted) hypervisors
- Snapshots — save a VM state and roll back after testing
- Isolated/host-only networking to prevent lab traffic leaking out

**Common Tools:**
- VirtualBox, VMware Workstation, Hyper-V

**Example workflow:**
1. Create a new VM, allocate 2–4 GB RAM
2. Install target OS (e.g., Metasploitable, DVWA VM)
3. Take a snapshot before testing
4. Set network adapter to "Host-only" or "Internal Network"

**Note:** Snapshots are your safety net — always snapshot before running anything experimental.

---

