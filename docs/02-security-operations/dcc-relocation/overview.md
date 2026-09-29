---
document_id: SEC-DCC-RELOCATION-001
title: DCC Relocation — Business Continuity Operational Reference
version: 0.1
status: Draft
owner: KB Owner
scope: DCC Relocation / Business Continuity / Secondary Site
updated: 2026-09-29
---

# DCC Relocation — Business Continuity Operational Reference

## 1. Status and Source Boundary
This document is a **Draft Operational Reference** derived from the KB Owner-supplied summary of **OB-SOP-DCC-0003 (BCP - DCC Relocation Rev. 03)**. It is not an Active SOP. Missing operational facts remain Knowledge Gaps and must not be inferred.

## 2. Purpose
Provide a controlled operational reference for relocating One Bangkok control and management operations from the primary DCC area to a Secondary Site under the Business Continuity Plan when the primary area cannot be used normally.

## 3. Scope
Participating units associated with Mozart operations: DCC, SOC, FMC, BMO, CC, NOC, and One Bangkok System Support (L1).

The source does not establish which personnel, if any, must remain at the Primary Site during relocation.

## 4. Trigger / Activation
DCC Relocation may be activated when the DCC area cannot be used normally, including:
- Emergency / unsafe condition
- System testing
- Necessary maintenance

**Activation Authority:** DCC Manager or an authorized decision-maker declares activation of BCP – DCC Relocation through POC.

The source does not further define “authorized decision-maker.”

## 5. Secondary Sites
The source identifies:
- PB1 / P1B1
- Engineering Room
- FCC

Secondary Site assignment differs by unit; examples include SOC/FMC relocating to FCC or Engineering Room while other units relocate to PB1.

### BCP Room Boundary
Skills Hunter separately defines **BCP Room** as an SOC backup operations center on B1 near Load 1 beneath Parade / The Storeys.

This source does not establish that PB1/P1B1, Engineering Room, FCC, and the canonical BCP Room are the same location. Do not merge or equate them without an approved source.

## 6. Roles and Responsibilities
### DCC / DCC Manager
- DCC sends Email Notification to relevant units regarding the incident and relocation schedule.
- DCC Manager or an authorized decision-maker activates the relocation plan through POC.
- DCC Manager declares return to the Primary Site through POC after confirmation from relevant parties.
- DCC Manager declares **Deactivate DCC Relocation** after readiness is confirmed.

### Participating Units
DCC, SOC, FMC, BMO, CC, NOC, and One Bangkok System Support (L1) relocate personnel/equipment according to the source-defined arrangement.

### IMT
During return to the Primary Site, the first returning staff report system-readiness results to DCC Manager and IMT.

## 7. Authority
Established:
- **Activate DCC Relocation:** DCC Manager or authorized decision-maker.
- **Return to Primary Site:** DCC Manager after confirmation from relevant parties.
- **Deactivate DCC Relocation:** DCC Manager after confirmation that systems are back online.

Not established:
- Formal authority to declare the Secondary DCC / Secondary Site **Operational**.
- Identity/scope of “authorized decision-maker” beyond DCC Manager.

## 8. Resources / Equipment
Depending on unit requirements:
- Notebook
- POC (Push-to-Talk Over Cellular)
- Radio
- IP Phone
- Earphone

Access Card is not identified as required equipment. The source states that the **BCP Room key** is collected at the Engineering Room, One Power, M Floor.

## 9. Systems / Pre-Relocation Check
**Pre-Relocation System Check Form: OB-SOP-FR-DCC-0302**

Systems identified include:
- CCTV Application
- Mozart
- Dispatcher Hytalk
- Telephone / radio communication
- Internet / WIFI

The detailed startup/testing/validation sequence and Secondary Site acceptance criteria are not established.

## 10. Relocation Procedure — Source-Supported Flow
1. A relocation trigger occurs and the DCC area cannot be used normally, or relocation is required for testing/necessary maintenance.
2. DCC Manager or an authorized decision-maker activates BCP – DCC Relocation through POC.
3. DCC sends Email Notification to relevant units with incident/relocation information and schedule.
4. Participating units relocate personnel and required equipment to their designated Secondary Site.
5. Required systems are checked using the applicable readiness process and OB-SOP-FR-DCC-0302.
6. Units operate from the Secondary Site.

**Knowledge Gap:** formal declaration authority and detailed criteria for declaring the Secondary Site Operational are not established.

## 11. Communication and Escalation
Established:
- Email Notification from DCC to relevant units.
- POC for activation and DCC Manager announcements.
- Radio / POC / IP Phone as communication resources.

**Knowledge Gap:** no radio channel number/name is established.

## 12. Return to Primary Site
1. After confirmation from relevant parties, DCC Manager announces return through POC.
2. A first group, described by the source as **half of the staff**, returns to DCC.
3. The first group starts, checks, and confirms that work systems are online and operating to the required standard.
4. The first group reports readiness to DCC Manager and IMT.
5. Once all systems are confirmed online, DCC Manager announces **Deactivate DCC Relocation**.
6. Remaining personnel return to normal operations.

## 13. Records and Forms
Established:
- **OB-SOP-FR-DCC-0302 — Pre-Relocation System Check Form**

The underlying SOP is described as including an evaluation form and formal document approvers, but fields, mandatory evidence, retention requirements, and approval workflow are not established in the supplied detailed summary.

## 14. Termination / Handover
Operational return is supported when the first returning staff confirm systems are online and report readiness to DCC Manager and IMT. DCC Manager then announces **Deactivate DCC Relocation**, after which remaining personnel return to normal operations.

No separate case-closure workflow is established by this source.

## 15. Knowledge Gaps
1. **Primary Site Staffing** — who, if anyone, remains at the Primary Site during relocation.
2. **Radio Channel** — specific radio channel/name used during DCC Relocation.
3. **Secondary Operational Declaration Authority** — who formally declares the Secondary Site Operational and the criteria.
4. **Secondary Site System Check Sequence** — detailed order and acceptance criteria.
5. Definition and authority scope of an “authorized decision-maker” other than DCC Manager.
6. Exact mapping of each participating unit to PB1/P1B1, Engineering Room, or FCC beyond supplied examples.
7. Relationship, if any, between PB1/P1B1, Engineering Room, FCC and the canonical SOC BCP Room.
8. Mandatory fields/evidence, retention, and approval workflow for evaluation/check forms.
9. Separate case-closure requirements, if any.

## 16. Source Traceability
Primary supplied source:
- KB Owner-provided summary based on **OB-SOP-DCC-0003 (BCP - DCC Relocation Rev. 03)**, supplied 2026-09-29.

Canonical cross-check:
- Skills Hunter `docs/00-system/terminology.md` for the existing BCP Room definition.

## 17. Guardrails
- Do not infer a radio channel.
- Do not infer which staff remain at the Primary Site.
- Do not infer who declares the Secondary Site Operational.
- Do not equate Secondary Site names with the canonical BCP Room unless an approved source establishes that relationship.
- Do not invent system acceptance criteria, form fields, evidence, or case-closure requirements.
- Preserve Draft status until unresolved operational gaps are reviewed and the KB Owner explicitly approves promotion.

## 18. Revision History
| Version | Status | Change |
|---|---|---|
| 0.1 | Draft | Initial DCC Relocation Operational Reference created from KB Owner-approved source input and gap analysis. |
