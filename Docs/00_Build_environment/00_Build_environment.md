---
title: 'Exercise 00: Build the environment'
layout: default
nav_order: 2
has_children: true
---


# Exercise 00: Build the environment

## Required Accounts & Permissions 

- Active Azure subscription is mandatory. 

- Lab environment: use the Owner role on the subscription to simplify setup and avoid permission issues. 

- Real-world deployments: granular RBAC assignments are recommended: 

- Contributor (or higher) on the subscription to enable Defender for Cloud plan settings. 

- Contributor (or higher) on the resource group to deploy the VM and template resources. 

- Security Reader (minimum) on Microsoft Defender XDR (security.microsoft.com) to verify device onboarding. 

- Security Administrator or Global Administrator if tenant-level security configurations need to be changed. 

## Licensing and Environment

- An active Microsoft 365 tenant with security.microsoft.com access. 

- Licensing covering each workload: 

    - Microsoft Defender XDR (via Microsoft 365 E5, Enterprise Mobility + Security E5). 

    - Defender for Endpoint Plan 2, Defender for Office 365 Plan 2, Defender for Identity, Defender for Cloud Apps, Microsoft Entra ID P2 (for risk-based policies & Identity Protection) 

- At least 1-2 test users, mailboxes, and onboarded devices (Windows 10/11/Server) to services MDE, MDI, MDO and MDCA for real telemetry.

## Roles & Permissions 

- Lab environment: Global Admin role for the lab 

- Real-world deployments: granular RBAC assignments are recommended: 

    - Security Reader (read-only) or Security Analyst / Security Administrator for M365 Defender. 

    - Global Reader or Service Support Admin to view M365 Service Health.  

    - Microsoft Sentinel Reader/Contributor on the Sentinel workspace (via Azure RBAC). 

    - Exchange Admin/ Security Admin (read) for Email & Collaboration policy visibility. 

    - Defender for Identity permissions (to view identity health & entities). 

    - Cloud App Security Admin/Reader (for Defender for Cloud Apps).