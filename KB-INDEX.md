---
document_id: SEC-KB-INDEX-001
title: Skills Hunter — Security Knowledge Base Retrieval Index
version: 1.6
status: Active
owner: KB Owner
scope: AI Retrieval / Repository Routing
updated: 2026-09-10
---

# Skills Hunter — Security Knowledge Base Retrieval Index

## Skills Hunter Identity

**Skills Hunter** is the display / conversational name of this Knowledge Base. The technical repository remains `jimmytherocket3-star/security-knowledge-base` and all existing repository paths remain unchanged.

When the user says `Skills Hunter`, `ค้นใน Skills Hunter`, `หาใน Skills Hunter`, `บันทึกเข้า Skills Hunter`, or equivalent wording, treat it as a direct reference to this Knowledge Base and apply the same retrieval, source-priority, and governance rules.

## Purpose

This file is the primary routing index for AI retrieval in `jimmytherocket3-star/security-knowledge-base`.

When answering a question from Skills Hunter, use this index to identify the most relevant source file and fetch/read that file directly. A failed GitHub search alone is not evidence that Skills Hunter lacks the information.

## Mandatory Retrieval Rule

1. Read this index first when the relevant Skills Hunter file is not already known.
2. Route the question to the most relevant file below.
3. Fetch/read the target file directly rather than relying only on repository search.
4. Prefer the latest Approved/Active material when sources conflict, subject to document-specific status and guardrails.
5. If search returns no result, check the routed file directly before declaring a Knowledge Gap.
6. Declare a Knowledge Gap only after the relevant routed source has been checked and does not support the requested fact.
7. Never invent internal facts or silently replace missing internal information with external information.
8. Skills Hunter create/edit/delete operations require explicit KB Owner approval before modification.

## Answer Source Status Labels

Every factual answer using Skills Hunter must clearly display the source status to the user.

- **✅ SKILLS HUNTER — APPROVED** — Use when the answer is supported by information retrieved and verified from the GitHub Knowledge Base. This label is the display-name equivalent of the former `✅ KB APPROVED` label. The answer must follow the status, scope, version, and guardrails of the source document.
- **⚠️ KNOWLEDGE GAP — ไม่พบข้อมูลใน Skills Hunter** — Use when the relevant routed source has been checked and the requested information is absent or unsupported. Do not guess.
- **🌐 EXTERNAL — ข้อมูลภายนอก Skills Hunter** — Use when information comes from outside the GitHub Knowledge Base. Keep external information clearly separated from Skills Hunter-derived information.

If an answer combines Skills Hunter-derived and external information, label the respective portions separately. A GitHub repository search miss alone is not sufficient to use the Knowledge Gap label; the relevant routed source must be checked directly first.

## Routing Table

| Question / Topic | Primary KB File | Retrieval Note |
|---|---|---|
| Skills Hunter identity / Knowledge Base branding | `docs/00-system/skills-hunter.md` | Skills Hunter is the display name of this Knowledge Base; repository and paths remain unchanged. |
| One00, One01, One02, One03, One04, One05; management personnel names/nicknames | `docs/00-system/management-personnel-reference.md` | Fetch directly for One00–One05 questions. Do not rely on search alone. |
| Building names, locations, Zone/Zoning, Loading 1–8, site labels | `docs/00-system/location-building-directory.md` | Use for approved location/building/loading mappings. |
| ทางเข้า-ออกโครงการ, Traffic Knowledge, ทางเข้า One Bangkok, รถยนต์เข้าโครงการ, รถจักรยานยนต์เข้าโครงการ, MRT connection, รถประจำทาง, Helipad | `docs/00-system/traffic-access-reference.md` | Fetch directly for approved project access counts/source roads, motorcycle entrances, public-transport connection, and Tower 4 Helipad. Do not infer unlisted Entrance numbers, routes, traffic direction, or operating hours. |
| Multi-Purpose Hall, อาคารอเนกประสงค์, ความจุอาคารอเนกประสงค์, project area/พื้นที่โครงการ, SOC orientation operational facts | `docs/00-system/soc-orientation-operational-reference.md` | Fetch directly for approved Multi-Purpose Hall capacity and SOC orientation operational facts; do not infer event-specific safe occupancy, evacuation capacity, fire-code occupant load, or permitted attendance. |
| จุดรวมพล, Assembly Point, จุดอพยพ/พื้นที่รวมพล | `docs/00-system/assembly-point-reference.md` | Fetch directly for Assembly Point location questions. Do not infer Building → Assembly Point mapping unless explicitly supported. |
| จุดจอดรถดับเพลิง, Fire Truck Parking, รถดับเพลิงจอดที่ไหน, จุดจอดรถดับเพลิงของอาคาร | `docs/00-system/fire-truck-parking-reference.md` | Fetch directly for building-specific fire truck parking questions. Numbers 1–5 are fire truck parking points, not Assembly Points. |
| โรงพยาบาล, Hospital, โรงพยาบาลนำส่งผู้ป่วย, ส่งฟรี, ค่านำส่ง, โรงพยาบาลภายใน 5 กม., โรงพยาบาลภายใน 10 กม. | `docs/00-system/hospital-transport-reference.md` | Fetch directly for approved hospital transport groups and source-stated transport conditions. “ส่งฟรี” refers to transport condition only, not free medical treatment. Do not recalculate distance or reclassify hospitals. |
| Internal/external emergency contacts, BMO, SOC, DCC, FMC, hotel contacts, First Aid | `docs/00-system/emergency-contact-directory.md` | Blank/unconfirmed values must not be guessed. For hospital transport conditions, route to hospital-transport-reference.md; use this directory for approved phone numbers. |
| MOD duty schedule for May 2026 | `docs/00-system/mod-duty-schedule/2026-05.md` | Time-bound reference only; do not treat as permanent contact data. |
| Terminology, abbreviations, roles, EMER_1/EMER_2, BMO, DCC, IMT, EOT, SOC, FCC, General Alarm, Assembly Point definition | `docs/00-system/terminology.md` | Use canonical terminology definitions. For Assembly Point locations, route to assembly-point-reference.md. |
| Canonical Code 1, Code 2, Code 3 definitions | `docs/01-emergency-codes/code-definitions.md` | Use as primary source for code definitions. |
| Code 1 detailed workflow/reference | `docs/01-emergency-codes/code-1/overview.md` | Check status/version and defer to canonical definitions where conflicting. |
| Code 2 detailed workflow/reference | `docs/01-emergency-codes/code-2/overview.md` | Check status/version and defer to canonical definitions where conflicting. |
| Code 3 / Evacuation procedure | `docs/01-emergency-codes/code-3/overview.md` | Use latest approved Code 3 procedure. |
| Code Sierra / Active Shooter | `docs/01-emergency-codes/code-sierra/overview.md` | Use current stored canonical document; do not silently apply unapproved corrections. |
| ONE89 Wireless residential fire evacuation drill 2026 | `docs/02-building-procedures/residential/one89-wireless/2026-fire-evacuation-drill.md` | Drill-specific/residential reference; do not generalize to all buildings. |
| GitHub KB-first retrieval behavior and source priority | `docs/00-system/github-kb-first-retrieval-policy.md` | Governs Skills Hunter / KB-first retrieval behavior. |
| Assistant persona / Kuroro | `docs/00-system/assistant-persona.md` | Persona only; does not alter SOP authority. |

## Query Routing Examples

- `Skills Hunter คืออะไร` → fetch `docs/00-system/skills-hunter.md`
- `One 04 ชื่ออะไร` → fetch `docs/00-system/management-personnel-reference.md`
- `One 00 ชื่ออะไร` → fetch `docs/00-system/management-personnel-reference.md`
- `Loading 5 เป็นของอาคารอะไร` → fetch `docs/00-system/location-building-directory.md`
- `Zone 3 มีอาคารอะไรบ้าง` → fetch `docs/00-system/location-building-directory.md`
- `ทางเข้า-ออกโครงการมีกี่ทาง` → fetch `docs/00-system/traffic-access-reference.md`
- `รถยนต์เข้า One Bangkok ได้กี่ทาง` → fetch `docs/00-system/traffic-access-reference.md`
- `รถจักรยานยนต์เข้าทางไหน` → fetch `docs/00-system/traffic-access-reference.md`
- `Helipad อยู่ที่ไหน` → fetch `docs/00-system/traffic-access-reference.md`
- `อาคารอเนกประสงค์บรรจุได้กี่คน` → fetch `docs/00-system/soc-orientation-operational-reference.md`
- `Multi-Purpose Hall รองรับได้กี่คน` → fetch `docs/00-system/soc-orientation-operational-reference.md`
- `One Bangkok มีพื้นที่เท่าไหร่` → fetch `docs/00-system/soc-orientation-operational-reference.md`
- `จุดรวมพลอยู่ที่ไหน` → fetch `docs/00-system/assembly-point-reference.md`
- `Assembly Point อยู่ที่ไหน` → fetch `docs/00-system/assembly-point-reference.md`
- `Tower 5 จุดรวมพลอยู่ที่ไหน` → fetch `docs/00-system/assembly-point-reference.md`; if no approved Building → Assembly Point mapping exists, return Knowledge Gap rather than infer from map position
- `Tower 5 รถดับเพลิงจอดที่ไหน` → fetch `docs/00-system/fire-truck-parking-reference.md`
- `จุดจอดรถดับเพลิง Tower 3` → fetch `docs/00-system/fire-truck-parking-reference.md`
- `ขอชื่อโรงพยาบาลที่นำส่งผู้ป่วยแล้วไม่เสียค่าใช้จ่าย` → fetch `docs/00-system/hospital-transport-reference.md`; explain that “ส่งฟรี” is the source-stated transport condition, not free treatment
- `โรงพยาบาลเอกชนภายใน 5 กม. มีที่ไหนบ้าง` → fetch `docs/00-system/hospital-transport-reference.md`
- `โรงพยาบาล 6–10 กม. ค่านำส่งเท่าไหร่` → fetch `docs/00-system/hospital-transport-reference.md`
- `เบอร์ MedPark` → fetch `docs/00-system/emergency-contact-directory.md`; transport-condition questions route to `hospital-transport-reference.md`
- `เบอร์ SOC` → fetch `docs/00-system/emergency-contact-directory.md`
- `Code 3 คืออะไร` → fetch `docs/01-emergency-codes/code-definitions.md`, then `docs/01-emergency-codes/code-3/overview.md` if procedural detail is requested
- `Code Sierra` → fetch `docs/01-emergency-codes/code-sierra/overview.md`
- `จุดรวมพล ONE89 ตามแผนซ้อม` → fetch `docs/02-building-procedures/residential/one89-wireless/2026-fire-evacuation-drill.md`

## Source Priority

`Latest Approved/Active Skills Hunter Knowledge → Approved Reference → Knowledge Gap → External source only when explicitly requested or clearly separated`

A repository search miss does **not** move the answer directly to Knowledge Gap. The routed source file must be checked first.

## Guardrails

- Skills Hunter is a branding layer over the existing Security Knowledge Base; it does not create new SOP facts.
- This index routes retrieval; it does not create new SOP facts.
- File status and document-specific guardrails remain authoritative.
- Do not infer emergency authority from personnel/location/contact reference files.
- Do not normalize source spellings or aliases unless explicitly approved.
- Do not generalize drill-specific procedures into Core SOP.
- Do not infer Building → Assembly Point mapping from visual proximity on a map unless an approved source explicitly maps them.
- Fire Truck Parking Points 1–5 must never be interpreted as Assembly Point numbers.
- For hospital transport questions, preserve the approved source grouping. Do not infer that free transport means free treatment, and do not recalculate distance to move hospitals between groups.
- For Traffic Knowledge, do not infer Entrance numbers, vehicle routes, traffic direction, opening hours, or access restrictions beyond the approved source. Treat construction status as time-sensitive source information.
- Do not modify this index or any routed file without explicit KB Owner approval.

## Change Log

- v1.6 — 2026-09-10 — Added direct routing for Traffic Knowledge / project entrance-exit questions to `traffic-access-reference.md`, including car access, motorcycle access, MRT/public transport, and Helipad queries; added traffic-specific retrieval guardrails.
- v1.5 — 2026-09-10 — Added direct routing for hospital transport questions to `hospital-transport-reference.md`, including free-transport, 5 km/10 km, and 6–10 km transport-fee queries; cross-routed hospital phone-number questions to the Emergency Contact Directory and added transport-specific guardrails.
- v1.4 — 2026-09-10 — Added direct routing for Multi-Purpose Hall / อาคารอเนกประสงค์ capacity, One Bangkok project-area questions, and SOC orientation operational facts to `soc-orientation-operational-reference.md`; added query examples to prevent false Knowledge Gaps caused by routing these questions to the location directory.
- v1.3 — 2026-09-08 — Added Skills Hunter as the display / conversational identity of the existing Security Knowledge Base, added direct routing to the Skills Hunter identity document, and updated answer labels while preserving the repository and file paths.
- v1.2 — 2026-09-08 — Added direct routing for Assembly Point and Fire Truck Parking references and query examples.
- v1.1 — 2026-09-08 — Added mandatory answer source status labels: KB APPROVED, KNOWLEDGE GAP, and EXTERNAL.
- v1.0 — 2026-09-08 — Created as the central AI retrieval/router index to reduce false Knowledge Gaps caused by repository search misses.
