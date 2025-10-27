---
title: 'Exercise 04: Investigate and resolve data ingestion failures from misconfigured app connectors'
layout: default
nav_order: 6
has_children: true
---


# Exercise 04: Investigate and resolve data ingestion failures from misconfigured app connectors

### Exercise learning objectives
- Detect ingestion gaps across multiple connectors using health dashboards and telemetry.  
- Identify, prioritize, and troubleshoot misconfigurations impacting visibility and investigations.  
- Restore and validate continuous data flow from critical log sources, verifying via timestamps and events.  



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


### Estimated exercise time (minutes) for a student: **60 minutes**