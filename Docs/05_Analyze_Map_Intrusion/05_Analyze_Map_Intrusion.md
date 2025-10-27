---
title: 'Exercise 05: Analyze and Map a Multi-Stage Intrusion'
layout: default
nav_order: 2
has_children: true
---

# Exercise 05: Analyze and Map a Multi-Stage Intrusion

### **Exercise Learning Objectives**
- Detect and trace a Business Email Compromise (BEC) path starting with a Safe Links bypass and malicious attachment in Defender for Office 365 (MDO).  
- Correlate post-phish endpoint activity in Defender for Endpoint (MDE) to build a user/device attack timeline.  
- Enrich the story across email, identity, device, and cloud apps using Advanced Hunting and MDA signals.  
- Map observed behaviors to MITRE ATT&CK techniques and document gaps and mitigations.  

### **Licensing and Environment** 

- An active Microsoft 365 tenant with security.microsoft.com access. 

- Licensing covering each workload: 

    - Microsoft Defender XDR (via Microsoft 365 E5, Enterprise Mobility + Security E5). 

    - Defender for Endpoint Plan 2, Defender for Office 365 Plan 2, Defender for Identity, Defender for Cloud Apps, Microsoft Entra ID P2 (for risk-based policies & Identity Protection) 

- At least 1–2 test users, mailboxes, and onboarded devices (Windows 10/11/Server) to produce real telemetry. 

    {: .note }
    > Lab uses seeded test activity data where required and at least one Azure Windows VM on boarded. 

### **Roles & Permissions** 

- Lab environment: Global Admin role for the lab 

- Real-world deployments: granular RBAC assignments are recommended: 

    - Security Reader (read-only) or Security Analyst / Security Administrator for M365 Defender. 

    - Global Reader or Service Support Admin to view M365 Service Health.  

    - Microsoft Sentinel Reader/Contributor on the Sentinel workspace (via Azure RBAC). 

    - Exchange Admin/ Security Admin (read) for Email & Collaboration policy visibility. 

    - Defender for Identity permissions (to view identity health & entities). 

    - Cloud App Security Admin/Reader (for Defender for Cloud Apps).


### **Estimated exercise time (minutes) for a student: 50 minutes**


