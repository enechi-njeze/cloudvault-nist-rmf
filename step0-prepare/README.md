# Step 0: Prepare

**CloudVault Federal Health Exchange (FHX)**
**NIST RMF Step 0, NIST SP 800-37 Rev 2**
**Prepared By:** Enechi P.C. Njeze, ISSO/ISSM

---

## What Step 0 Is

Step 0 (Prepare) is the foundational step added in NIST SP 800-37 Rev 2. It exists at both the organization level and the system level. Before any system is categorized, before any controls are selected, the organization must establish the context, roles, risk tolerance, and governance structures that will govern all RMF decisions. Skipping this step means authorization decisions are made without a defined risk appetite, without assigned accountability, and without the documented organizational context that gives an AO the confidence to sign an ATO.

For CloudVault FHX, Step 0 is especially critical because the system crosses 47 federal agencies, involves five data types (PHI, PII, CUI, FTI, PCI), and is seeking simultaneous Agency ATO and JAB P-ATO authorization. The preparation activities define who is responsible for every decision in the authorization lifecycle.

## Documents in This Folder

| Document | Description | Status |
|---|---|---|
| rmf-roles-responsibilities.md | Assigned RMF roles per NIST SP 800-37 Rev 2 Appendix D | In Progress |
| risk-management-strategy.md | Organization-level risk tolerance and risk framing decisions | Planned |
| system-registration.md | CloudVault FHX registered in federal system inventory | Planned |
| common-controls-identification.md | Controls inherited from AWS GovCloud and agency infrastructure | Planned |
| mission-business-objectives.md | System purpose, critical functions, and dependencies | Planned |

## Key Step 0 Tasks (NIST SP 800-37 Rev 2)

The following tasks must be completed before Step 1 begins:

| Task | Description | Responsible Role |
|---|---|---|
| P-1 | Establish risk management roles | Senior Agency Official for Privacy, SAISO |
| P-2 | Establish a risk management strategy | Senior Leadership |
| P-3 | Identify missions and business functions | System Owner |
| P-4 | Identify stakeholders | System Owner, ISSO |
| P-5 | Identify assets | System Owner, ISSO/ISSM |
| P-6 | Identify authorization boundaries | ISSO/ISSM, System Owner |
| P-7 | Identify information types | ISSO/ISSM (NIST SP 800-60) |
| P-8 | Conduct organizational risk assessment | Risk Executive |
| P-9 | Identify and prioritize requirements | System Owner, Privacy Officer |
| P-10 | Apply System Development Life Cycle (SDLC) | Program Manager |
| P-11 | Select common controls | SAISO, ISSO/ISSM |
| P-12 | Define authorization strategy | SAISO, AO |
| P-13 | Identify and document supply chain risks | System Owner, ISSO |
| P-14 | Conduct system-level risk assessment | ISSO/ISSM |
| P-15 | Define the authorization boundary | ISSO/ISSM, System Owner, AO |
| P-16 | Register the information system | ISSO/ISSM |
| P-17 | Select the security categorization approach | ISSO/ISSM |
| P-18 | Identify privacy requirements | Privacy Officer |
| P-19 | Identify privacy controls | Privacy Officer, ISSO/ISSM |

## Why Step 0 Matters for CloudVault FHX

Without completed Step 0 activities, the authorization boundary (P-15) is undefined. This means the 3PAO does not know what to test. Without P-11 (common controls), CloudVault FHX must re-document controls that AWS GovCloud already provides under its own FedRAMP High authorization, wasting assessment time and inflating the POA&M. Without P-12 (authorization strategy), no one has made the formal decision to pursue both Agency ATO and JAB P-ATO simultaneously, meaning the resource and timeline implications have not been presented to the AO.

## Related Documents

- [README (Repository Index)](../README.md)
- [Step 1: Categorize](../step1-categorize/README.md)
- [Authorization Package](https://github.com/enechi-njeze/cloudvault-fedramp-ato/tree/main/authorization)

---

*Enechi P.C. Njeze, CGRC, CISA, CISM, PMP, PMI-RMP, Security+, CHP, CSCS*
*ISSO and ISSM, CloudVault Federal Health Exchange (FHX)*
