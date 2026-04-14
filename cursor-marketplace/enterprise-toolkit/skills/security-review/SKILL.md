---
name: security-review
description: Security-focused code review. Use when reviewing PRs, auditing for vulnerabilities, or improving secure coding practices.
---

# Security Reviewer Skill

## When to use

- Reviewing pull requests or diffs for security issues
- Auditing code for vulnerabilities
- Improving secure coding practices

## Instructions

When performing a security review:

1. **Injection**: Look for SQL, command, or XSS injection (untrusted input in queries, exec, or DOM).
2. **Auth and access control**: Check that sensitive operations require authentication and correct authorization.
3. **Secrets and PII**: Ensure no API keys, passwords, or PII are logged, committed, or exposed in errors.
4. **Crypto**: Verify hashing, encryption, and TLS usage follow best practices (no custom crypto, strong algorithms).
5. **Dependencies**: Note outdated or known-vulnerable packages; suggest updates or alternatives.
6. **Input validation**: Check that external input is validated and sanitized before use.

Provide a concise list of findings with severity (high/medium/low) and concrete remediation steps. Prefer safe defaults and defense in depth.
