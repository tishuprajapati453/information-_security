## Task 7: Vulnerability Assessment

**Overview:** Once services are enumerated, the next step is checking them against known vulnerabilities.

**Why it matters:** Finding a service is only half the picture — knowing that it's running an outdated, exploitable version turns raw information into an actionable finding. This is where reconnaissance connects to risk: a CVSS score helps prioritize which of dozens of findings actually deserves urgent attention versus which can wait. Learning to separate a scanner's automated "maybe" from a manually confirmed "yes, this is exploitable" is a core skill that separates junior from senior analysts.

**Key Concepts:**
- CVE (Common Vulnerabilities and Exposures) database
- CVSS scoring (severity rating of a vulnerability)
- Automated scanners vs manual verification

**Common Tools:**
- OpenVAS, Nessus, Nikto (for web servers)

**Example:**
```bash
# Basic web server vulnerability scan
nikto -h http://192.168.1.10
```

**Note:** A scanner flags *potential* issues — always manually verify before reporting a finding as confirmed.

---

