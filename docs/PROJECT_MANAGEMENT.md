# Project Management Guidelines

This document provides internal guidelines for the maintainers of crAPI-Hardened on how to manage the repository, issues, and releases.

## Labels
Ensure the following labels are created in the GitHub repository to manage issues and PRs effectively:
- `security`: For confirmed vulnerability reports.
- `critical`, `high`, `medium`, `low`: For vulnerability severity.
- `duplicate`: For reports of already known issues.
- `confirmed`: When a vulnerability is validated.
- `under review`: For new reports being analyzed.
- `fixed`: When a fix is deployed in the latest release.
- `documentation`: For docs-only changes.
- `community`: For questions, ideas, or community discussions.
- `hall-of-fame-eligible`: To track users who need to be added to `HALL_OF_FAME.md`.

## GitHub Discussions
Enable GitHub Discussions in the repository settings and create the following categories:
- **Announcements**: For maintainer updates and new releases.
- **General**: For general chatter about API security.
- **Q&A**: For troubleshooting setup and deployment issues.
- **Security Research**: For discussing exploitation techniques and security testing tools.
- **Ideas**: For proposing new hardening techniques.

## Releases and Versioning
We use [Semantic Versioning](https://semver.org/).
* **Major (X.0.0)**: Reserved for when the entire application is fully hardened (e.g., v1.0.0).
* **Minor (0.X.0)**: Incremented when a batch of vulnerabilities (e.g., an entire category like BOLA) is remediated.
* **Patch (0.0.X)**: Incremented for single vulnerability fixes, documentation updates, or minor bug fixes.

**Release Strategy:**
1. Maintainers fix vulnerabilities on the `main` branch or a `develop` branch.
2. A new release is drafted and tagged (e.g., `v0.1.0`).
3. Release notes are generated using the `CHANGELOG.md` format, heavily acknowledging the researchers who discovered the fixed issues.

## Documentation Structure
The `/docs/` directory is organized as follows:
- `/docs/fixes/`: Detailed writeups on how specific vulnerabilities were remediated.
- `/docs/writeups/`: Researcher-submitted Proofs of Concept (PoCs) and analysis.
- `/docs/releases/`: Detailed architectural diffs and notes for major releases.
- `/docs/security-review/`: Internal audits, threat models, and architecture reviews.
