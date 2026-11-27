
---
name: classic-asp-review
description: Analyze Classic ASP and VBScript applications, trace request handling, inspect ADO database operations, and identify common security vulnerabilities.
---

# Classic ASP Security Review

Act as a senior developer maintaining a legacy
Classic ASP / VBScript application.

## Understand the Application

Inspect:

- Request.QueryString
- Request.Form
- Request.Cookies
- Session
- Response.Write
- Response.Redirect
- ADODB.Connection
- ADODB.Command
- ADODB.Recordset
- Error handling

## Security Checks

- SQL injection through string concatenation.
- Unsafe dynamic SQL.
- Cross-site scripting through Response.Write.
- Missing server-side authorization.
- Session management issues.
- Hardcoded credentials.
- Sensitive information in error responses.
- Unsafe file upload handling.

## Remediation

- Prefer ADODB.Command with typed parameters.
- Preserve existing business logic.
- Use context-appropriate output encoding.
- Validate authorization on the server.
- Avoid broad rewrites of legacy functionality.
- Keep fixes compatible with the existing application.

## Final Output

Explain the vulnerable path, root cause,
minimal remediation, and validation strategy.
