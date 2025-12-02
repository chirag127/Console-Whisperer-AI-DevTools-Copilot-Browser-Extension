# Security Policy for Console Whisperer AI DevTools Copilot Browser Extension

As the Apex Technical Authority, we treat security as a non-negotiable aspect of our development lifecycle, adhering to Zero-Defect principles.

## 1. Overview & Philosophy

This repository, built upon TypeScript, Vite, and designed for direct integration within browser DevTools, handles sensitive runtime data. Therefore, security is paramount. We follow the principle of **Least Privilege** for all browser APIs utilized and maintain strict dependency hygiene.

## 2. Supported Versions

We only actively support the latest stable release branch of the extension. Security patches for older major versions are not guaranteed.

| Version | Status | Supported Until |
| :--- | :--- | :--- |
| v1.x.x (Current) | Active Support | Ongoing |

## 3. Reporting a Vulnerability

If you discover any security vulnerability within this project, please follow these steps immediately. **DO NOT** open a public issue until the vulnerability has been responsibly disclosed and remediated by the core team.

**Responsible Disclosure Timeline:**

1.  **Initial Report (Private):** Immediately email the security contact below with a detailed description of the vulnerability, including proof-of-concept steps, affected files, and potential impact.
2.  **Triage & Acknowledgement:** We will acknowledge receipt within 48 hours.
3.  **Remediation:** The Apex team will prioritize patching based on severity (Critical > High > Medium > Low).
4.  **Public Disclosure:** We will coordinate a public disclosure timeline with you once the patch is released.

### Security Contact

Please direct all security-related communications to:

**Email:** `security+console-whisperer@chirag127.dev`

## 4. Vulnerability Disclosure & Severity Scoring

Reported vulnerabilities will be scored using the Common Vulnerability Scoring System (CVSS) version 3.1. Severity mapping for internal triage is as follows:

*   **Critical (9.0 - 10.0):** Remote Code Execution (RCE), Privilege Escalation, Data Exfiltration bypassing standard browser sandboxing.
*   **High (7.0 - 8.9):** Sensitive data leakage via logs/telemetry, Cross-Site Scripting (XSS) vector within the DevTools overlay.
*   **Medium (4.0 - 6.9):** Denial of Service (DoS) vector impacting DevTools performance, unauthorized configuration changes.
*   **Low (0.1 - 3.9):** Informational findings, minor XSS that requires user interaction outside of normal extension workflow.

## 5. Automated Security Scanning

This repository employs automated security checks integrated into the CI/CD pipeline (`.github/workflows/ci.yml`):

*   **Dependency Scanning:** We utilize **Snyk** (via GitHub Actions integration) to continuously monitor for known vulnerabilities in npm/Node dependencies (targeting TypeScript/JavaScript ecosystem risks).
*   **Static Analysis:** **Biome** is configured not only for formatting but also for catching common anti-patterns that could lead to security issues (e.g., unsafe usage of `eval` or unchecked inputs).

## 6. Development Security Practices

All developers contributing to this project must adhere to the following:

1.  **Input Validation:** All data received from the browser context or external APIs **MUST** be treated as untrusted and rigorously sanitized before rendering or processing.
2.  **Content Security Policy (CSP):** The extension's manifest rigorously defines a restrictive CSP to prevent unauthorized resource loading.
3.  **API Key Management:** All secrets (e.g., AI provider keys) are stored securely in GitHub Secrets and are **never** hardcoded or committed.
4.  **Dependency Review:** All `package.json` dependencies are reviewed for age, license compatibility, and known security advisories before being merged into the main branch.