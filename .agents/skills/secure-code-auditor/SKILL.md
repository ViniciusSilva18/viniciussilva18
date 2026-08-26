---
name: secure-code-auditor
description: >-
  Audits and hardens codebases against security vulnerabilities, OWASP Top 10,
  data leakage, and misconfigurations. Use during development and code review to
  guarantee zero vulnerabilities and production-grade security.
---

# Secure Code Auditor & Security Hardening

Expert skill for reviewing, auditing, and hardening web applications, APIs, and scripts against common vulnerabilities and security pitfalls.

## Core Security Rules

### 1. Secret and Credential Protection
- **NEVER** hardcode API keys, database credentials, passwords, JWT secrets, or private tokens in source code.
- Always use environment variables (`.env`) loaded via `dotenv` (Node) or `python-dotenv` (Python).
- Add `.env`, `*.pem`, `*.key`, `*.secret`, and build artifacts to `.gitignore` before initial commit.

### 2. Input Sanitization & Injection Prevention
- **SQL Injection**: Always use parameterized queries or trusted ORMs (e.g. Prisma, Drizzle, SQLAlchemy, SQLite parameterized `?` or `%s`). Never concatenate user input into raw SQL strings.
- **XSS (Cross-Site Scripting)**: Sanitize and escape all user inputs rendered in HTML/DOM. Use `textContent` instead of `innerHTML` or use DOMPurify when rendering markdown/rich text.
- **Path Traversal**: Validate and normalize file paths with `path.resolve` / `os.path.abspath` and ensure they remain within safe directories.

### 3. API Security & Headers
- Configure secure HTTP headers (Helmet in Express / CORS settings).
- Restrict CORS origins instead of using wildcards `*` in production endpoints.
- Enforce Rate Limiting to prevent brute-force attacks and DDoS.
- Use secure cookies (`HttpOnly`, `Secure`, `SameSite=Strict`).

### 4. Dependency Safety
- Run security audits (`npm audit`, `pip-audit`) to detect known CVEs in third-party libraries.
- Avoid obsolete or unmaintained dependencies.
