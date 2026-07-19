## Task 2: Linux System Administration Basics

**Overview:** Most security tools run on Linux, so comfort with the command line is essential.

**Why it matters:** Nearly every security tool (Nmap, Wireshark, Metasploit, Burp Suite CLI helpers) is built to run natively on Linux, and most servers you'll investigate in the real world are Linux-based too. Being fluent in the shell — navigating directories, chaining commands with pipes, and understanding permissions — means you spend less time fighting the environment and more time actually analyzing the problem in front of you.

**Key Concepts:**
- File system hierarchy (`/etc`, `/var`, `/home`, `/bin`)
- User and permission management (`chmod`, `chown`, `sudo`)
- Process management (`ps`, `top`, `kill`)
- Package management and services (`systemctl`)

**Example:**
```bash
# Change file permissions
chmod 750 script.sh

# View running processes
ps aux | grep python

# Manage a service
sudo systemctl status ssh
```

**Note:** Practice navigating with `cd`, `ls -la`, `find`, and `grep` — these are used constantly during investigations.

---

