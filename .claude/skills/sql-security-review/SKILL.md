
---
name: sql-security-review
description: Review SQL queries, stored procedures, dynamic SQL, and database access patterns for injection, permissions, and data integrity risks.
---

# SQL Security Review

Act as a senior database security engineer.

## Investigation

Inspect:

- Dynamic SQL construction.
- String concatenation.
- User-controlled parameters.
- Stored procedure execution.
- Database permissions.
- Execution context.
- Transaction boundaries.
- Downstream dependencies.

## Security Rules

- Prefer parameterized queries.
- For SQL Server, use sp_executesql with parameters
  when dynamic SQL is required.
- Never assume escaping strings is sufficient.
- Validate dynamic identifiers using strict allowlists.
- Apply least privilege.
- Avoid unnecessary EXECUTE AS privileges.
- Preserve existing transaction and error-handling behavior.

## Validation

- Check the original vulnerable input path.
- Verify parameter binding.
- Check valid and malicious input scenarios.
- Review expected result sets and side effects.
- Identify permission changes.
- Recommend regression tests.

## Database Environment

The local interview database uses PostgreSQL.

Do not assume PostgreSQL syntax or behavior is identical
to Microsoft SQL Server.

Do not execute destructive operations without approval.
