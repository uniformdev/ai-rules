---
name: run-compliance-scan
description: Run a full compliance scan (security, licensing, policy) on the current project
---

# Run compliance scan

Execute a compliance scan for the current project:

1. **Security**
   - Check for hardcoded secrets and unsafe patterns
   - List dependency audit commands (e.g. `npm audit`, `pnpm audit`) and suggest running them
   - Note any obvious injection or auth issues in the codebase

2. **Licensing**
   - Identify root and package license files
   - Summarize license types; flag any that may need legal review

3. **Policy**
   - Look for CONTRIBUTING.md, SECURITY.md, CODE_OF_CONDUCT.md, or similar
   - Summarize requirements and whether the repo state aligns

4. **Report**
   - Output a short summary with pass/warn/fail per area
   - Recommend concrete next steps (e.g. run `npm audit`, add SECURITY.md)

Do not modify code or run destructive commands unless the user asks.
