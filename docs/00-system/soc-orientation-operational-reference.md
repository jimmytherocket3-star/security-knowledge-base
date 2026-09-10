---
document_id: SEC-SYSTEM-SOC-ORIENTATION-OPS-001
title: SOC Orientation Operational Reference — Selective Merge
version: 1.0
status: Approved Reference
owner: KB Owner
scope: One Bangkok SOC Orientation operational knowledge
source: User-provided `ข้อมูลเชิงปฏิบัติการ.md`, selectively approved by KB Owner on 2026-09-10
updated: 2026-09-10
---

# SOC Orientation Operational Reference — Selective Merge

## 1. Governance and Precedence

This file is a **Selective Merge** of the KB Owner-approved non-conflicting operational knowledge from the SOC Orientation source.

Rules:

1. New non-conflicting information recorded below is approved for Skills Hunter use.
2. Information that agrees with existing Skills Hunter knowledge is retained as a **Supporting Reference** only and does not replace the more specific source.
3. Conflicting information from the source is quarantined under **Knowledge Conflicts** and MUST NOT override existing Approved/Active or more specific approved knowledge.
4. Source-identified missing details remain **Knowledge Gaps**.
5. Emergency-code canonical definitions and specific approved SOPs take precedence over this orientation-level reference.

## 2. Approved New Knowledge

### 2.1 Building / Project Facts

- **Multi-Purpose Hall**: source states capacity for concerts and exhibitions is **up to 6,000 people**.
- One Bangkok project area: **108 rai**.
- Total usable/floor area stated by source: **1.93 million sq.m.**
- Premium Grade A office: **5 buildings**, total stated area **>500,000 sq.m.**
- Retail: stated area **>190,000 sq.m.**
- Residence: **3 projects**.
- Hotel: **5 buildings**.

These are orientation-source project facts. Do not infer event-specific safe occupancy, evacuation capacity, fire-code occupant load, or permitted attendance from the 6,000-person statement unless separately approved.

### 2.2 SOC Seating / Coverage Structure

The source describes SOC seating as **Front Line** and **Back Line**, with a **Command Station** and **Video Wall** controlled by the **SOC Supervisor**.

Seat Coverage:

| Seat / Coverage | Source-listed responsibility |
|---|---|
| **Z1** | Parade, MRT Link A, Tower 3, Tower 2, Frasers Suite |
| **Z2** | The Storeys, Tower 4, MRT Link B, Andaz, Pathom House |
| **Z3** | ONE89 Wireless, EI8HTEEN SEVEN, Tower 5, POST1928, The Ritz-Carlton |
| **Z4** | Forum, One Power, P5 Parking, One Bangkok Tower, R4, P5 Residential |
| **TR** | I/O Traffic — Entrance, Loading, Drop-Off |
| **SE** | Security Coordination / CI — Boundary, Parks, Basement |
| **A1** | Assets 1 — The PARQ, FYI, Samyan Mitrtown |

This is **SOC Seat Coverage** from the orientation source. It must not be used to silently redefine approved site Zone boundaries beyond mappings separately approved in the Location & Building Directory.

### 2.3 SOC Daily Routine

The source records:

- **Prework Checklist** through OpsApp before each shift, covering equipment, CCTV cameras in the assigned zone, and software/program systems.
- **Virtual Patrol** through CCTV every hour.
- **Guard Tour Monitoring**.
- **HOTO — Hand Over / Take Over**.
- **Shift Report**.

### 2.4 Virtual Patrol — Camera Abnormality Classification

When CCTV abnormalities are found during Virtual Patrol, the source classifies them as:

| Type | Classification | Source-listed escalation |
|---|---|---|
| **Type 1** | Technical | TCC Tech / Vision |
| **Type 2** | Environmental | Security field team |
| **Type 3** | Operational | SOC Manager |

Do not infer severity, SLA, closure criteria, or additional escalation steps not provided by the source.

### 2.5 Threat Level

The source defines **5 Threat Levels**:

| Level | Source description |
|---|---|
| **Green** | Normal situation |
| **Yellow** | Broad/global threat that is not specific |
| **Orange** | Threat affecting mixed-use / landmark targets in Thailand |
| **Red** | Threat near One Bangkok or affecting related businesses |
| **Black** | Threat specifically targeting One Bangkok, or currently occurring to nearby businesses |

The source states the authority to determine/escalate Threat Level is **AVP of Integrated Ops Control**, based on intelligence.

This reference does not add response actions for each level because the source does not provide them.

### 2.6 DCC / ONE POWER

The source states:

- **District Command Center (DCC)** is located at **ONE POWER**.
- ONE POWER is described in the source as the former **CUP** building.
- Source building data: **28,878 sq.m., 15 floors, B4–L10**.
- DCC includes **FMC, SOC, Contact Center, and ICT**.
- Joint project-management entities named by the source: **JLL** and **Senses Property Management**.
- **TCC Technology (TCCT)** is stated as responsible for Smart City systems.
- The SOC team structure is stated to be **under revision** in the orientation document.

### 2.7 MOZART — Organization and Orientation-Level Workflow

The source describes **MOZART** as the main web application for case management and operational coordination, and states that the system is maintained by **TCC Technology / CERTIS**.

Orientation-level workflow recorded by the source:

```text
Incident / report received
→ SOC Operator opens Case in MOZART
→ DCC receives report
→ SOC Supervisor manages Case
→ Security-Ops receives work through OpsApp / POC
→ Case closed after resolution
```

This is a high-level orientation workflow. It does not replace specific approved emergency-code Mozart workflows, automatic device-created Case behavior, CAT/SLA rules, or closure requirements documented elsewhere.

## 3. Supporting Reference — Consistent with Existing Knowledge

The orientation source also supports existing site zoning relationships including:

- Z1: Parade, Tower 3, Tower 2, Frasers Suite
- Z2: The Storeys, Tower 4, Andaz, Pathom House
- Z3: ONE89 Wireless, EI8HTEEN SEVEN, Tower 5, POST1928, The Ritz-Carlton
- Z4: Forum, One Bangkok Tower

For direct Building → Zone answers, the approved `location-building-directory.md` mapping remains the primary reference.

The orientation source also describes Code 2 as a confirmed smoke/fire condition, which is broadly consistent with the canonical **Code 2 = Real Fire** definition. The canonical emergency-code definition remains authoritative.

## 4. Knowledge Conflicts — QUARANTINED / DO NOT OVERRIDE

The following source statements are preserved only to document conflicts. They are **not approved as replacements** for current Skills Hunter emergency knowledge.

### KC-01 — Code 1 Definition

Orientation source wording: `CODE 1 (RECEIVE / VERIFY)`.

Current Skills Hunter canonical definition remains:

**Code 1 = รับรู้/รับแจ้ง (Acknowledge)**.

`RECEIVE / VERIFY` must not override the canonical definition. Verification may remain part of procedure where separately approved.

### KC-02 — Code 3 Trigger

Orientation source describes Code 3 in the sequence `คุมเพลิงไม่ได้ → Evacuate / Respond`.

Current Skills Hunter Code 3 knowledge states **Code 3 = Evacuation** and does **not** require waiting until EOT/fire brigade cannot control the fire. Approved Code 3 triggers remain the specific System Trigger / Command Trigger knowledge documented in the Code 3 file.

### KC-03 — EMER_1 / EMER_2 Wording

Orientation source uses `EMER_1 / EMER_2` in its Code 2 summary.

Do not interpret this notation as making both channels interchangeable. Existing specific emergency-channel knowledge takes precedence, including primary/backup distinctions where approved.

### KC-04 — “Water Cut Authorization”

Orientation source contains wording equivalent to `ขออนุมัติตัดน้ำ (Water Cut Authorization)`.

This conflicts with the specific Code 2 knowledge describing **electrical isolation before water suppression**. The orientation wording must not override the specific Code 2 procedure and requires clarification before any SOP change.

### KC-05 — CAT1 / CAT2 Orientation Classification

The orientation source describes:

- CAT1 (Critical): examples include confirmed fire Code 2/3, critical medical emergency, direct threat; managed/coordinated by SOC Supervisor.
- CAT2 (Non-Critical): examples include False Alarm investigation or minor events handled through normal operations.

Existing specific Code 1 knowledge states **Code 1 = CAT1** with Mozart Acknowledge SLA ≤5 minutes. Therefore the orientation CAT1/CAT2 explanation must not replace the existing CAT/SLA taxonomy until the relationship is explicitly reconciled and approved by KB Owner.

## 5. Knowledge Gaps — Remain Open

The source itself identifies missing operational detail. These remain Knowledge Gaps:

- **MOZART**: mandatory/required fields, SLA by Priority, real Case Log examples.
- **Emergency Codes**: Code Sierra detail in this orientation source, other emergency codes, and declaration authority for each Code.
- **SOC SOP / Escalation**: detailed Escalation Matrix by person/position, Radio Channel Map, Call Sign, standard radio-message format.
- **Organization**: confirmed definition, role and authority of **ERT**; complete confirmed Org Chart.
- **Site Knowledge** within this orientation source: Assembly Points, Fire Truck Parking, Ambulance Pickup, approved emergency routes. These topics may already have separate approved Skills Hunter references; their absence from the orientation source must not erase those references.

## 6. AI Retrieval Rules

When answering from this file:

1. Use Section 2 as approved orientation-derived knowledge.
2. Use Section 3 only as supporting evidence; retrieve the more specific primary reference for operational answers.
3. Never answer using Section 4 conflict wording as the authoritative SOP.
4. For Section 5 gaps, check other routed Skills Hunter files before declaring a repository-wide Knowledge Gap.
5. Latest Approved/Active and more specific approved emergency SOP knowledge overrides this orientation-level reference when conflict exists.

## Change Log

- v1.0 — 2026-09-10 — KB Owner approved Selective Merge: accepted non-conflicting Building/Project Facts, SOC Seat Coverage, Daily Routine, Virtual Patrol classification, Threat Level, DCC/ONE POWER, and MOZART organization/workflow; retained consistent information as Supporting Reference; quarantined identified conflicts without overriding existing knowledge; preserved Knowledge Gaps.
