## Task 13: Malware Identification and Safe Analysis

**Overview:** Recognizing malicious files/behavior and analyzing them safely without risking real infection.

**Why it matters:** Being able to recognize the signs of malware — an unexpected process, a file reaching out to an unfamiliar server, a scheduled task that reappears after deletion — is essential for anyone doing incident response or system administration. Safe analysis technique matters just as much as identification skill: this topic is as much about *discipline* (never running unknown files on a real machine) as it is about technical steps, since a single mistake here can cause a real infection.

**Key Concepts:**
- Static analysis (examining a file without running it) vs dynamic analysis (observing behavior in a sandbox)
- Indicators of Compromise (IOCs): unusual processes, network beacons, persistence mechanisms
- Always analyze in an isolated, disposable/snapshotted VM with no internet access

**Common Tools:**
- VirusTotal (hash/file reputation lookup), `strings`, a sandboxed VM (e.g., Cuckoo Sandbox concepts)

**Example (static, safe):**
```bash
# Check a suspicious file's hash before running it anywhere
sha256sum suspicious_file.exe
# Look up the hash on VirusTotal instead of executing the file
```

**Note:** Never execute unknown/suspicious files on your host machine — only in a fully isolated, network-disconnected VM snapshot.

---

