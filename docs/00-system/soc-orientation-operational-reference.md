---
document_id: SEC-SYSTEM-SOC-ORIENTATION-OPS-001
title: SOC Orientation Operational Reference — Selective Merge
version: 1.2
status: Approved Reference
owner: KB Owner
scope: One Bangkok SOC Orientation operational knowledge
source: User-provided operational knowledge, selectively approved by KB Owner
updated: 2026-09-10
---

# SOC Orientation Operational Reference — Selective Merge

## 1. Governance and Precedence

This file contains KB Owner-approved non-conflicting operational knowledge from SOC Orientation and subsequent approved clarifications.

Rules:
1. Approved non-conflicting information recorded below is available for Skills Hunter use.
2. Supporting information does not replace more specific Approved/Active sources.
3. Conflicting source information is quarantined under Knowledge Conflicts and MUST NOT override existing Approved/Active knowledge.
4. Missing details remain Knowledge Gaps.
5. Emergency-code canonical definitions and specific approved SOPs take precedence over this orientation-level reference.

## 2. Approved New Knowledge

### 2.1 Building / Project Facts
- **Multi-Purpose Hall**: capacity for concerts and exhibitions is **up to 6,000 people**.
- One Bangkok project area: **108 rai**.
- Total usable/floor area stated by source: **1.93 million sq.m.**
- Premium Grade A office: **5 buildings**, total stated area **>500,000 sq.m.**
- Retail: stated area **>190,000 sq.m.**
- Residence: **3 projects**.
- Hotel: **5 buildings**.

Do not infer event-specific safe occupancy, evacuation capacity, fire-code occupant load, or permitted attendance from the 6,000-person statement unless separately approved.

### 2.2 SOC Seating / Coverage Structure
SOC seating is described as **Front Line** and **Back Line**, with a **Command Station** and **Video Wall** controlled by the **SOC Supervisor**.

| Seat / Coverage | Responsibility |
|---|---|
| **Z1** | Parade, MRT Link A, Tower 3, Tower 2, Frasers Suite |
| **Z2** | The Storeys, Tower 4, MRT Link B, Andaz, Pathom House |
| **Z3** | ONE89 Wireless, EI8HTEEN SEVEN, Tower 5, POST1928, The Ritz-Carlton |
| **Z4** | Forum, One Power, P5 Parking, One Bangkok Tower, R4, P5 Residential |
| **TR** | I/O Traffic — Entrance, Loading, Drop-Off |
| **SE** | Security Coordination / CI — Boundary, Parks, Basement |
| **A1** | Assets 1 — The PARQ, FYI, Samyan Mitrtown |

This is SOC Seat Coverage and must not silently redefine approved site Zone boundaries.

### 2.3 SOC Daily Routine
- **Prework Checklist** through OpsApp before each shift: equipment, CCTV cameras in assigned zone, software/program systems.
- **Virtual Patrol** through CCTV every hour.
- **Guard Tour Monitoring**.
- **HOTO — Hand Over / Take Over**.
- **Shift Report**.

### 2.4 Virtual Patrol — Camera Abnormality Classification
| Type | Classification | Escalation |
|---|---|---|
| **Type 1** | Technical | TCC Tech / Vision |
| **Type 2** | Environmental | Security field team |
| **Type 3** | Operational | SOC Manager |

Do not infer severity, SLA, closure criteria, or additional escalation steps not provided.

### 2.5 Threat Level
| Level | Description |
|---|---|
| **Green** | Normal situation |
| **Yellow** | Broad/global threat that is not specific |
| **Orange** | Threat affecting mixed-use / landmark targets in Thailand |
| **Red** | Threat near One Bangkok or affecting related businesses |
| **Black** | Threat specifically targeting One Bangkok, or currently occurring to nearby businesses |

Authority to determine/escalate Threat Level: **AVP of Integrated Ops Control**, based on intelligence.

Response actions for each level remain unspecified.

### 2.6 DCC / ONE POWER
- **District Command Center (DCC)** is located at **ONE POWER**.
- ONE POWER is the former **CUP** building.
- Source building data: **28,878 sq.m., 15 floors, B4–L10**.
- DCC includes **FMC, SOC, Contact Center, and ICT**.
- Joint project-management entities named by source: **JLL** and **Senses Property Management**.
- **TCC Technology (TCCT)** is responsible for Smart City systems.
- SOC team structure was stated to be **under revision** in the orientation source.

#### ICT — Approved Role
- **ICT = Information & Communication Technology**.
- ICT is one of the units operating at the **District Command Center (DCC), ONE POWER**.
- ICT's primary role is **ดูแลระบบเทคโนโลยีของโครงการ (maintain/support the project's technology systems)**.

Guardrail: this approved statement does not define ICT's detailed scope, escalation authority, staffing, SLA, or ownership of each individual system unless separately confirmed.

### 2.7 MOZART — Organization and Orientation-Level Workflow
**MOZART** is the main web application for case management and operational coordination and is maintained by **TCC Technology / CERTIS**.

```text
Incident / report received
→ SOC Operator opens Case in MOZART
→ DCC receives report
→ SOC Supervisor manages Case
→ Security-Ops receives work through OpsApp / POC
→ Case closed after resolution
```

This high-level workflow does not replace specific approved emergency-code Mozart workflows, automatic device-created Case behavior, CAT/SLA rules, or closure requirements documented elsewhere.

### 2.8 Smart City / SOC Operational Systems — Approved Ownership Knowledge
The approved clarification states that Smart City operational systems and software used by SOC, including **MOZART, OpsApp & CMS, and SenseStudio**, are developed and maintained/supported by **TCC Technology (TCCT)**. For MOZART, the earlier approved orientation reference also identifies **TCC Technology / CERTIS** in maintenance; do not infer exclusive single-vendor ownership without further evidence.

#### System Ownership Matrix — Current Approved Scope
| System / Platform | Vendor / Maintainer | Function / Scope | Approved operational note |
|---|---|---|---|
| **MOZART** | **TCC Technology / CERTIS** | Main web application for Case Management and operational coordination | Case is recorded in MOZART for onward coordination with DCC and Security-Ops |
| **Qognify VMS** | **Vision** | Primary CCTV VMS; CCTV viewing and elevator Intercom | For Type 1 Technical camera issues, create a MOZART case and coordinate **TCC Technology / Vision** |
| **HikCentral** | **Forward System** | Management of Guidance cameras and Barrier Cameras | Record/open case in MOZART |
| **EASY 7** | **Frasers (FM)** | Mobile & Temporary CCTV | Record/open case in MOZART |
| **Dispatcher Hytalk** | **Not confirmed** | Main two-way radio communication application between POC | Vendor remains Knowledge Gap; emergency-channel wording is quarantined under KC-06 |
| **OpsApp & CMS** | **TCC Technology (TCCT)** | Operational management; Prework equipment/camera checks before shift and case sending/receiving | Supporting confirmation of previously approved TCCT ownership/support |
| **SenseStudio** | **TCC Technology (TCCT)** | AI backend: Video Analytics, AI Detection, Facial Recognition | Supporting confirmation of previously approved TCCT ownership/support |
| **DTC GPS** | **DTC** | Golf-cart CCTV viewing and GPS tracking | Record/open case in MOZART |
| **Honeywell** | **Honeywell / Shinasub** | Access Control operation and monitoring | Record/open case in MOZART |
| **Security Desk** | **Forward System** | Smart Pole operation and monitoring | Record/open case in MOZART |

Guardrails:
- **ICT and TCCT must not be treated as the same organizational unit.**
- Do not infer exclusive ownership, first-line/second-line support, escalation authority, contact person, SLA, or technical scope beyond the confirmed statements above.
- For **Honeywell / Shinasub**, the exact division of responsibility between the two parties is not yet confirmed.
- For **Dispatcher Hytalk**, vendor/maintainer is not confirmed.

## 3. Supporting Reference — Consistent with Existing Knowledge
- MOZART → TCC Technology / CERTIS is consistent with existing approved orientation knowledge.
- OpsApp & CMS → TCC Technology is supporting confirmation of existing approved knowledge.
- SenseStudio → TCC Technology is supporting confirmation of existing approved knowledge.
- Qognify VMS → Vision is consistent with the existing approved Virtual Patrol Type 1 Technical escalation to TCC Tech / Vision.
- Orientation material supports overlapping site zoning relationships and broadly supports **Code 2 = Real Fire**; more specific approved sources remain authoritative.

## 4. Knowledge Conflicts — QUARANTINED / DO NOT OVERRIDE

### KC-01 — Code 1 Definition
Orientation wording `CODE 1 (RECEIVE / VERIFY)` does not override canonical **Code 1 = รับรู้/รับแจ้ง (Acknowledge)**.

### KC-02 — Code 3 Trigger
Orientation sequence `คุมเพลิงไม่ได้ → Evacuate / Respond` does not override approved Code 3 knowledge.

### KC-03 — EMER_1 / EMER_2 Wording
Orientation `EMER_1 / EMER_2` notation must not be interpreted as making both channels interchangeable. Specific approved emergency-channel knowledge takes precedence.

### KC-04 — “Water Cut Authorization”
Orientation wording equivalent to `ขออนุมัติตัดน้ำ (Water Cut Authorization)` conflicts with specific Code 2 knowledge describing electrical isolation before water suppression. It requires clarification before SOP change.

### KC-05 — CAT1 / CAT2 Orientation Classification
Orientation CAT1/CAT2 wording must not replace existing specific Code 1 CAT/SLA taxonomy until explicitly reconciled and approved.

### KC-06 — Dispatcher Hytalk Emergency Channel Wording
The System Ownership Matrix source states that for Code 2/3 the radio should be switched to **EMER_1 / EMER_2**. This wording is quarantined and MUST NOT be used to imply that EMER_1 and EMER_2 are interchangeable or equally primary. Existing more specific approved emergency-channel knowledge remains authoritative.

## 5. Knowledge Gaps — Remain Open
- **MOZART**: mandatory/required fields, SLA by Priority, real Case Log examples.
- **Emergency Codes**: other emergency codes and declaration authority for each Code; check specific Sierra reference before declaring repository-wide gap.
- **SOC SOP / Escalation**: detailed Escalation Matrix, Radio Channel Map, Call Sign, standard radio-message format.
- **Organization**: confirmed definition, role and authority of **ERT**; complete confirmed Org Chart.
- **System Ownership / Support Matrix**:
  - individual Contact Persons for TCCT, Vision, Forward System, Honeywell, Shinasub, DTC and other vendors;
  - Vendor Escalation Matrix / escalation sequence;
  - System Downtime SLA / response and restoration targets;
  - confirmed vendor/maintainer for Dispatcher Hytalk;
  - precise responsibility split between Honeywell and Shinasub.
- **Site Knowledge within this orientation source**: Assembly Points, Fire Truck Parking, Ambulance Pickup, approved emergency routes; check separate approved references before declaring repository-wide gap.

## 6. AI Retrieval Rules
1. Use Section 2 as approved orientation-derived/KB Owner-approved knowledge.
2. Use Section 3 only as supporting evidence and retrieve more specific primary references for operational answers.
3. Never use Section 4 conflict wording as authoritative SOP.
4. For Section 5 gaps, check other routed Skills Hunter files before declaring repository-wide Knowledge Gap.
5. Latest Approved/Active and more specific approved emergency SOP knowledge overrides this orientation-level reference when conflict exists.

## Change Log
- v1.2 — 2026-09-10 — KB Owner approved Selective Merge of the System Ownership Matrix: accepted non-conflicting System→Vendor→Function mappings; retained MOZART/OpsApp/SenseStudio as supporting confirmation; added Qognify VMS, HikCentral, EASY 7, DTC GPS, Honeywell and Security Desk mappings; quarantined Dispatcher Hytalk `EMER_1 / EMER_2` wording; retained Contact Persons, Vendor Escalation Matrix, System Downtime SLA and Hytalk vendor as Knowledge Gaps.
- v1.1 — 2026-09-10 — KB Owner approved ICT definition/role and TCCT support/development knowledge for MOZART, OpsApp & CMS, and SenseStudio; added initial System Ownership Matrix and retained unmapped Vision/Forward System/Honeywell details as Knowledge Gaps.
- v1.0 — 2026-09-10 — KB Owner approved Selective Merge of non-conflicting SOC Orientation operational knowledge; consistent information retained as Supporting Reference; conflicts quarantined; Knowledge Gaps preserved.
