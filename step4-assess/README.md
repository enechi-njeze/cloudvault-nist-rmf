# Step 4: Assess

**CloudVault Federal Health Exchange (FHX)**
**NIST RMF Step 4, NIST SP 800-53A Rev 5, NIST SP 800-115**
**Prepared By:** Enechi P.C. Njeze, ISSO/ISSM

---

## What Step 4 Is

Step 4 (Assess) is the independent verification that the controls selected in Step 2 and implemented in Step 3 are actually working as intended. For FedRAMP, this assessment must be performed by an accredited Third-Party Assessment Organization (3PAO). The 3PAO uses NIST SP 800-53A Rev 5 assessment procedures and NIST SP 800-115 testing methodology to examine, interview, and test each control.

The output of Step 4 is the Security Assessment Report (SAR), which documents every finding, every tested control, and the 3PAO's overall determination. The SAR feeds directly into the POA&M (unresolved findings become open items) and is a required component of the authorization package reviewed by the AO in Step 5.

For CloudVault FHX, the 3PAO is ClearPath Security Assessors LLC, A2LA-accredited and ISO/IEC 17020-certified, with no conflict of interest with CloudVault FHX or its vendors.

## Documents in This Folder

| Document | Description | Status |
|---|---|---|
| [security-assessment-plan.md](https://github.com/enechi-njeze/cloudvault-fedramp-ato/blob/main/assessments/security-assessment-plan.md) | Full SAP (in cloudvault-fedramp-ato) | Complete |
| [security-assessment-report.md](https://github.com/enechi-njeze/cloudvault-fedramp-ato/blob/main/assessments/security-assessment-report.md) | SAR shell (in cloudvault-fedramp-ato) | Complete |
| assessment-methodology-summary.md | Summary of NIST SP 800-53A methods used by ClearPath | In Progress |
| penetration-test-scope.md | Penetration test authorization, scope, and rules of engagement | Planned |

## Assessment Scope for CloudVault FHX

| Component | Assessment Method | Controls Covered |
|---|---|---|
| AWS GovCloud Application Tier | Document Review, Configuration Inspection, Automated Scan | AC, IA, SC, SI |
| Database Tier (RDS) | Document Review, Configuration Inspection, Automated Scan | AC, AU, SC, SI |
| API Gateway and Load Balancers | Configuration Inspection, Penetration Testing | AC, SC |
| IAM and Identity | Document Review, Interview, Configuration Inspection | AC, IA, PS |
| Audit Logging (CloudTrail, CloudWatch) | Configuration Inspection, Log Review | AU |
| Incident Response Procedures | Document Review, Tabletop Exercise | IR |
| Contingency and DR | Document Review, Tabletop Exercise | CP |
| Personnel and Training | Document Review, Interview | AT, PS |
| Physical Security | AWS Inherited: Document Review of FedRAMP Package | PE |
| Supply Chain | Document Review, Interview | SR, SA |

## 3PAO Assessment Timeline

| Phase | Duration | Key Deliverable |
|---|---|---|
| Kick-off and document review | 2 weeks | Document review findings |
| Automated scanning | 2 weeks | Scan results, initial findings |
| Interviews and configuration review | 3 weeks | Interview notes, configuration findings |
| Penetration testing | 2 weeks | Penetration test report |
| SAR drafting and review | 3 weeks | Draft SAR |
| Final SAR delivery | 1 week | Final SAR |
| **Total** | **16 weeks** | **Complete authorization package** |

## Key Step 4 Tasks (NIST SP 800-37 Rev 2)

| Task | Description | Reference |
|---|---|---|
| A-1 | Select assessor or assessment team | NIST SP 800-53A Rev 5 |
| A-2 | Develop, review, and approve assessment plan | SAP |
| A-3 | Assess security and privacy controls | NIST SP 800-53A Rev 5 |
| A-4 | Prepare assessment report | SAR |
| A-5 | Conduct initial remediation | POA&M |

## Related Documents

- [Step 3: Implement](../step3-implement/README.md)
- [Step 5: Authorize](../step5-authorize/README.md)
- [Security Assessment Plan](https://github.com/enechi-njeze/cloudvault-fedramp-ato/blob/main/assessments/security-assessment-plan.md)
- [Security Assessment Report](https://github.com/enechi-njeze/cloudvault-fedramp-ato/blob/main/assessments/security-assessment-report.md)
- [POA&M Master Tracker](https://github.com/enechi-njeze/cloudvault-fedramp-ato/blob/main/poam/poam-master-tracker.md)

---

*Enechi P.C. Njeze, CGRC, CISA, CISM, PMP, PMI-RMP, Security+, CHP, CSCS*
*ISSO and ISSM, CloudVault Federal Health Exchange (FHX)*
