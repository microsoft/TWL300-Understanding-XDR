---
title: 'Exercise 02: Configure XDR according to Microsoft Recommended Practices'
layout: default
nav_order: 4
has_children: true
---

# Exercise 02: Configure XDR according to Microsoft Recommended Practices

### Exercise learning objectives:
•	Configure core Microsoft Defender products (Endpoint, Office 365, Cloud Apps) in Microsoft Defender XDR to align with recommended practices.

•	Implement and validate security baselines for endpoint hardening, email/web protection, and identity access controls.

•	Tune key policies (e.g. Attack Surface Reduction, Safe Links/Attachments,    Alert Tuning Rules) and observe the impact on detections, user experience and Secure Score.



### Licensing and environment

- An active Microsoft 365 tenant with security.microsoft.com access. 

- Licensing covering each workload: 

    - Microsoft Defender XDR (via Microsoft 365 E5, Enterprise Mobility + Security E5). 

    - Defender for Endpoint Plan 2, Defender for Office 365 Plan 2, Defender for Identity, Defender for Cloud Apps, Microsoft Entra ID P2 (for risk-based policies & Identity Protection) 

- At least 1–2 test users, mailboxes, and onboarded devices (Windows 10/11/Server) to produce real telemetry. Note: Lab uses seeded test activity data where required and at least one Azure Windows VM on boarded. 

### Roles and permissions

- Lab environment: Global Admin role for the lab 

- Real-world deployments: granular RBAC assignments are recommended: 

    - Security Reader (read-only) or Security Analyst / Security Administrator for M365 Defender. 

    - Global Reader or Service Support Admin to view M365 Service Health.  

    - Microsoft Sentinel Reader/Contributor on the Sentinel workspace (via Azure RBAC). 

    - Exchange Admin/ Security Admin (read) for Email & Collaboration policy visibility. 

    - Defender for Identity permissions (to view identity health & entities). 

    - Cloud App Security Admin/Reader (for Defender for Cloud Apps).



### Estimated exercise time (minutes) for a student: **6**0 minutes**