# Fintech App Security Checklist (OWASP Mobile Top 10)

> Created by [TrustGrid Technology Limited](https://trustgridhq.com) — App Security & Compliance Consulting.
> Based on OWASP Mobile Security Testing Guide (MSTG) and OWASP Mobile Top 10.

---

## 1. Improper Credential Usage (M1)

- [ ] No hardcoded credentials, API keys, or secrets in source code
- [ ] No credentials stored in plain text in shared preferences or local storage
- [ ] API keys restricted by platform (iOS Keychain / Android Keystore)
- [ ] Service account credentials rotated regularly
- [ ] Environment variables used for sensitive configuration

---

## 2. Inadequate Supply Chain Security (M2)

- [ ] All third-party SDKs reviewed for security and privacy implications
- [ ] SDK versions pinned and regularly updated
- [ ] Software Bill of Materials (SBOM) maintained
- [ ] Third-party SDKs sourced from official repositories only
- [ ] Open source dependencies scanned for known vulnerabilities

---

## 3. Insecure Authentication & Authorization (M3)

- [ ] Strong authentication implemented (OAuth 2.0 / OIDC)
- [ ] Multi-factor authentication available for high-risk actions
- [ ] Session tokens are sufficiently random and long
- [ ] Session tokens expire after inactivity
- [ ] Re-authentication required for sensitive operations (transfers, password change)
- [ ] Authorization checks performed server-side, not client-side only

---

## 4. Insufficient Input/Output Validation (M4)

- [ ] All user inputs validated and sanitised on server-side
- [ ] SQL injection prevention implemented
- [ ] No sensitive data displayed in error messages
- [ ] File uploads validated for type, size, and content
- [ ] Output encoding applied to prevent XSS in WebViews

---

## 5. Insecure Communication (M5)

- [ ] All network communication uses HTTPS/TLS 1.2 or higher
- [ ] Certificate pinning implemented for critical API endpoints
- [ ] No HTTP fallback permitted
- [ ] TLS certificate validity checked
- [ ] No sensitive data passed in URL parameters

---

## 6. Inadequate Privacy Controls (M6)

- [ ] Minimum data collected (data minimisation principle)
- [ ] Sensitive data not logged to console or crash logs
- [ ] Sensitive data not stored in app screenshots/backgrounding cache
- [ ] Clipboard access restricted for sensitive fields
- [ ] Screen recording/screenshot prevention implemented for sensitive screens
- [ ] Keyboard cache disabled for sensitive input fields

---

## 7. Insufficient Binary Protections (M7)

- [ ] Code obfuscation applied to production build
- [ ] Anti-tampering controls implemented
- [ ] Root/jailbreak detection implemented
- [ ] Debugger detection implemented
- [ ] App integrity verified at runtime

---

## 8. Security Misconfiguration (M8)

- [ ] Debug mode disabled in production build
- [ ] Unnecessary permissions removed from manifest
- [ ] Backup disabled for sensitive data (Android)
- [ ] WebView JavaScript interface restricted
- [ ] Firebase/cloud services access rules properly configured
- [ ] Default credentials changed on all integrated services

---

## 9. Insecure Data Storage (M9)

- [ ] No sensitive data stored in plain text on device
- [ ] iOS Keychain / Android Keystore used for credentials and tokens
- [ ] Database files encrypted
- [ ] Temporary files containing sensitive data deleted after use
- [ ] External storage not used for sensitive data
- [ ] Sensitive data excluded from device backups

---

## 10. Insufficient Cryptography (M10)

- [ ] Strong encryption algorithms used (AES-256, RSA-2048+)
- [ ] No deprecated algorithms (MD5, SHA-1, DES)
- [ ] Encryption keys stored securely, not hardcoded
- [ ] Random number generation uses cryptographically secure functions
- [ ] Key rotation policy defined and implemented

---

## Fintech-Specific Additional Checks

- [ ] Transaction signing implemented for financial operations
- [ ] Amount and recipient confirmation step before transaction execution
- [ ] Transaction limits enforced server-side
- [ ] Fraud detection integrated for unusual transaction patterns
- [ ] API rate limiting implemented to prevent abuse
- [ ] IDOR (Insecure Direct Object Reference) prevented on account endpoints
- [ ] Admin and customer endpoints properly separated and authenticated

---

## Risk Rating Summary

After completing this checklist, rate each finding:

| Rating | Description |
|--------|-------------|
| Critical | Must fix before launch — immediate security risk |
| High | Should fix before launch — significant vulnerability |
| Medium | Fix within 30 days of launch |
| Low | Fix within 90 days of launch |
| Informational | Best practice recommendation |

---

*Created by [TrustGrid Technology Limited](https://trustgridhq.com). For a full mobile app security audit, visit our [Fiverr service page](https://www.fiverr.com/s/WE5jVGR).*
