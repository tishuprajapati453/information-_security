## Task 15: Security Audit and Best Practices

**Overview:** Regular audits verify that security controls are actually working as intended, not just documented on paper.

**Why it matters:** Policies and configurations tend to drift over time — a firewall rule added "temporarily" two years ago, a patch that never got applied, an account that should have been disabled. Regular audits against a recognized framework (CIS, NIST, ISO 27001) catch this drift before it becomes a breach, and they force an organization to prove its security posture with evidence rather than assumptions. This topic ties together everything else in the guide into a single repeatable process of continuous improvement.

**Key Concepts:**
- Compliance frameworks (ISO 27001, NIST, CIS Benchmarks)
- Configuration review vs penetration testing
- Continuous improvement cycle

**Common Tools:**
- CIS-CAT, Lynis (Linux auditing tool)

**Example:**
```bash
# Run a basic Linux security audit
sudo apt install lynis -y
sudo lynis audit system
```

**Best Practices Checklist:**
- Keep systems and software patched
- Enforce least-privilege access
- Use strong authentication (MFA)
- Maintain and review logs regularly
- Have a tested incident response plan
- Document every change and finding


