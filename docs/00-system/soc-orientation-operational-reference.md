---
document_id: SEC-SYSTEM-SOC-ORIENTATION-OPS-001
title: SOC Orientation Operational Reference — Selective Merge
version: 1.1
status: Approved Reference
owner: KB Owner
scope: One Bangkok SOC Orientation operational knowledge
source: User-provided operational knowledge, selectively approved by KB Owner
updated: 2026-09-10
---

# SOC Orientation Operational Reference — Selective Merge

## 1. Governance and Precedence

This file contains KB Owner-approved non-conflicting operational knowledge from SOC Orientation and subsequent approved clarification.

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
The approved clarification states that Smart City operational systems and software used by SOC, including:

- **MOZART**
- **OpsApp & CMS**
- **SenseStudio**

are developed and maintained/supported by **TCC Technology (TCCT)**.

For **MOZART**, the earlier approved orientation reference also identifies **TCC Technology / CERTIS** in system maintenance. This statement is retained; do not infer an exclusive single-vendor ownership model without further evidence.

#### System Ownership Matrix — Current Confirmed Scope
| System / Platform | Confirmed developer / maintainer / support | Status |
|---|---|---|
| MOZART | TCC Technology (TCCT); orientation reference also identifies CERTIS in maintenance | Confirmed at current approved scope |
| OpsApp & CMS | TCC Technology (TCCT) | Confirmed at current approved scope |
| SenseStudio | TCC Technology (TCCT) | Confirmed at current approved scope |
| Other Vision systems | Not yet sufficiently mapped by specific system | Knowledge Gap |
| Forward System | Not yet sufficiently mapped | Knowledge Gap |
| Honeywell systems | Not yet sufficiently mapped | Knowledge Gap |

Guardrails:
- **ICT and TCCT must not be treated as the same organizational unit.**
- Do not infer vendor ownership, first-line support, escalation sequence, contact person, SLA, or technical scope beyond the confirmed statements above.

## 3. Supporting Reference — Consistent with Existing Knowledge
Orientation material supports existing site zoning relationships for overlapping buildings and supports **Code 2 = Real Fire** broadly. Direct Building → Zone answers must use the approved Location & Building Directory; canonical emergency-code definitions remain authoritative.

## 4. Knowledge Conflicts — QUARANTINED / DO NOT OVERRIDE

### KC-01 — Code 1 Definition
Orientation wording `CODE 1 (RECEIVE / VERIFY)` does not override canonical **Code 1 = รับรู้/รับแจ้ง (Acknowledge)**. Verification may remain part of procedure where separately approved.

### KC-02 — Code 3 Trigger
Orientation sequence `คุมเพลิงไม่ได้ → Evacuate / Respond` does not override approved Code 3 knowledge. Code 3 does not require waiting until EOT/fire brigade cannot control the fire.

### KC-03 — EMER_1 / EMER_2 Wording
Orientation `EMER_1 / EMER_2` notation must not be interpreted as making both channels interchangeable. Specific approved emergency-channel knowledge takes precedence.

### KC-04 — “Water Cut Authorization”
Orientation wording equivalent to `ขออนุมัติตัดน้ำ (Water Cut Authorization)` conflicts with specific Code 2 knowledge describing electrical isolation before water suppression. It requires clarification before SOP change.

### KC-05 — CAT1 / CAT2 Orientation Classification
Orientation describes CAT1 Critical and CAT2 Non-Critical while existing specific Code 1 knowledge states Code 1 = CAT1 with Mozart Acknowledge SLA ≤5 minutes. Do not replace the existing CAT/SLA taxonomy until explicitly reconciled and approved.

## 5. Knowledge Gaps — Remain Open
- **MOZART**: mandatory/required fields, SLA by Priority, real Case Log examples.
- **Emergency Codes**: other emergency codes and declaration authority for each Code; check specific Sierra reference before declaring repository-wide gap.
- **SOC SOP / Escalation**: detailed Escalation Matrix, Radio Channel Map, Call Sign, standard radio-message format.
- **Organization**: confirmed definition, role and authority of **ERT**; complete confirmed Org Chart.
- **System Ownership / Support Matrix**: detailed mapping for Vision, Forward System, Honeywell; responsible team/person, escalation path, contact and SLA for each system.
- **Site Knowledge within this orientation source**: Assembly Points, Fire Truck Parking, Ambulance Pickup, approved emergency routes; check separate approved references before declaring repository-wide gap.

## 6. AI Retrieval Rules
1. Use Section 2 as approved orientation-derived/KB Owner-approved knowledge.
2. Use Section 3 only as supporting evidence and retrieve more specific primary references for operational answers.
3. Never use Section 4 conflict wording as authoritative SOP.
4. For Section 5 gaps, check other routed Skills Hunter files before declaring repository-wide Knowledge Gap.
5. Latest Approved/Active and more specific approved emergency SOP knowledge overrides this orientation-level reference when conflict exists.

## Change Log
- v1.1 — 2026-09-10 — KB Owner approved ICT definition/role and TCCT support/development knowledge for MOZART, OpsApp & CMS, and SenseStudio; added initial System Ownership Matrix and retained unmapped Vision/Forward System/Honeywell details as Knowledge Gaps.
- v1.0 — 2026-09-10 — KB Owner approved Selective Merge of non-conflicting SOC Orientation operational knowledge; consistent information retained as Supporting Reference; conflicts quarantined; Knowledge Gaps preserved.
