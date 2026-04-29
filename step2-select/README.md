# Step 2: Select

**CloudVault Federal Health Exchange (FHX)**
**NIST RMF Step 2, NIST SP 800-53 Rev 5, FedRAMP High Baseline**
**Prepared By:** Enechi P.C. Njeze, ISSO/ISSM

---

## What Step 2 Is

Step 2 (Select) takes the HIGH impact categorization from Step 1 and translates it into a specific set of security and privacy controls that CloudVault FHX must implement. For a FedRAMP High system, the starting point is the FedRAMP High baseline: 421 controls across 20 NIST SP 800-53 Rev 5 control families. The ISSO then reviews that baseline and makes tailoring decisions, identifying controls that can be inherited from AWS GovCloud, controls that require system-specific implementation, and any controls that require organizational parameters (called assignment and selection values).

This step is where deep NIST SP 800-53 knowledge matters. A practitioner who understands the High baseline can identify appropriate compensating controls, justify tailoring decisions to the AO, and reduce unnecessary assessment scope by accurately documenting inherited controls.

## Documents in This Folder

| Document | Description | Status |
|---|---|---|
| control-selection-record.md | Tailoring decisions for all 421 FedRAMP High controls | In Progress |
| inherited-controls-matrix.md | Controls fully or partially inherited from AWS GovCloud | Planned |
| organizational-parameters.md | Assignment and selection values for parameterized controls | Planned |
| compensating-controls-register.md | Compensating controls applied where standard controls cannot be met | Planned |

## FedRAMP High Baseline Summary

| Control Family | Abbr. | FedRAMP High Count |
|---|---|---|
| Access Control | AC | 42 |
| Awareness and Training | AT | 6 |
| Audit and Accountability | AU | 16 |
| Assessment, Authorization, Monitoring | CA | 9 |
| Configuration Management | CM | 14 |
| Contingency Planning | CP | 13 |
| Identification and Authentication | IA | 13 |
| Incident Response | IR | 10 |
| Maintenance | MA | 6 |
| Media Protection | MP | 8 |
| Physical and Environmental Protection | PE | 20 |
| Planning | PL | 11 |
| Program Management | PM | 32 |
| Personnel Security | PS | 9 |
| PII Processing and Transparency | PT | 8 |
| Risk Assessment | RA | 10 |
| System and Services Acquisition | SA | 23 |
| System and Communications Protection | SC | 51 |
| System and Information Integrity | SI | 23 |
| Supply Chain Risk Management | SR | 12 |
| **Total** | | **421** |

## Key Tailoring Decisions for CloudVault FHX

**Inherited from AWS GovCloud (approximately 156 controls):** Physical controls (PE family), many infrastructure-level SC controls, hardware-level MA controls, and portions of the AU family covering CloudTrail and infrastructure logging.

**System-specific (approximately 187 controls):** All application-layer AC controls, the full IA family for CloudVault FHX users (AWS handles infrastructure identity, not application identity), all IR procedures, and the full CM family for the application and its configuration.

**Shared responsibility (approximately 78 controls):** AU (CloudVault FHX owns application-layer audit logging, AWS owns infrastructure-layer), SC-8 (AWS provides TLS on the network layer, CloudVault FHX owns application-level encryption).

## Key Step 2 Tasks (NIST SP 800-37 Rev 2)

| Task | Description | Reference |
|---|---|---|
| S-1 | Select security controls | NIST SP 800-53 Rev 5, FedRAMP High Baseline |
| S-2 | Tailor security controls | NIST SP 800-53 Rev 5, Appendix C |
| S-3 | Document security controls in the SSP | SSP Control Implementation Summary |

## Related Documents

- [Step 1: Categorize](../step1-categorize/README.md)
- [Step 3: Implement](../step3-implement/README.md)
- [SSP Control Implementation Summary](https://github.com/enechi-njeze/cloudvault-fedramp-ato/blob/main/docs/system-security-plan.md)
- [CIS and CISM Tables](https://github.com/enechi-njeze/cloudvault-fedramp-ato/tree/main/ssp-attachments/att-08-control-implementation-summary)

---

*Enechi P.C. Njeze, CGRC, CISA, CISM, PMP, PMI-RMP, Security+, CHP, CSCS*
*ISSO and ISSM, CloudVault Federal Health Exchange (FHX)*
