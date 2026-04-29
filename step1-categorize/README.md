# Step 1: Categorize

**CloudVault Federal Health Exchange (FHX)**
**NIST RMF Step 1, FIPS 199, NIST SP 800-60**
**Prepared By:** Enechi P.C. Njeze, ISSO/ISSM

---

## What Step 1 Is

Step 1 (Categorize) establishes the security impact level for the information system. This is not a judgment call: FIPS 199 defines a structured methodology, and NIST SP 800-60 provides a detailed catalog of information types mapped to provisional impact values. The ISSO applies both standards to every type of information the system processes, then applies the high-water mark principle to determine the overall system categorization.

For CloudVault FHX, every information type in the system (PHI, PII, FTI, CUI, PCI, and administrative data) independently drives a HIGH categorization on at least one security objective. The result is the maximum possible impact level: SC CloudVault FHX = {(Confidentiality, HIGH), (Integrity, HIGH), (Availability, HIGH)}.

This categorization directly determines the FedRAMP baseline (HIGH), the number of controls (421), and every resource and timeline decision in the authorization.

## Documents in This Folder

| Document | Description | Status |
|---|---|---|
| [fips199-security-categorization.md](https://github.com/enechi-njeze/cloudvault-fedramp-ato/blob/main/assessments/fips199-security-categorization.md) | Full FIPS 199 categorization document (in cloudvault-fedramp-ato) | Complete |
| categorization-worksheet.md | Step-by-step working document showing categorization decisions | In Progress |
| information-types-inventory.md | All NIST SP 800-60 information types with provisional and adjusted impact values | Planned |

## Categorization Result

| Security Objective | Impact Level | Primary Driver |
|---|---|---|
| Confidentiality | HIGH | PHI (HIPAA), FTI (IRS Pub 1075), PII (Privacy Act) |
| Integrity | HIGH | Patient safety, clinical decision-making, benefits eligibility |
| Availability | HIGH | 47-agency dependency, life-safety during medical emergencies, 4-hour RTO |
| **Overall System** | **HIGH** | **High-water mark: all three objectives are HIGH** |

## Key Step 1 Tasks (NIST SP 800-37 Rev 2)

| Task | Description | Reference |
|---|---|---|
| C-1 | Document the characteristics of the system | NIST SP 800-60, FIPS 199 |
| C-2 | Categorize the system and document results | FIPS 199 |

## Why This Categorization Cannot Be Lowered

Five independent factors each independently require HIGH:

1. FTI (Federal Tax Information) requires HIGH Confidentiality as a statutory requirement under IRC Section 6103 and IRS Pub 1075. No agency may override this.
2. PHI affecting 890,000+ patients requires HIGH Confidentiality under HIPAA civil monetary penalty thresholds, which can reach $1.9M per violation category per year.
3. Clinical decision-making integrity drives HIGH Integrity: an incorrect medication record or erroneous eligibility determination could directly harm patients.
4. 47-agency dependency on a single platform drives HIGH Availability: loss of availability is not inconvenient, it stops health services delivery across federal programs simultaneously.
5. The FedRAMP Authorization Act requires cloud systems at this scale seeking JAB P-ATO to meet the FedRAMP High baseline. Categorizing below HIGH would disqualify CloudVault FHX from JAB review.

## Related Documents

- [Step 0: Prepare](../step0-prepare/README.md)
- [Step 2: Select](../step2-select/README.md)
- [FIPS 199 Document](https://github.com/enechi-njeze/cloudvault-fedramp-ato/blob/main/assessments/fips199-security-categorization.md)

---

*Enechi P.C. Njeze, CGRC, CISA, CISM, PMP, PMI-RMP, Security+, CHP, CSCS*
*ISSO and ISSM, CloudVault Federal Health Exchange (FHX)*
