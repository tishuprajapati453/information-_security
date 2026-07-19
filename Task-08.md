## Task 8: Password Security and Authentication

**Overview:** Weak authentication is one of the most common real-world breach causes. This topic covers how passwords are stored, verified, and strengthened — not how to break into accounts you don't own.

**Why it matters:** Study after study shows that stolen or guessed credentials are involved in the majority of breaches — far more often than exotic exploits. Understanding the difference between a system that stores passwords safely (salted, slow hashes like bcrypt/argon2) versus one that stores them dangerously (plaintext or fast unsalted hashes) is one of the highest-impact things you can evaluate in any security review. Layering in MFA is often the single most effective control against account takeover.

**Key Concepts:**
- Hashing vs encryption for password storage
- Salting to prevent rainbow-table attacks
- Multi-factor authentication (MFA)
- Password policies (length, complexity, rotation trade-offs)

**Common Tools (defensive/educational context):**
- `openssl` for hashing demonstrations
- Password managers, MFA apps (Authy, Google Authenticator)

**Example (hash demonstration only):**
```bash
echo -n "MySecurePass123" | sha256sum
```

**Note:** Focus your study on *how* to defend systems — enforcing MFA, strong hashing (bcrypt/argon2), and account lockout policies.

---

