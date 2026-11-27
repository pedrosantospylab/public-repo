# AI-Assisted Application Security Remediation

A demonstration environment for AI-assisted security investigation, code remediation, and validation using Claude Code.

## Objectives

Demonstrate a structured engineering workflow for identifying and remediating common application security vulnerabilities in enterprise applications.

## Technologies

- C# / .NET
- ASP.NET Core
- SQL Server / T-SQL concepts
- Classic ASP / VBScript
- Angular
- PostgreSQL (local sandbox)
- Claude Code
- Agent Skills

## AI Engineering Approach

The repository uses specialized Claude Code skills to support:

- Security finding investigation and root-cause analysis.
- Secure code implementation and remediation.
- SQL injection and database security reviews.
- Classic ASP and VBScript legacy application analysis.
- Test generation and validation.

## Engineering Principles

- Human-reviewed AI-generated changes.
- Minimal and focused remediation.
- Least-privilege database access.
- Parameterized database operations.
- Regression testing.
- Explicit validation and remediation evidence.

## Database Environment

A local PostgreSQL database is provided as a disposable sandbox for database investigation and testing.

It does not represent a production environment or replace SQL Server-specific validation.

## Security Notice

This repository is intended for educational and interview demonstration purposes. Never use production credentials, customer data, or unrestricted database permissions in this environment.