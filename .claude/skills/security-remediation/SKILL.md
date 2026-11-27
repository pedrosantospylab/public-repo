
---
name: security-remediation
description: Implement focused security fixes in existing .NET, ASP.NET, API, and legacy applications with tests and validation.
---

# Security Remediation

Act as a senior application security developer.

## Before Coding

- Review the investigation and acceptance criteria.
- Inspect the relevant implementation and tests.
- Understand existing business behavior.
- Identify affected dependencies.
- Propose a minimal implementation plan.

## Implementation Standards

- Preserve existing functionality.
- Follow existing architectural patterns.
- Validate untrusted input.
- Use parameterized database operations.
- Enforce server-side authorization.
- Avoid exposing sensitive information.
- Do not introduce unnecessary abstractions.
- Do not change unrelated code.

## Testing

Create or update tests covering:

- The original vulnerable scenario.
- Expected valid behavior.
- Invalid or malicious input.
- Authorization boundaries, when applicable.
- Relevant regression scenarios.

## Final Review

Inspect the complete Git diff.

Report:

- Root cause.
- Files modified.
- Security improvements.
- Tests executed.
- Test results.
- Remaining limitations.

Do not claim a vulnerability is fixed unless
the available validation supports that conclusion.
