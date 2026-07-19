## Task 12: System Log Monitoring and Analysis

**Overview:** Logs are the primary evidence trail for detecting and investigating security incidents.

**Why it matters:** When something goes wrong, logs are usually the only record of what actually happened — who logged in, what command ran, what file was accessed, and when. An attacker who has compromised a system will often try to delete or tamper with logs, which is exactly why centralized, tamper-resistant logging (shipping logs off the source machine immediately) is a security best practice. Learning to read logs quickly and spot anomalies is a foundational skill for both monitoring and incident response.

**Key Concepts:**
- Centralized logging (SIEM concepts)
- Key log locations on Linux (`/var/log/auth.log`, `/var/log/syslog`)
- Identifying anomalies (failed logins, unusual access times)

**Common Tools:**
- `journalctl`, `grep`/`awk`, ELK Stack (Elasticsearch, Logstash, Kibana), Splunk

**Example:**
```bash
# Check failed SSH login attempts
grep "Failed password" /var/log/auth.log

# Live log monitoring
sudo journalctl -f
```

**Note:** Set up log rotation and retention policies so logs are available long enough for investigations.

---

