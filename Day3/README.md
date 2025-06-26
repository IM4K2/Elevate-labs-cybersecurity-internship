
# 🔍 Basic Vulnerability Scan on Personal Computer

This repository documents a hands-on vulnerability assessment conducted on a personal computer using **Nessus Essentials**. It highlights how to discover, interpret, and mitigate common system vulnerabilities from a beginner-friendly standpoint.

---

## 🧑‍💻 Project Overview

Vulnerability scanning is a core activity in cybersecurity, aimed at identifying weaknesses in systems that could be exploited. In this project, a complete scan was executed on the local host machine using the **Nessus Essentials** scanner. The scan provided insights into misconfigurations, outdated services, and insecure protocols.

---

## 🎯 Objective

- Perform a vulnerability scan on a local computer
- Identify and document **critical** and **high** vulnerabilities
- Suggest beginner-level remediations
- Understand the real-world implications of common weaknesses

---

## 🛠️ Tools Used

| Tool              | Description                                 |
|-------------------|---------------------------------------------|
| Nessus Essentials | Free vulnerability scanner by Tenable       |
| Localhost         | Target system (`127.0.0.1`)                 |
| Web Browser       | Accessed Nessus Dashboard (`https://localhost:8834`) |

---

## 🧪 Project Steps

1. Installed Nessus Essentials and registered with the free license key
2. Created a basic network scan targeting `127.0.0.1`
3. Launched the scan and monitored progress (took ~50 minutes)
4. Analyzed the scan report to filter important vulnerabilities
5. Verified each issue with official CVE documentation
6. Suggested beginner-level mitigations for identified vulnerabilities
7. Documented findings and included relevant screenshots in the report

---

## 📋 Key Findings (Summary)

| Vulnerability                        | Severity | CVE ID         | CVSS Score | Suggested Fix                        |
|-------------------------------------|----------|----------------|------------|--------------------------------------|
| SMBv1 Enabled                       | Critical | CVE-2017-0144  | 9.3        | Disable SMBv1 protocol in Windows    |
| Outdated OpenSSH Server            | High     | CVE-2023-48795 | 8.5        | Update OpenSSH to latest version     |
| SSL Certificate Expired            | Medium   | CVE-2022-3859  | 6.8        | Renew or replace expired certificate |
| HTTP TRACE Method Enabled          | Medium   | CVE-2004-2320  | 5.8        | Disable TRACE method on the server   |
| Open Port Without Service Firewall | Info     | -              | -          | Restrict unused open ports           |

---


## 🧠 Lessons Learned

- Legacy protocols like SMBv1 pose severe threats and should be disabled
- Expired certificates and TRACE methods are common, easy-to-overlook issues
- Even localhost systems can expose real vulnerabilities worth addressing
- Vulnerability assessment teaches both technical and security thinking skills

---

## 🔐 Disclaimer

This scan was run on a personal, non-production system for educational purposes only. The techniques and results may vary based on the system configuration, OS version, and installed software.

---
