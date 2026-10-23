🛡️ ReleaseShield AI

AI-Powered DevSecOps Security Analysis Platform

ReleaseShield AI is a DevSecOps platform designed to improve software security by integrating multiple security scanning tools, consolidating findings, reducing duplicate alerts, and providing actionable security insights.

Developed as part of the EPAM CoE Project.

🚀 Overview

Modern software development pipelines generate security findings from multiple tools. ReleaseShield AI aims to simplify security analysis by normalizing findings, identifying duplicates, mapping code ownership, and helping developers understand potential vulnerabilities.

✨ Key Features

- Multi-Tool Security Scanning: Integrates multiple security tools for vulnerability detection.
- Finding Normalization: Standardizes findings from different security scanners.
- Intelligent Deduplication: Identifies duplicate findings to reduce alert noise.
- AI-Assisted Explanations: Helps developers understand security findings and remediation options.
- Code Ownership Mapping: Uses GitHub CODEOWNERS to identify responsible teams.
- Security Dashboard: Provides a centralized view of security analysis results.
- GitHub Integration: Supports repository and pull request security analysis.

🧰 Technology Stack

Technology| Purpose
Trivy| Vulnerability and dependency scanning
Semgrep| Static Application Security Testing (SAST)
OWASP ZAP| Dynamic Application Security Testing (DAST)
Gitleaks| Secret detection
SARIF 2.1.0| Standardized security result reporting
Git & GitHub| Version control and repository integration

⚙️ Workflow

1. Scan the codebase using supported security tools.
2. Collect and normalize security findings.
3. Identify duplicate findings using fingerprints and metadata.
4. Map findings to code ownership where possible.
5. Generate explanations and consolidated reports.
6. Review findings and prioritize remediation.

🎯 Project Objectives

- Reduce duplicate security alerts.
- Improve visibility into vulnerabilities.
- Simplify security reviews during development.
- Help developers prioritize remediation.
- Strengthen security throughout the software development lifecycle.

👨‍💻 Maintainer

Krishna Kumar

GitHub: "@Krishna-1551" (https://github.com/Krishna-1551)

🤝 Acknowledgements

This repository is based on the original EPAM CoE project by "Team-Algorithm" (https://github.com/Team-Algorithm/ReleaseSheild_EPAM-Project).

Credit goes to the original project contributors. Please refer to the original repository for its history and licensing information.

📌 Project Status

Ongoing development of a DevSecOps security analysis platform with security finding normalization, deduplication, and AI-assisted insights.

---

Building safer software through intelligent security automation.
