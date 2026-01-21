# Security Policy

Security matters. If you discover a vulnerability, we appreciate responsible disclosure.

## Reporting a vulnerability (preferred process)

1. **Do not open a public issue** or post details publicly.
2. Report it privately using the contact route in **SUPPORT.md**:
    - https://www.cyborgcode.io/contact
3. Include enough detail for us to reproduce and assess impact.

## Subject line tagging (recommended)

When contacting us, please prefix the subject/title to help routing:

- **[SECURITY]** <short summary>
- **[SECURITY][ROA]** <short summary> (if you know the ecosystem)
- **[SECURITY][REPO:<name>]** <short summary> (if you know the repo)

Example:
- **[SECURITY][REPO:roa-plugins]** Deserialization issue in distributed runner

## What to include

Please provide:
- A clear description of the issue and why it is a security risk
- Affected repository/module and **affected version(s)** (or commit hash)
- Reproduction steps or a minimal proof-of-concept
- Impact assessment (what an attacker can do)
- Any suggested mitigation or patch (optional)

**Do not include secrets** (tokens, private keys, credentials). If sensitive data is required to reproduce, redact it or describe it.

## Scope

This policy applies to security vulnerabilities in:
- Code and workflows maintained in this GitHub organization
- Released artifacts and their build/release pipelines

Issues caused by downstream usage, misconfiguration, or third-party dependencies may be addressed as guidance or documented mitigations, at our discretion.

## Coordinated disclosure

Please allow reasonable time for investigation and remediation before public disclosure.
We may request an embargo period to protect users while a fix is prepared and released.

## Handling and outcomes

We aim to:
- Acknowledge receipt of your report
- Confirm whether the issue is in scope
- Work on a mitigation or fix when appropriate

Remediation approach, timelines, and publication decisions are determined by the project maintainers and administrators.

## Bug bounty

We do not currently operate a paid bug bounty program.
