# Networkwalks Week 4 – Mediroza General Hospital Penetration Testing Report

![Networkwalks Logo](images/networkwalks-logo.png)

## Project Overview

This repository contains my Week 4 cybersecurity assessment project for **Networkwalks**.

The project focuses on a black-box web application security assessment of **Mediroza General Hospital**, with the objective of reviewing the security posture of its public-facing web application, identifying potential weaknesses, assessing their security implications, and documenting appropriate remediation recommendations.

## Assessment Information

| Item | Details |
|---|---|
| Project | Week 4 – Penetration Testing |
| Organisation | Networkwalks |
| Batch | B083 |
| Assessor | Nizamaddeen Umar |
| Target | Mediroza General Hospital |
| Target Domain | `https://medirozahospital.com` |
| Assessment Type | Black-Box Web Application Security Assessment |
| Report Version | 1.0 – Final |

## Objectives

The main objectives of this assessment were to:

- Conduct reconnaissance of the target's public-facing infrastructure.
- Review the web application's externally observable security controls.
- Assess authentication and information-disclosure weaknesses.
- Examine potential exposure of sensitive files and documents.
- Evaluate the security implications of identified findings.
- Recommend appropriate remediation measures.
- Prepare a structured penetration testing report.

## Methodology

The assessment followed a phased security testing approach:

1. **Passive Reconnaissance** – Collection and review of publicly available domain and DNS information.
2. **Service and Application Review** – Examination of externally observable services and web application components.
3. **Vulnerability Assessment** – Review of authentication behaviour, file exposure, directory configuration and error handling.
4. **Evidence Review** – Documentation and assessment of relevant security observations.
5. **Reporting and Remediation** – Classification of findings and preparation of security recommendations.

## Tools and Technologies

The assessment report documents the use of the following tools and utilities:

- Nmap
- WHOIS
- Dig
- Nslookup
- WhatWeb
- WAFW00F
- Gobuster
- Burp Suite
- cURL
- John the Ripper
- ExifTool
- PDF analysis utilities
- Web browser inspection

## Summary of Reported Findings

The assessment report documents seven security findings:

| No. | Finding | Reported Severity |
|---|---|---|
| 1 | SQL Injection – Patient Portal Authentication | Critical |
| 2 | Exposed Database Backup File | Critical |
| 3 | Weak PDF Encryption Passwords | High |
| 4 | Sensitive Path Disclosure through robots.txt | Medium |
| 5 | Directory Listing Enabled | Medium |
| 6 | Username Enumeration on Login Form | Medium |
| 7 | Verbose SQL Error Messages | Low |

The report includes descriptions of the findings, their potential security impact, supporting evidence and recommended remediation measures.

## Key Security Recommendations

The report recommends:

- Using parameterised database queries.
- Securing sensitive files and database backups.
- Improving document encryption and password protection.
- Disabling unnecessary directory listings.
- Implementing consistent authentication error messages.
- Preventing detailed server errors from being displayed to users.
- Reviewing access controls and applying security monitoring.

## Repository Structure

```text
Networkwalks-Week4-Pentest/
│
├── images/
│   └── networkwalks-logo.png
│
├── report/
│   └── Mediroza_Penetration_Test_Report.pdf
│
└── README.md
```

## Learning Outcomes

This project provided practical exposure to:

- Web application security assessment concepts.
- Passive reconnaissance and DNS information gathering.
- Security testing methodology.
- Identification and classification of common web application weaknesses.
- Evidence documentation and security reporting.
- Vulnerability remediation and security recommendations.

## Disclaimer

This repository is intended for educational and cybersecurity learning purposes as part of the Networkwalks Week 4 assessment.

The findings summarised here are those documented in the assessment report. They should not be interpreted as an independent verification of the target's current security status.

No unauthorised access or testing outside the approved project scope is intended. Sensitive patient, employee, credential and organisational information must not be published in this repository.

## Author

**Nizamaddeen Umar**  
Networkwalks – Batch B083

---

© 2026 Networkwalks. All rights reserved.
