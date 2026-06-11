# Security Policy

*Org-wide default; per-repo `SECURITY.md` overrides.*

**Do not report security vulnerabilities in a public issue, PR, or discussion.**

## Reporting

Report privately via **GitHub's private vulnerability reporting** — open the
repository's **Security → Report a vulnerability** form (GitHub Security
Advisories). Each repo may have its own advisory intake; this org-level file
is the fallback.

If the repository you're reporting against lacks its own `SECURITY.md`, it
inherits this default.

## What to include

- Affected repo and commit/branch (or `VERSION` if applicable).
- A description of the vulnerability and its impact.
- Steps to reproduce (minimal PoC if possible).
- **Never include real secrets, credentials, cluster IPs/DNS, or operator
  identity** — use placeholders.

## Disclosure

We work with reporters on a coordinated-disclosure timeline and credit them
(if requested) in the advisory and release notes. Acknowledgement within
5 business days.

## Supported versions

This project is pre-1.0 prototype — no released versions are formally
supported. Reproduce against the current `main` tip before reporting.
