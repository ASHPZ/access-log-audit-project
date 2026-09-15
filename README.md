# Access Control Incident Response and Audit

## Project Overview
This project presents an incident response investigation and access control audit for a growing business. The primary objective was to investigate an unauthorized financial transaction, analyze server access logs to identify the threat actor, and recommend robust security controls to improve the company's Identity and Access Management (IAM) posture.

## Scenario
A growing company recently experienced a security incident where an unauthorized deposit was initiated to an unknown bank account. Fortunately, the financial manager flagged the anomaly and successfully stopped the payment. As the newly hired cybersecurity professional, I was tasked with conducting a thorough incident audit. This involved reviewing access logs to track the threat actor, identifying critical flaws in the company's user access controls, and recommending mitigations to prevent future occurrences.

## Key Findings & Vulnerabilities
During the log analysis and audit, several critical vulnerabilities were identified:
* **Orphaned Accounts (Improper Offboarding):** A former contractor (Robert Taylor Jr.) whose contract expired on 12/27/2019 still had an active, accessible account in 2023.
* **Violation of Least Privilege:** The compromised contractor account retained full Administrator privileges, granting unrestricted access to critical financial and payroll systems.
* **Missing Technical Controls:** The organization lacked automated account expiration policies and did not enforce Multi-Factor Authentication (MFA) for privileged access.

## Compliance & Frameworks Applied
This investigation and subsequent recommendations align with industry best practices and frameworks:
* **NIST Cybersecurity Framework (CSF):** Applied the "Protect" and "Detect" functions, specifically focusing on Identity Management, Authentication, and Access Control (PR.AC) and Anomalies and Events (DE.AE).
* **Principle of Least Privilege (PoLP):** Evaluated user permissions to ensure employees and third-party contractors only possess the minimum access rights necessary to perform their legitimate duties.
* **Identity and Access Management (IAM) Best Practices:** Assessed the lifecycle of user accounts, highlighting the critical need for strict offboarding procedures and Role-Based Access Control (RBAC).

## Documentation Included
* **[Incident_Access_Control_Report.pdf](./Incident_Access_Control_Report.pdf):** The finalized incident report detailing the audit notes, identified access control issues, and the formal recommendations for security mitigation.
* **[Log.xlsx](./Log.xlsx):** A log describing the incident and containing a table of company employees.
