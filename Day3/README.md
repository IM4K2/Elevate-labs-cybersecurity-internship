# 🔍 Localhost Vulnerability Assessment Using Nessus Essentials

This repository presents a basic vulnerability scan conducted on a personal computer using **Nessus Essentials**. The purpose of this assessment was to explore, interpret, and learn from real-world system vulnerabilities from a beginner's perspective.

---

## 🧑‍💻 Overview

Vulnerability scanning plays a key role in strengthening system security. By identifying known weaknesses, one can proactively address them before they are exploited. In this task, a complete scan was carried out on the local machine (localhost) using the free version of Nessus Essentials to detect threats and evaluate their severity.

---

## 🎯 Goals

- Run a basic vulnerability scan on the local PC
- Detect and log significant (high/critical) vulnerabilities
- Recommend simple mitigation strategies
- Build familiarity with vulnerability management tools

---

## 🛠️ Tools & Environment

| Tool              | Purpose                                      |
|-------------------|----------------------------------------------|
| Nessus Essentials | Free scanner from Tenable used for scanning  |
| 127.0.0.1         | Target IP (represents the local system)      |
| Web Browser       | Used to access the Nessus interface (`https://santhohex:8834`) |

---

## 🧪 Procedure

1. Installed Nessus Essentials and completed the free license activation.
2. Set up a new scan profile aimed at the localhost IP (`127.0.0.1`).
3. Initiated a basic scan of the system.
4. Monitored the scan, which took approximately 45 minutes to complete.
5. Reviewed the scan findings and highlighted major issues.
6. Investigated each vulnerability to understand its risk and resolution.
7. Compiled a summary report with fixes and captured screenshots.

---

## 📋 Summary of Detected Vulnerabilities

| Vulnerability                   | Risk Level | CVE Reference   | CVSS Rating | Suggested Action                    |
|--------------------------------|------------|------------------|-------------|-------------------------------------|
| SMB Signing Disabled           | High       | CVE-2017-0143    | 8.1         | Enable mandatory SMB signing        |
| Firefox Browser Outdated       | Medium     | CVE-2023-5381    | 6.5         | Update Firefox to the latest build  |
| Weak SSL/TLS Cipher Support    | Medium     | CVE-2016-2183    | 5.9         | Disable legacy SSL cipher suites    |
| ICMP Timestamp Disclosure      | Informational | -            | -           | Block timestamp replies via firewall |

---

## 📁 Project Contents

- `/report/`: Contains a detailed summary of the scan and analysis
- `/screenshots/`: Includes visuals of vulnerabilities and scan output
- `README.md`: Documentation of project process and key learnings

---

## 🧠 Key Takeaways

- Even a standalone personal machine can present exploitable vulnerabilities.
- Outdated applications and misconfigured protocols pose real security threats.
- Tools like Nessus offer valuable insights and learning opportunities for beginners.
- Security is a continuous process — regular scans and updates are essential.

---

## ⚠️ Disclaimer

The assessment was carried out solely for educational and training purposes on a personal, non-production system. Vulnerability behavior may differ based on system settings and installed software.

---
