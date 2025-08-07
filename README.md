# CyberSecurity_Task_3

## Task: Perform a Basic Vulnerability Scan on Your PC
### 🛠 Tool Used: OpenVAS 


## Objective

To identify potential vulnerabilities on my local machine using a free vulnerability scanner and understand risk levels, CVEs, and basic remediation steps.


## Tools & Setup

- **Scanner Used**: [OpenVAS (Greenbone Vulnerability Manager) / Nessus Essentials]
- **Platform**: Kali Linux / Windows 10 / Other (mention your OS)
- **Target**: My own system (localhost / local IP)


## Steps Followed

1. Installed and configured the scanner.
2. Created a full system scan task.
3. Ran the scan on `127.0.0.1` or my local IP.
4. Waited for the scan to complete (~30 mins).
5. Analyzed vulnerabilities by severity and CVE ID.
6. Researched top critical vulnerabilities.
7. Took relevant screenshots of the scan report.

---

## Key Vulnerabilities Found

| CVE ID         | Title                                | Severity | Description                              | Fix/Recommendation                        |
|----------------|--------------------------------------|----------|------------------------------------------|-------------------------------------------|
| CVE-2022-XXXXX | SMBv1 Enabled                        | High     | Legacy protocol can be exploited remotely| Disable SMBv1 via system config           |
| CVE-2021-YYYYY | Outdated OpenSSL Version             | Medium   | May allow man-in-the-middle attack       | Upgrade to the latest OpenSSL version     |
| CVE-2023-ZZZZZ | Unpatched Browser Vulnerability      | High     | Can allow remote code execution          | Update browser / disable vulnerable plugin|

---

## Screenshots

All screenshots of the scan setup, results, and CVEs are in the `screenshots/` folder.

---

## Learnings

- Understood how vulnerability scanners identify risks.
- Learned about CVSS scores and how to prioritize issues.
- Explored the difference between scanning vs. penetration testing.


