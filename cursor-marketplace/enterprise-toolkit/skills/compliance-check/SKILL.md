---
name: compliance-check
description: Run compliance checks for security, licensing, and policy. Use when auditing a codebase, before releases, or when asked about compliance or policy.
---

# Compliance Check Skill

## When to use

- Auditing a codebase for security or policy compliance
- Before releases or merge to main
- When the user asks about compliance, licensing, or policy

## Instructions

1. **Security**: Scan for hardcoded secrets, unsafe dependencies, and obvious injection or auth issues. Suggest fixes or follow-up tools (e.g. npm audit, secret scanning).
2. **Licensing**: Note any license files or package metadata. Flag incompatible or unclear licenses if the user cares about license compliance.
3. **Policy**: If the project has a CONTRIBUTING, SECURITY, or policy doc, summarize requirements and check whether the current change aligns.
4. **Reporting**: Summarize findings in a short report (pass/warn/fail per area). Recommend concrete next steps.

Do not run destructive or invasive commands unless the user explicitly requests them.
