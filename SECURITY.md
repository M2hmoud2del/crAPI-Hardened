# Security Policy

## Supported Versions

Currently, the project is actively maintaining and reviewing vulnerabilities on the `main` branch. Older releases will be evaluated on a case-by-case basis.

| Version | Supported          |
| ------- | ------------------ |
| `main`  | :white_check_mark: |
| < 1.0.0 | :x:                |

## Reporting a Vulnerability

**Please do not report security vulnerabilities through public GitHub issues.** (For a typical project, you would email security@example.com, but since this is a community hardening project, please use the provided [Vulnerability Report Template](.github/ISSUE_TEMPLATE/vulnerability_report.md) or use GitHub Security Advisories if enabled).

If using the GitHub Issue system for this project:
1. Navigate to the **Issues** tab.
2. Select **New Issue**.
3. Choose the **Vulnerability Report** template.
4. Fill out the required details including Summary, Steps to Reproduce, PoC, and Impact.

### What to Include in a Report
To help us quickly validate the issue, please ensure your report contains:
* A clear and concise description of the vulnerability.
* The exact version or commit hash where you observed the issue.
* Step-by-step instructions to reproduce the vulnerability.
* A Proof of Concept (PoC).
* Any relevant screenshots, logs, or network requests/responses.
* The potential security impact (e.g., Data Exfiltration, Privilege Escalation).

### Validation and Disclosure Process
1. **Triage:** The maintainer will acknowledge receipt of your vulnerability report within 48 hours.
2. **Validation:** We will attempt to reproduce the issue using your provided steps. We may ask for clarification.
3. **Remediation:** A fix will be developed. No code changes will be made publicly until the fix is ready for release.
4. **Recognition:** Upon successful validation, you will be credited in our [Hall of Fame](HALL_OF_FAME.md) and the next [Release Changelog](CHANGELOG.md).
5. **Disclosure:** Once the fix is released, the vulnerability details will be documented and published for educational purposes in `/docs/fixes/`.

### Rules of Engagement
* **Duplicate Reports:** If multiple researchers report the same vulnerability, the first valid submission will receive the "First Blood" recognition.
* **False Positives:** Reports that are determined to be intended behavior or not a security risk will be closed with an explanation.
* **Destructive Testing:** Please test responsibly. Do not perform actions that could cause data destruction, denial of service, or impact other users.

Thank you for helping to improve the security of crAPI-Hardened!
