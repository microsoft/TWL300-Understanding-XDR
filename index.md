---
title: Introduction
layout: home
nav_order: 1
---

# TechWorkshop L300 Understanding XDR

## **Learning objectives**:  
At the end of this workshop, you will be able to:

•	Explain the Microsoft Defender XDR portfolio (MDE, MDO, MDI, MDA) and the daily SOC health-check workflow.

•	Apply Microsoft recommended practices to configure endpoint, email, identity, and cloud-app protections, and review Secure Score impact.

•	Evaluate medium-severity incidents by triaging alerts, pivoting across entities, and validating findings with Advanced Hunting (KQL).

•	Analyze and troubleshoot data-ingestion issues  ; verify restored telemetry with timestamps and test alerts.

•	Review a multi-stage intrusion (e.g., BEC) by correlating MDO/MDE/MDI/MDA signals, mapping to MITRE ATT&CK, and review mitigations.

•	Design and execute containment/remediation using AIR and Live Response (session revocation, MFA reset, device isolation).




## **Lab objectives**:
By the end of this workshop, you'll be able to:

-	Perform an XDR health check: verify service health, agent health, licensing/connections, and data ingestion via KQL.

-	Review Threat Intelligence and manage IoCs and exceptions. Review critical assets, asset criticality and asset rules.

-	Configure and validate MDE, MDO, MDA, and MDI; track Secure Score. 

-	Investigate a password-spray alert end-to-end using Advanced Hunting across Email, Identity, Device, and CloudApp events.

-	Restore connector telemetry by troubleshooting MDA connectors and MDI sensors; confirm via timestamps and test alerts.

-	Use Attack Story to build a kill-chain storyboard for a Business Email Compromise (BEC) scenario, from Safe Links bypass to endpoint activity with ATT&CK mapping.

-	Automate response by setting AIR remediation levels, enabling MDE advanced features, running Live Response scripts, and validating with safe artifacts.



## **Customer scenario**:

Zava Group supplies petroleum products across multiple regions. With demand volatility and tight margins, leadership has prioritized resilience and cost control at refineries while maintaining safe, continuous operations, terminals, and corporate offices. The workforce is split between 10,000 office staff who run finance, trading, procurement, and engineering, and 16,000 frontline workers on shifts who rely on shared kiosks and rugged devices. The environment spans on-prem AD for plant operations, hybrid-joined Windows endpoints, and a growing set of SaaS apps for vendor collaboration and invoicing.

Adversaries have adapted to the sector's pressure. Over recent weeks, Zava's finance/Accounts Payable P mailboxes have seen thread-hijack attempts and payment redirection requests that look indistinguishable from real vendor traffic. A targeted phish evaded an initial URL check and led to suspicious inbox rules on a priority account; concurrent identity telemetry showed atypical sign-ins and a small cluster of password-spray failures against shift accounts coming from a single   Autonomous System Number. On several machines, endpoint traces hinted at post-phish tooling (scripted archive exfiltration and OAuth consent prompts), while cloud app logs captured risky OAuth grants and anomalous downloads after hours. The security team needs unified visibility across email, identity, device, and cloud apps and fast, automated containment without disrupting plant safety.

Today, office users run Microsoft 365 E3 with Defender for Office 365 Plan 2, giving them strong email protection and investigations. Frontline workers, however, are on Microsoft 365 F3, which focuses on lightweight productivity and does not include advanced endpoint detection/response or automated email investigations by default. Zava's domain controllers supporting refinery authentication, require deep identity threat detection and the Security team wants consistent conditional access and risk-based controls across all users. To raise overall security maturity, Zava aims to standardize on a single XDR experience, expand telemetry coverage to frontline devices, and enable safe automation (AIR) while keeping tight control over change windows in operational sites.