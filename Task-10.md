## Task 10: Web Application Security Testing

**Overview:** Web apps are a major attack surface. This covers finding and understanding common web vulnerabilities.

**Why it matters:** Web applications are usually the most exposed part of any organization — reachable by anyone on the internet, updated constantly, and often built by combining many third-party libraries. The OWASP Top 10 exists because the same handful of mistakes (unsanitized input, broken access control, poor session handling) keep showing up across countless real breaches. Practicing against intentionally vulnerable apps builds the pattern recognition needed to spot these issues in real code and real traffic.

**Key Concepts:**
- OWASP Top 10 (SQL Injection, XSS, CSRF, Broken Auth, etc.)
- Intercepting and modifying requests
- Input validation and output encoding as defenses

**Common Tools:**
- Burp Suite, OWASP ZAP, DVWA (Damn Vulnerable Web App) for practice

**Example concept (defensive):**
```text
Input:  ' OR '1'='1
Vulnerable query: SELECT * FROM users WHERE username='' OR '1'='1'
Fix: Use parameterized queries / prepared statements
```

**Note:** Always test against intentionally vulnerable practice apps (DVWA, bWAPP, Juice Shop) — never against live/public sites.

---

