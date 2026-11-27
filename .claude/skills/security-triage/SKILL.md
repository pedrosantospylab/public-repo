
---
name: security-triage
description: Investigate application security findings, trace vulnerable data flows, identify root causes, and prepare remediation plans before coding.
---

# Security Finding Investigation

Act as an application security engineer investigating
a security scanner finding.

## Workflow

1. Read the complete finding and acceptance criteria.
2. Identify the affected files, methods, and components.
3. Trace the input from its source to its final use.
4. Identify trust boundaries and user-controlled data.
5. Inspect relevant dependencies and downstream behavior.
6. Determine whether the finding is exploitable.
7. Identify the actual root cause.
8. Distinguish confirmed vulnerabilities from false positives
   or findings requiring additional investigation.

## Output

Provide:

- Finding summary.
- Vulnerable code location.
- Source of untrusted input.
- Data flow and execution path.
- Root cause.
- Potential impact.
- Recommended remediation.
- Suggested regression tests.
- Confidence level and unresolved questions.

Do not modify code during triage unless explicitly requested.
Never dismiss a finding without supporting evidence.
