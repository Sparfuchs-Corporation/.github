# Security Policy

Sparfuchs Corporation takes the security of our software and the agents it governs seriously. This policy applies to all public repositories under the [Sparfuchs-Corporation](https://github.com/Sparfuchs-corporation) organization.

## Reporting a Vulnerability

**Please do not file public GitHub issues for security vulnerabilities.** Public disclosure before a fix is available puts every user of the affected code at risk.

Instead, email **security@sparfuchs-pro.com** with:

- A description of the vulnerability and its potential impact
- Steps to reproduce, or a proof-of-concept if available
- The affected repository, version, or commit
- Your name and a preferred contact method (optional, for credit)

You can expect:

- **Acknowledgement within 2 business days** that we've received your report
- **An initial assessment within 5 business days** with our understanding of the issue and next steps
- **Regular updates** as we work on a fix
- **Credit in the release notes** once the fix ships, unless you prefer to remain anonymous

## Scope

This policy covers vulnerabilities in:

- Source code in any public Sparfuchs repository
- Official release artifacts and container images
- Documentation that could mislead users into insecure configurations
- Agent prompts, policies, and configuration defaults that ship with our platforms

Out of scope:

- Vulnerabilities in third-party dependencies (please report those upstream; we will track and update)
- Findings that require physical access to a user's machine
- Social engineering of Sparfuchs employees or contractors
- Denial-of-service attacks that require unrealistic traffic volumes

## Responsible Disclosure

We ask that you:

- Give us reasonable time to fix the issue before public disclosure (typically 90 days)
- Avoid accessing, modifying, or deleting data belonging to others
- Not run automated scanners against production Sparfuchs infrastructure

In return, we commit to treating your report seriously, fixing verified issues promptly, and crediting your contribution.

## Supported Versions

Each repository's `README.md` documents its supported versions. In general, we support:

- The latest major version (security and bug fixes)
- The previous major version (security fixes only, for a defined deprecation window)

## Questions

For questions about this policy that do not involve a specific vulnerability, email **hello@sparfuchs-pro.com**.

<sub>© 2026 Sparfuchs Corporation. All rights reserved.</sub>
