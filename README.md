# cloudvault-nist-rmf

![NIST RMF](https://img.shields.io/badge/Framework-NIST%20RMF-navy)
![FedRAMP High](https://img.shields.io/badge/FedRAMP-High-red)
![Impact Level](https://img.shields.io/badge/Impact-HIGH-critical)
![Status](https://img.shields.io/badge/Status-In%20Progress-yellow)
![AWS GovCloud](https://img.shields.io/badge/Cloud-AWS%20GovCloud-orange)

---

## NIST Risk Management Framework: Steps 0-6 Implementation
### CloudVault Federal Health Exchange (FHX)

This repository documents the complete, step-by-step implementation of the NIST Risk Management Framework (RMF) for the CloudVault Federal Health Exchange (FHX), a FedRAMP High federal health data platform operating on AWS GovCloud. Every document here reflects the actual work product a senior ISSO and ISSM produces when executing RMF across a HIGH-impact system handling PHI, PII, CUI, and FTI for 47 federal health agencies and 890,000+ patient records.

While the `cloudvault-fedramp-ato` repository contains the finished authorization package, this repository shows the full methodology and decision trail behind it, from the earliest preparation activities through ongoing continuous monitoring.

---

## System Reference Card

| Field | Detail |
|---|---|
| System Name | CloudVault Federal Health Exchange (FHX) |
| System Type | Federally operated cloud-based health data exchange |
| Impact Level | HIGH: Confidentiality HIGH, Integrity HIGH, Availability HIGH |
| Cloud Platform | AWS GovCloud (us-gov-east-1 and us-gov-west-1) |
| FedRAMP Baseline | FedRAMP High: 421 controls, NIST SP 800-53 Rev 5 |
| Authorization Tracks | Agency ATO (AO: Deputy Director Henry Kline) and JAB P-ATO |
| Data Types | PHI, PII, CUI, FTI, PCI at HIGH sensitivity |
| Scale | 47 federal agencies, 890,000+ patient records, 12,000+ endpoints |
| System Owner | Dr. Patricia Owens, Deputy Director, Federal Health Systems |
| ISSO/ISSM | Enechi P.C. Njeze, CGRC, CISA, CISM, PMP, PMI-RMP, Security+, CHP, CSCS |
| Authorizing Official | Deputy Director Henry Kline |
| 3PAO | ClearPath Security Assessors LLC, FedRAMP-accredited |

---

## What the NIST RMF Is

The NIST Risk Management Framework (RMF), defined in NIST SP 800-37 Rev 2, is the mandatory process all federal information systems must follow to obtain and maintain authorization to operate. It consists of 7 steps:

- **Step 0: Prepare** — Establish the organizational context, assign roles, and build the risk management infrastructure before any system-specific work begins.
- **Step 1: Categorize** — Determine the system's impact level using FIPS 199 and NIST SP 800-60.
- **Step 2: Select** — Choose the appropriate security controls baseline (FedRAMP High for CloudVault FHX) and tailor as needed.
- **Step 3: Implement** — Deploy the selected controls and document how each one is implemented.
- **Step 4: Assess** — Have a 3PAO independently test the controls and produce a Security Assessment Report (SAR).
- **Step 5: Authorize** — The AO reviews the full package and makes a formal risk-based authorization decision.
- **Step 6: Monitor** — Maintain the authorization through ongoing ConMon, POA&M management, and annual assessments.

For a HIGH-impact system like CloudVault FHX, skipping or shortcutting any step creates legal liability under FISMA, exposes 890,000+ patient records, and invalidates the ATO.

---

## Repository Deliverables

| # | Document | Folder | Framework Reference | Status |
|---|---|---|---|---|
| 1 | RMF Step 0: Prepare Activities | step0-prepare/ | NIST SP 800-37 Rev 2, Task P-1 through P-19 | In Progress |
| 2 | System Categorization Worksheet | step1-categorize/ | FIPS 199, NIST SP 800-60 | In Progress |
| 3 | Control Selection and Tailoring Record | step2-select/ | NIST SP 800-53 Rev 5, FedRAMP High Baseline | In Progress |
| 4 | Control Implementation Evidence Summary | step3-implement/ | NIST SP 800-53 Rev 5 | In Progress |
| 5 | Security Assessment Plan (SAP) | step4-assess/ | NIST SP 800-53A Rev 5 | In Progress |
| 6 | Security Assessment Report (SAR) Shell | step4-assess/ | NIST SP 800-53A Rev 5 | In Progress |
| 7 | Authorization Decision Memorandum | step5-authorize/ | NIST SP 800-37 Rev 2, Task R-4 | In Progress |
| 8 | Authorization Package Checklist | step5-authorize/ | FedRAMP Authorization Package Guide | In Progress |
| 9 | Continuous Monitoring Strategy | step6-monitor/ | NIST SP 800-137, FedRAMP ConMon Guide | In Progress |
| 10 | Annual Assessment Schedule | step6-monitor/ | FedRAMP ConMon Requirements | In Progress |
| 11 | RMF Roles and Responsibilities Matrix | step0-prepare/ | NIST SP 800-37 Rev 2, Appendix D | In Progress |
| 12 | RMF Process Flow Diagram | diagrams/ | NIST SP 800-37 Rev 2 | In Progress |

---

## Folder Structure

```
cloudvault-nist-rmf/
├── step0-prepare/          # Organizational preparation: roles, policies, risk tolerance
├── step1-categorize/       # FIPS 199 categorization and NIST SP 800-60 mapping
├── step2-select/           # Control baseline selection and tailoring decisions
├── step3-implement/        # Control implementation evidence and documentation
├── step4-assess/           # SAP, SAR, and 3PAO assessment artifacts
├── step5-authorize/        # Authorization package, AO decision memo, risk acceptance
├── step6-monitor/          # ConMon strategy, monthly reports, annual assessment schedule
└── diagrams/               # RMF process flow, step dependency map, timeline
```

---

## Laws, Regulations, and Standards

| Instrument | Relevance to This Repository |
|---|---|
| FISMA (44 U.S.C. § 3551 et seq.) | Mandates RMF implementation for all federal systems |
| NIST SP 800-37 Rev 2 | Defines the 7 RMF steps, tasks, and role responsibilities |
| NIST SP 800-53 Rev 5 | Security and privacy controls applied in Steps 2 and 3 |
| NIST SP 800-53A Rev 5 | Assessment procedures applied in Step 4 |
| NIST SP 800-60 Vol I and II | Information type mapping used in Step 1 |
| FIPS 199 | Security categorization standard applied in Step 1 |
| FIPS 200 | Minimum security requirements driving control selection in Step 2 |
| NIST SP 800-137 | Continuous monitoring guidance for Step 6 |
| OMB Circular A-130 | Federal information management and RMF policy |
| FedRAMP Authorization Act (Pub. L. 117-290) | FedRAMP statutory authority and JAB authorization |
| HIPAA/HITECH | PHI protection requirements driving HIGH categorization |
| IRS Publication 1075 | FTI safeguarding requirements affecting control selection |

---

## Certifications This Portfolio Showcases

| Certification | Issuing Body | Relevance |
|---|---|---|
| CGRC (Certified in Governance, Risk, and Compliance) | ISC2 | Core RMF and FedRAMP competency |
| CISA (Certified Information Systems Auditor) | ISACA | Assessment methodology, Step 4 |
| CISM (Certified Information Security Manager) | ISACA | Risk governance, Step 0 and Step 5 |
| PMP (Project Management Professional) | PMI | RMF program management and milestone tracking |
| PMI-RMP (Risk Management Professional) | PMI | Risk assessment and treatment in Steps 1-2 |
| CompTIA Security+ SY0-701 | CompTIA | Technical control implementation, Step 3 |
| CHP (Certified HIPAA Professional) | APHP | PHI protection, HIPAA-driven control tailoring |
| CSCS | - | Cloud security control selection |
| CISSP (in progress) | ISC2 | Comprehensive security architecture across all steps |

---

## Core Competencies Demonstrated

Executing NIST RMF Steps 0-6 for a FedRAMP High system of this scale demonstrates the following senior GRC competencies:

Categorization judgment under FIPS 199 and NIST SP 800-60, including independent analysis of information types, high-water mark application, and written justification for each security objective. Control tailoring and selection from the 421-control FedRAMP High baseline, including scoping, compensating controls, and inherited control identification for AWS GovCloud. Evidence collection and control implementation documentation across all 20 NIST SP 800-53 Rev 5 families. 3PAO coordination and SAP development, including scope definition, methodology selection, and assessment scheduling. AO briefing and authorization package assembly, including risk posture summaries and executive decision support. Continuous monitoring program design and execution, including POA&M governance, scan scheduling, and FedRAMP PMO reporting.

---

## Related Repositories

| Repository | Relationship |
|---|---|
| [cloudvault-fedramp-ato](https://github.com/enechi-njeze/cloudvault-fedramp-ato) | The resulting authorization package produced by this RMF process |
| cloudvault-hipaa | HIPAA compliance program that informs PHI-driven control tailoring in Step 2 |
| cloudvault-risk-governance | Enterprise risk register that feeds RMF Step 0 risk tolerance decisions |
| cloudvault-master-controls | Capstone cross-framework control mapping referencing this repository |

---

## Portfolio Status

| Component | Status |
|---|---|
| Repository created | Complete |
| README.md | Complete |
| Step 0: Prepare folder | In Progress |
| Step 1: Categorize folder | In Progress |
| Step 2: Select folder | In Progress |
| Step 3: Implement folder | In Progress |
| Step 4: Assess folder | In Progress |
| Step 5: Authorize folder | In Progress |
| Step 6: Monitor folder | In Progress |
| Diagrams folder | In Progress |
| RMF Roles and Responsibilities Matrix | Planned |
| Step-by-step implementation documents | Planned |

---

*Prepared by: Enechi P.C. Njeze, CGRC, CISA, CISM, PMP, PMI-RMP, CompTIA Security+ SY0-701, CHP, CSCS*
*ISSO and ISSM: CloudVault Federal Health Exchange (FHX)*
*LinkedIn: [Enechi P.C. Njeze](https://www.linkedin.com/in/enechi-njeze)*
*Portfolio: [CloudVault GRC Portfolio](https://github.com/enechi-njeze)*
