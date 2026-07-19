## Task 5: Packet Capture and Traffic Analysis

**Overview:** Capturing and analyzing network packets reveals what's actually happening on the wire — useful for troubleshooting and detecting suspicious activity.

**Why it matters:** Logs and dashboards can lie or miss things, but packets don't — they're the raw ground truth of what was actually sent between two machines. This skill is central to both offense (understanding how a protocol works well enough to exploit it) and defense (spotting a plaintext credential, an unusual outbound connection, or a malware beacon). Learning to read a TCP handshake or an HTTP request byte-by-byte builds an intuition that no automated tool can fully replace.

**Key Concepts:**
- Promiscuous mode capturing
- Protocol analysis (TCP/UDP/HTTP handshakes)
- Filters to isolate relevant traffic

**Common Tools:**
- Wireshark (GUI), tcpdump (CLI)

**Example:**
```bash
# Capture traffic on interface eth0, filter for HTTP
sudo tcpdump -i eth0 port 80 -w capture.pcap

# In Wireshark, filter:
http.request
ip.addr == 192.168.1.10
```

**Note:** Always capture traffic only on networks/systems you're authorized to monitor.

---

