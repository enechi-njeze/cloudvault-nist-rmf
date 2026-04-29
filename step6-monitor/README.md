# Step 6: Monitor

**CloudVault Federal Health Exchange (FHX)**
**NIST RMF Step 6, NIST SP 800-137, FedRAMP ConMon Requirements**
**Prepared By:** Enechi P.C. Njeze, ISSO/ISSM

---

## What Step 6 Is

Step 6 (Monitor) is the ongoing, never-ending work that begins the moment an ATO is granted and continues until the system is decommissioned. It is the most operationally intensive step in the RMF and the one that most clearly separates practitioners who understand authorization lifecycle management from those who only know how to get an initial ATO.

Under FedRAMP, continuous monitoring (ConMon) has specific, non-negotiable monthly and annual deliverables. The ISSO is personally accountable for ensuring these submissions are accurate, timely, and consistent with the system's actual security posture. A late or inaccurate ConMon submission can trigger a FedRAMP PMO review, a conditional status designation, or in serious cases, ATO revocation.

For CloudVault FHX, Step 6 is especially demanding because the dual-track authorization (Agency ATO plus JAB P-ATO) means two different audiences receive monthly reporting: the Federal Health Data Office AO staff and the FedRAMP PMO.

## Documents in This Folder

| Document | Description | Status |
|---|---|---|
| conmon-strategy.md | Formal continuous monitoring strategy document | In Progress |
| annual-assessment-schedule.md | 3-year assessment and testing calendar | Planned |
| significant-change-procedures.md | SCN process for changes that trigger AO notification | Planned |

## FedRAMP ConMon Monthly Requirements

The following must be submitted to the FedRAMP PMO every month:

| Deliverable | Due Date | Responsible Party |
|---|---|---|
| Vulnerability scan results (authenticated) | Within 30 days of scan | ISSO/ISSM |
| POA&M update (all open items) | Monthly | ISSO/ISSM |
| Inventory update (hardware, software) | Monthly | ISSO/ISSM |

## FedRAMP ConMon Annual Requirements

| Deliverable | Frequency | Responsible Party |
|---|---|---|
| Annual security assessment (3PAO) | Every 12 months | ISSO/ISSM, 3PAO |
| Penetration test | Every 12 months | 3PAO |
| Contingency plan test | Every 12 months | System Owner, ISSO |
| Incident response tabletop | Every 12 months | ISSO, IR Team |
| Privacy threshold analysis review | Every 12 months | Privacy Officer |

## Significant Change Notification (SCN) Process

Not every system change requires AO notification, but the following categories always trigger a Significant Change Notification under FedRAMP:

Changes to the authorization boundary, changes to external connections, changes to data types processed, changes to cryptographic modules, changes to the underlying cloud infrastructure (new AWS services added to scope), and changes that affect more than 30% of the total control baseline.

An SCN must be submitted to the AO and the FedRAMP PMO before the change is implemented. The AO may require a new assessment of affected controls. Failing to submit an SCN for a qualifying change is a material finding that can result in conditional ATO status.

## ConMon Posture History

| Reporting Period | Open POA&M Items | Risk Posture | On-Time Submission |
|---|---|---|---|
| April 2025 (Month 1 post-ATO) | 14 | ACCEPTABLE | Yes |
| May 2025 | 13 | ACCEPTABLE | Yes |
| June 2025 | 12 | ACCEPTABLE | Yes |
| July 2025 | 11 | ACCEPTABLE | Yes |
| August 2025 | 11 | ACCEPTABLE | Yes |
| September 2025 | 10 | ACCEPTABLE | Yes |
| October 2025 | 10 | ACCEPTABLE | Yes |
| November 2025 | 9 | ACCEPTABLE | Yes |
| December 2025 | 9 | ACCEPTABLE | Yes |
| January 2026 | 8 | ACCEPTABLE | Yes |
| February 2026 | 8 | ACCEPTABLE | Yes |
| March 2026 | 14 | ACCEPTABLE | Yes |

Note: March 2026 increase reflects new findings from the 12-month annual assessment, per standard FedRAMP ConMon lifecycle. All new findings have been assessed and assigned to appropriate responsible parties with approved completion dates.

## Key Step 6 Tasks (NIST SP 800-37 Rev 2)

| Task | Description | Reference |
|---|---|---|
| M-1 | Monitor control effectiveness | NIST SP 800-137 |
| M-2 | Assess selected controls | FedRAMP ConMon Guide |
| M-3 | Conduct remediation actions | POA&M |
| M-4 | Update the risk assessment | Risk Assessment |
| M-5 | Report security and privacy posture | FedRAMP PMO |
| M-6 | Make ongoing authorization decisions | AO |
| M-7 | System disposal | NIST SP 800-88 |

## Related Documents

- [Step 5: Authorize](../step5-authorize/README.md)
- [ConMon Monthly Report](https://github.com/enechi-njeze/cloudvault-fedramp-ato/blob/main/conmon/conmon-monthly-report-template.md)
- [POA&M Master Tracker](https://github.com/enechi-njeze/cloudvault-fedramp-ato/blob/main/poam/poam-master-tracker.md)
- [Authorization Package Hub](https://github.com/enechi-njeze/cloudvault-fedramp-ato/tree/main/authorization)

---

*Enechi P.C. Njeze, CGRC, CISA, CISM, PMP, PMI-RMP, Security+, CHP, CSCS*
*ISSO and ISSM, CloudVault Federal Health Exchange (FHX)*
