## Task 9: Cryptography Fundamentals

**Overview:** Cryptography underpins confidentiality, integrity, and authentication across all security tools.

**Why it matters:** Almost every security control you'll ever configure — HTTPS, VPNs, disk encryption, password hashing, digital signatures — is built on top of a small set of cryptographic primitives. Once you understand the difference between encryption (reversible, needs a key) and hashing (one-way, used for verification), a lot of "magic" in security tools suddenly makes sense, and you become much better at spotting when crypto is being used incorrectly (e.g., a weak cipher, a missing salt, an expired certificate).

**Key Concepts:**
- Symmetric encryption (AES) vs asymmetric encryption (RSA)
- Hashing (SHA-256) vs encryption — hashing is one-way, encryption is reversible with a key
- Digital signatures and certificates (SSL/TLS)

**Common Tools:**
- OpenSSL, GPG

**Example:**
```bash
# Generate an RSA key pair
openssl genrsa -out private.pem 2048
openssl rsa -in private.pem -pubout -out public.pem

# Encrypt a file symmetrically
openssl enc -aes-256-cbc -in file.txt -out file.enc
```

**Note:** Understanding *why* HTTPS/TLS works (certificate chain, handshake) ties directly into web security testing later.

---

