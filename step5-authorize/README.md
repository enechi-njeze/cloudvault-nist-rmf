# Step 5: Authorize

**CloudVault Federal Health Exchange (FHX)**
**NIST RMF Step 5, NIST SP 800-37 Rev 2**
**Prepared By:** Enechi P.C. Njeze, ISSO/ISSM

---

## What Step 5 Is

Step 5 (Authorize) is the formal risk-based decision by the Authorizing Official (AO) to accept the residual risk in the system and grant an Authorization to Operate (ATO). The AO reviews the complete authorization package: the SSP, SAP, SAR, POA&M, and all supporting attachments. Based on the overall risk posture, the AO either grants the ATO, grants a conditional ATO (requiring POA&M completion within specified timeframes), or denies authorization.

For CloudVault FHX, the authorization package must be compelling for two separate audiences: Deputy Director Henry Kline (Agency ATO) reviews residual risk for Federal Health Data Office operations, while the JAB Board (Col. Diana Marsh, Frank Osei, Carol Whitfield) reviews government-wide suitability for reuse across all federal agencies.

An ATO is not a certification that the system is perfectly secure. It is a formal documented decision that the residual risk is acceptable given the mission need. The ISSO's job is to present that risk picture clearly, accurately, and without minimizing or hiding findings.

## Documents in This Folder

| Document | Description | Status |
|---|---|---|
| [ato-letter.md](https://github.com/enechi-njeze/cloudvault-fedramp-ato/blob/main/authorization/ato-letter.md) | Formal ATO letter (in cloudvault-fedramp-ato) | Complete |
| authorization-package-checklist.md | Complete checklist of all required package components | In Progress |
| risk-acceptance-memo.md | Formal AO risk acceptance statement | Planned |
| authorization-decision-briefing.md | ISSO briefing document for AO review session | Planned |

## Authorization Package Components

The following documents must be assembled and submitted for AO review:

| Component | Location | Status |
|---|---|---|
| System Security Plan (SSP) | cloudvault-fedramp-ato/docs/ | Complete |
| FIPS 199 Security Categorization | cloudvault-fedramp-ato/assessments/ | Complete |
| Security Assessment Plan (SAP) | cloudvault-fedramp-ato/assessments/ | Complete |
| Security Assessment Report (SAR) | cloudvault-fedramp-ato/assessments/ | Complete |
| POA&M Master Tracker | cloudvault-fedramp-ato/poam/ | Complete |
| SSP Attachments (12 folders) | cloudvault-fedramp-ato/ssp-attachments/ | Complete |
| Authorization Boundary Diagrams | cloudvault-fedramp-ato/diagrams/ | Complete |
| Evidence Index | cloudvault-fedramp-ato/evidence/ | Complete |
| JAB Prioritization Request | cloudvault-fedramp-ato/jab-path/ | Complete |
| ATO Letter | cloudvault-fedramp-ato/authorization/ | Complete |

## ATO Decision Outcomes

| Outcome | Meaning | Next Step |
|---|---|---|
| ATO Granted | AO accepts residual risk, system authorized to operate | Proceed to Step 6: Monitor |
| Conditional ATO | Authorized with conditions: POA&M items must close by specified dates | Step 6 with enhanced monitoring |
| Authorization Denied | Risk is unacceptable, system cannot operate | Return to Step 3, remediate findings |

## CloudVault FHX Authorization Result

Authorization Type: Agency ATO + JAB P-ATO (dual track)
Agency ATO: Granted by Deputy Director Henry Kline, effective February 14, 2025
ATO Duration: 3 years (expires February 14, 2028)
JAB P-ATO: In JAB review process
POA&M Items at Authorization: 14 open items (0 Critical, 3 High, 6 Moderate, 5 Low)
Risk Posture: ACCEPTABLE

## Key Step 5 Tasks (NIST SP 800-37 Rev 2)

| Task | Description | Reference |
|---|---|---|
| R-1 | Prepare authorization package | SSP, SAR, POA&M |
| R-2 | Submit authorization package | AO submission |
| R-3 | Review authorization package | AO review |
| R-4 | Determine risk | AO risk determination |
| R-5 | Identify and implement risk responses | Risk acceptance or remediation |
| R-6 | Determine if risk is acceptable | AO decision |

## Related Documents

- [Step 4: Assess](../step4-assess/README.md)
- [Step 6: Monitor](../step6-monitor/README.md)
- [Authorization Package Hub](https://github.com/enechi-njeze/cloudvault-fedramp-ato/tree/main/authorization)
- [ATO Letter](https://github.com/enechi-njeze/cloudvault-fedramp-ato/blob/main/authorization/ato-letter.md)

---

*Enechi P.C. Njeze, CGRC, CISA, CISM, PMP, PMI-RMP, Security+, CHP, CSCS*
*ISSO and ISSM, CloudVault Federal Health Exchange (FHX)*
