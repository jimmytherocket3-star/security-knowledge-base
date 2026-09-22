---
document_id: SEC-KB-INDEX-001
title: Skills Hunter — Security Knowledge Base Retrieval Index
version: 2.3
status: Active
owner: KB Owner
scope: AI Retrieval / Repository Routing
updated: 2026-09-22
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
4. After reading the primary source, check `docs/00-system/source-conflict-register.md` for a matching registered conflict. If one exists, read every original source listed in its record directly and report each conflicting claim with provenance; the register does not replace those sources or select a winner.
5. Prefer the latest Approved/Active material where established source priority applies, subject to document-specific status and guardrails. Generic source priority does not resolve an explicitly registered conflict between applicable sources; preserve approved canonical precedence and Draft/Active and External/Internal boundaries.
6. If search returns no result, check the routed file directly before declaring a Knowledge Gap.
7. Declare a Knowledge Gap only after the relevant routed source and any required conflict/cross-check sources have been checked and do not support the requested fact.
8. Never invent internal facts or silently replace missing internal information with external information.
9. Skills Hunter create/edit/delete operations require explicit KB Owner approval before modification.

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
| Email signature, ลายเซ็นอีเมล, company banner, โลโก้บริษัทในอีเมล, ทุกอีเมลของผู้ใช้ | `docs/00-system/email-signature-banner-standard.md` | Status: Approved. Global rule for all user email drafting: approved Sittipong signature followed immediately by the approved Senses company banner image. Never claim the banner is present unless the actual image has been inserted. |
| Guard Tour email drafting, ร่างอีเมล Guard Tour, Daily Guard Tour Report summary, Skip reason verification, ตรวจอีเมลฝ่ายอาคารกรณี Skip/ยกเลิกสแกน | `docs/00-system/guard-tour-email-drafting-standard.md` | Status: Approved. Use this standard for Guard Tour email structure, per-round reporting, Skip verification, building-email cross-checks, cancellation verification, abnormal equipment findings, attachments, recipients, and draft-version handling. Never invent a Skip reason. |
| Contact Center email drafting, รายงานการโอนสายเวลานอกเวลา, Contact Centre มายัง SOC, Case/Inquiry table, Contact Center Gmail Draft | `docs/00-system/contact-center-email-drafting-standard.md` | Status: Approved. Use for the approved Contact Center email layout, 9-column Case/Inquiry table, no recipient-contact footer, SOC follow-up contact line, approved Sittipong signature, and Senses company banner as a real inline image when the approved source image is available. Never invent missing case details. |
| Registered source conflicts / conflict tracking / `KB-CONFLICT-001`, `KB-CONFLICT-002` | `docs/00-system/source-conflict-register.md` | Retrieval-control record only; read all original sources listed in a matching record. The register does not establish new personnel, terminology, or operational facts. |
| One00, One01, One02, One03, One04, One05; management personnel names/nicknames | `docs/00-system/management-personnel-reference.md` | Fetch directly for One00–One05 questions. For One05, check `KB-CONFLICT-001` in `docs/00-system/source-conflict-register.md`, then read both original sources, including `docs/08-reference/one-bangkok-executive-callsigns.md`. Report both labels and the unresolved identity; do not select a winner. |
| Building names, locations, Zone/Zoning, Loading 1–8, site labels | `docs/00-system/location-building-directory.md` | Use for approved location/building/loading mappings. |
| Parade ambulance / patient pickup or drop-off points, รถพยาบาลรับผู้ป่วยที่ Parade | `docs/00-system/location-building-directory.md` | Primary current pickup-location reference; cross-check `docs/08-reference/one-bangkok-ambulance-pickup-dropoff-points.md`, which retains an older approved list. The directory adds Loading 1 ชั้น B1. Preserve both sources' status; do not mark the older page Superseded or infer a preferred point, priority, or route. |
| ทางเข้า-ออกโครงการ, Traffic Knowledge, ทางเข้า One Bangkok, รถยนต์เข้าโครงการ, รถจักรยานยนต์เข้าโครงการ, MRT connection, รถประจำทาง, Helipad | `docs/00-system/traffic-access-reference.md` | Fetch directly for approved project access counts/source roads, motorcycle entrances, public-transport connection, and Tower 4 Helipad. Do not infer unlisted Entrance numbers, routes, traffic direction, or operating hours. |
| Multi-Purpose Hall, อาคารอเนกประสงค์, ความจุอาคารอเนกประสงค์, project area/พื้นที่โครงการ, SOC orientation operational facts | `docs/00-system/soc-orientation-operational-reference.md` | Fetch directly for approved Multi-Purpose Hall capacity and SOC orientation operational facts; do not infer event-specific safe occupancy, evacuation capacity, fire-code occupant load, or permitted attendance. |
| กฎหมายเบื้องต้นสำหรับ SOC, SOC legal awareness, ความผิดซึ่งหน้า, การจับ/เชิญตัว, การควบคุมตัว/หน่วงเหนี่ยว, Use of Force, การค้นกระเป๋า/ตรวจค้น/ยึดสิ่งของ, PDPA + CCTV, CCTV Request, LINE และข้อมูล CCTV | `docs/00-system/soc-basic-legal-awareness-reference.md` | Approved Internal Training Reference. Fetch directly and preserve source boundaries/Knowledge Gaps. Do not treat training content as independently verified law; do not infer arrest/search/seizure/detention/use-of-force authority or missing CCTV/PDPA workflow. |
| SOC Legal Awareness source-specific CCTV / Picture / Video Retention Period questions | `docs/00-system/soc-basic-legal-awareness-reference.md` | This training reference does not state a Retention Period. If useful, separately cross-check `docs/00-system/terminology.md`; never attribute its 90-day value to SOC Legal Awareness. |
| Skills Hunter-wide CCTV / Picture / Video Retention Period questions | `docs/00-system/terminology.md` | Active canonical terminology states 90 days for Picture / Video from CCTV in the project's area and care. Cross-check `docs/00-system/soc-basic-legal-awareness-reference.md` when source provenance matters; that training reference does not supply this value. Do not infer legal retention duties or a CCTV Request workflow. |
| จุดรวมพล, Assembly Point, จุดอพยพ/พื้นที่รวมพล | `docs/00-system/assembly-point-reference.md` | Fetch directly for Assembly Point location questions. Do not infer Building → Assembly Point mapping unless explicitly supported. |
| จุดจอดรถดับเพลิง, Fire Truck Parking, รถดับเพลิงจอดที่ไหน, จุดจอดรถดับเพลิงของอาคาร | `docs/00-system/fire-truck-parking-reference.md` | Fetch directly for building-specific fire truck parking questions. Numbers 1–5 are fire truck parking points, not Assembly Points. |
| โรงพยาบาล, Hospital, โรงพยาบาลนำส่งผู้ป่วย, ส่งฟรี, ค่านำส่ง, โรงพยาบาลภายใน 5 กม., โรงพยาบาลภายใน 10 กม. | `docs/00-system/hospital-transport-reference.md` | Fetch directly for approved hospital transport groups and source-stated transport conditions. “ส่งฟรี” refers to transport condition only, not free medical treatment. Do not recalculate distance or reclassify hospitals. |
| Internal/external emergency contacts, BMO, SOC, DCC, FMC, hotel contacts, First Aid | `docs/00-system/emergency-contact-directory.md` | Blank/unconfirmed values must not be guessed. For hospital transport conditions, route to hospital-transport-reference.md; use this directory for approved phone numbers. |
| MOD duty schedule for May 2026 | `docs/00-system/mod-duty-schedule/2026-05.md` | Time-bound reference only; do not treat as permanent contact data. |
| Terminology, abbreviations, roles, EMER_1/EMER_2, BMO, DCC, IMT, EOT, SOC, FCC, General Alarm, Assembly Point definition | `docs/00-system/terminology.md` | Use canonical terminology definitions. For FCC in Code M context, also check `KB-CONFLICT-002`; do not silently replace the canonical expansion while reconciliation is pending. For Assembly Point locations, route to assembly-point-reference.md. |
| Canonical Code 1 and Code 2 definitions | `docs/01-emergency-codes/code-definitions.md` | Active canonical source for Code 1 and Code 2 definitions only; it does not define Code 3. |
| Code 1 detailed workflow/reference | `docs/01-emergency-codes/code-1/overview.md` | Check status/version and defer to canonical definitions where conflicting. |
| Code 2 detailed workflow/reference | `docs/01-emergency-codes/code-2/overview.md` | Check status/version and defer to canonical definitions where conflicting. |
| Code 3 definition / Evacuation / การอพยพ and procedure questions | `docs/01-emergency-codes/code-3/overview.md` | Status: Draft. Identify its definition and procedural content as Draft; do not present it as an Approved/Active operational procedure. `code-definitions.md` covers Code 1 and Code 2 only. |
| Code M / Medical Emergency / เหตุฉุกเฉินทางการแพทย์ / ขั้นตอน Code M | `docs/01-emergency-codes/code-m/overview.md` | Status: Approved Reference. Primary route for Code M operational procedure. Preserve its explicit Knowledge Gaps. For hospital transport and pickup-location details, follow its cross-references. Check `KB-CONFLICT-002` for the unresolved FCC expansion disagreement. |
| Code Sierra / Active Shooter | `docs/01-emergency-codes/code-sierra/overview.md` | Use current stored canonical document; do not silently apply unapproved corrections. |
| Code D, Deceased Person, พบผู้เสียชีวิต, การจัดการเหตุพบผู้เสียชีวิต | `docs/01-emergency-codes/code-d/overview.md` | Status: Approved Reference. Preserve its source scope and guardrails; do not promote it to an Active SOP or infer unsupported system configuration or authority. |
| Threat Level, Threat Response, ระดับภัยคุกคาม, การประกาศระดับภัยคุกคาม; Green, Yellow, Orange, Red, Black when threat context is clear | `docs/00-system/threat-response-procedure-reference.md` | Status: Approved Reference. Preserve the Yellow source conflict. Declaration, escalation, reduction, and cancellation authority remain a Knowledge Gap. Do not equate Threat Levels with Emergency Codes; disambiguate color-only queries. |
| ONE89 Wireless residential fire evacuation drill 2026 | `docs/02-building-procedures/residential/one89-wireless/2026-fire-evacuation-drill.md` | Drill-specific/residential reference; do not generalize to all buildings. |
| GitHub KB-first retrieval behavior and source priority | `docs/00-system/github-kb-first-retrieval-policy.md` | Governs Skills Hunter / KB-first retrieval behavior. |
| Assistant persona / Kuroro | `docs/00-system/assistant-persona.md` | Persona only; does not alter SOP authority. |

## Query Routing Examples

- `Skills Hunter คืออะไร` → fetch `docs/00-system/skills-hunter.md`
- `ใส่โลโก้บริษัทท้ายอีเมล` → fetch `docs/00-system/email-signature-banner-standard.md`; use the approved Sittipong signature and insert the approved Senses banner immediately after Mobile / Mail when the source image is available
- `ร่างอีเมล Guard Tour ให้หน่อย` → fetch `docs/00-system/guard-tour-email-drafting-standard.md`; verify all source reports, Remarks, Skip reasons, and building emails as required before drafting
- `ร่างอีเมลรายงาน Contact Center ให้หน่อย` → fetch `docs/00-system/contact-center-email-drafting-standard.md`; use the approved 9-column table, omit recipient-contact footer, preserve source facts, use the approved Sittipong signature, and render the Senses banner as a real inline image when the source image is available
- `Guard Tour มี Skip แต่ไม่มีสาเหตุ` → fetch `docs/00-system/guard-tour-email-drafting-standard.md`; do not infer a reason, cross-check related building emails, and explicitly state when no cancellation/skip instruction is found
- `One 04 ชื่ออะไร` → fetch `docs/00-system/management-personnel-reference.md`
- `One 00 ชื่ออะไร` → fetch `docs/00-system/management-personnel-reference.md`
- `One05 คือใคร` → fetch `docs/00-system/management-personnel-reference.md`, check `KB-CONFLICT-001` in `docs/00-system/source-conflict-register.md`, then read `docs/08-reference/one-bangkok-executive-callsigns.md`; report the unresolved conflict without choosing an identity
- `Loading 5 เป็นของอาคารอะไร` → fetch `docs/00-system/location-building-directory.md`
- `รถพยาบาลรับผู้ป่วยที่ Parade จุดไหน` → fetch `docs/00-system/location-building-directory.md`, then cross-check `docs/08-reference/one-bangkok-ambulance-pickup-dropoff-points.md`; include the later approved Loading 1 ชั้น B1 addition without assigning priority
- `Zone 3 มีอาคารอะไรบ้าง` → fetch `docs/00-system/location-building-directory.md`
- `ทางเข้า-ออกโครงการมีกี่ทาง` → fetch `docs/00-system/traffic-access-reference.md`
- `รถยนต์เข้า One Bangkok ได้กี่ทาง` → fetch `docs/00-system/traffic-access-reference.md`
- `รถจักรยานยนต์เข้าทางไหน` → fetch `docs/00-system/traffic-access-reference.md`
- `Helipad อยู่ที่ไหน` → fetch `docs/00-system/traffic-access-reference.md`
- `อาคารอเนกประสงค์บรรจุได้กี่คน` → fetch `docs/00-system/soc-orientation-operational-reference.md`
- `Multi-Purpose Hall รองรับได้กี่คน` → fetch `docs/00-system/soc-orientation-operational-reference.md`
- `One Bangkok มีพื้นที่เท่าไหร่` → fetch `docs/00-system/soc-orientation-operational-reference.md`
- `รปภ. บังคับค้นกระเป๋าได้ไหม` → fetch `docs/00-system/soc-basic-legal-awareness-reference.md`; preserve Internal Training Reference status and source boundary
- `ความผิดซึ่งหน้า รปภ. ทำอะไรได้บ้าง` → fetch `docs/00-system/soc-basic-legal-awareness-reference.md`; do not infer authority beyond approved training content
- `ใช้กำลังกับผู้ก่อเหตุได้แค่ไหน` → fetch `docs/00-system/soc-basic-legal-awareness-reference.md`; preserve Use-of-Force Knowledge Gaps
- `ขอภาพ CCTV ต้องทำอย่างไร` → fetch `docs/00-system/soc-basic-legal-awareness-reference.md`; if requested SOP/form/approver detail is unsupported, return Knowledge Gap
- `ส่งภาพ CCTV ใน LINE ได้ไหม` → fetch `docs/00-system/soc-basic-legal-awareness-reference.md`; distinguish approved training guidance from independently verified law
- `SOC Legal Awareness ระบุ Retention Period เท่าไร` → fetch `docs/00-system/soc-basic-legal-awareness-reference.md`; state that this source does not specify it, without attributing terminology's 90-day value to training
- `Skills Hunter มีข้อมูล CCTV Retention Period หรือไม่` → fetch `docs/00-system/terminology.md`; attribute the 90-day Picture / Video Retention term to that Active source and distinguish the SOC Legal Awareness source gap
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
- `Code 3 คืออะไร` → fetch `docs/01-emergency-codes/code-3/overview.md`; clearly label its status Draft and do not treat its content as an Approved operational procedure
- `Code M คืออะไร` → fetch `docs/01-emergency-codes/code-m/overview.md`; preserve Approved Reference status, explicit Knowledge Gaps, and `KB-CONFLICT-002` FCC terminology handling
- `ใครยืนยัน Code M` → fetch `docs/01-emergency-codes/code-m/overview.md`; return the explicit declaration/confirmation-authority Knowledge Gap rather than infer from nurse/EOT hospital-transfer confirmation
- `Code Sierra` → fetch `docs/01-emergency-codes/code-sierra/overview.md`
- `Code D คืออะไร` → fetch `docs/01-emergency-codes/code-d/overview.md`; preserve Approved Reference status
- `ใครมีอำนาจประกาศ Threat Level` → fetch `docs/00-system/threat-response-procedure-reference.md`; return the explicit authority Knowledge Gap
- `จุดรวมพล ONE89 ตามแผนซ้อม` → fetch `docs/02-building-procedures/residential/one89-wireless/2026-fire-evacuation-drill.md`

## Source Priority

`Latest Approved/Active Skills Hunter Knowledge → Approved Reference → Knowledge Gap → External source only when explicitly requested or clearly separated`

A repository search miss does **not** move the answer directly to Knowledge Gap. The routed source file must be checked first.

This generic priority does not automatically settle an explicitly registered conflict between applicable sources. Follow the conflict record's direct-source checks while retaining established canonical precedence, document status, and internal/external source boundaries.

## Guardrails

- Skills Hunter is a branding layer over the existing Security Knowledge Base; it does not create new SOP facts.
- For Guard Tour email drafting, route to `docs/00-system/guard-tour-email-drafting-standard.md`; keep results traceable to the Daily Guard Tour Report and related emails, verify Remarks/Skip/cancellation evidence, and never invent or assume a Skip reason.
- For Contact Center email drafting, route to `docs/00-system/contact-center-email-drafting-standard.md`; preserve the approved 9-column Case/Inquiry structure and source facts, do not add recipient-contact footer data, do not invent missing Case No. or actions, and use the approved Senses company banner as a real inline image when the source image is available.
- This index routes retrieval; it does not create new SOP facts.
- File status and document-specific guardrails remain authoritative.
- Do not infer emergency authority from personnel/location/contact reference files.
- Do not normalize source spellings or aliases unless explicitly approved.
- For One05, check `KB-CONFLICT-001`, read both original personnel references, and report their conflicting labels; do not infer a correct identity or full name. `source-conflict-register.md` tracks the disagreement and is not a factual replacement for either source.
- For Code M, route operational procedure questions to `docs/01-emergency-codes/code-m/overview.md`; preserve its explicit gaps, do not infer Code M trigger or declaration authority from UCEP or hospital-transfer confirmation, and check `KB-CONFLICT-002` for the unresolved FCC expansion disagreement.
- For Parade ambulance pickup, use the later approved location directory as the primary pickup-location reference and retain the older approved page as a cross-check; do not infer point priority or change either source's status.
- Do not generalize drill-specific procedures into Core SOP.
- Do not infer Building → Assembly Point mapping from visual proximity on a map unless an approved source explicitly maps them.
- Fire Truck Parking Points 1–5 must never be interpreted as Assembly Point numbers.
- For hospital transport questions, preserve the approved source grouping. Do not infer that free transport means free treatment, and do not recalculate distance to move hospitals between groups.
- For Traffic Knowledge, do not infer Entrance numbers, vehicle routes, traffic direction, opening hours, or access restrictions beyond the approved source. Treat construction status as time-sensitive source information.
- For SOC legal-awareness questions, route to `soc-basic-legal-awareness-reference.md`, preserve its **Approved Internal Training Reference** status, and do not present source-described legal claims as independently verified law. Its missing statutory authority, procedures, forms, approvers, retention period, or other explicitly open items remain gaps within that source; check a relevant routed source before declaring a Skills Hunter-wide Knowledge Gap. The 90-day Picture / Video Retention term is from `terminology.md`, not SOC Legal Awareness.
- For Code 3, preserve the routed overview's Draft status. For Code M, Code D and Threat Response, preserve Approved Reference status. Do not infer Threat Level declaration, escalation, reduction, or cancellation authority from Emergency Codes.
- Do not modify this index or any routed file without explicit KB Owner approval.

## Change Log

- v2.2 — 2026-09-20 — KB Owner-approved Contact Center email drafting route: added the Approved Contact Center email standard, 9-column Case/Inquiry table, recipient-contact exclusion rule, SOC follow-up contact line, approved Sittipong signature, and Senses company-banner inline-image requirement.
- v2.1 — 2026-09-20 — KB Owner-approved Guard Tour email drafting route: added the Approved Guard Tour email drafting standard, Skip-reason verification, building-email cancellation cross-checks, attachment/recipient/draft handling, query examples, and no-inference guardrail.
- v2.0 — 2026-09-17 — KB Owner-approved Code M gap closure routing: added the Approved Reference Code M procedure route, explicit Knowledge Gap handling, hospital/pickup cross-routing, and `KB-CONFLICT-002` FCC terminology cross-check.
- v1.9 — 2026-09-17 — Phase 4B KB Owner-approved conflict-management routing: added mandatory matching-register checks, the conflict-register route, and `KB-CONFLICT-001` cross-check for One05; clarified unresolved-conflict handling while preserving canonical precedence, status boundaries, and original-source provenance.
- v1.8 — 2026-09-17 — Phase 4A KB Owner-approved routing update: corrected Code 1/2 and Draft Code 3 routes/status wording; added Code D and Threat Response direct routes; separated source-specific and KB-wide CCTV retention provenance; added One05 conflict cross-check and Parade ambulance pickup source ordering/guardrails. No source knowledge document was changed.
- v1.7 — 2026-09-13 — Added direct routing for SOC basic legal awareness, caught-in-the-act/custody, Use of Force, search/seizure, detention/restraint, PDPA+CCTV, CCTV Request, and LINE/CCTV-data questions to `soc-basic-legal-awareness-reference.md`; added source-boundary and legal Knowledge-Gap guardrails plus query examples.
- v1.6 — 2026-09-10 — Added direct routing for Traffic Knowledge / project entrance-exit questions to `traffic-access-reference.md`, including car access, motorcycle access, MRT/public transport, and Helipad queries; added traffic-specific retrieval guardrails.
- v1.5 — 2026-09-10 — Added direct routing for hospital transport questions to `hospital-transport-reference.md`, including free-transport, 5 km/10 km, and 6–10 km transport-fee queries; cross-routed hospital phone-number questions to the Emergency Contact Directory and added transport-specific guardrails.
- v1.4 — 2026-09-10 — Added direct routing for Multi-Purpose Hall / อาคารอเนกประสงค์ capacity, One Bangkok project-area questions, and SOC orientation operational facts to `soc-orientation-operational-reference.md`; added query examples to prevent false Knowledge Gaps caused by routing these questions to the location directory.
- v1.3 — 2026-09-08 — Added Skills Hunter as the display / conversational identity of the existing Security Knowledge Base, added direct routing to the Skills Hunter identity document, and updated answer labels while preserving the repository and file paths.
- v1.2 — 2026-09-08 — Added direct routing for Assembly Point and Fire Truck Parking references and query examples.
- v1.1 — 2026-09-08 — Added mandatory answer source status labels: KB APPROVED, KNOWLEDGE GAP, and EXTERNAL.
- v1.0 — 2026-09-08 — Created as the central AI retrieval/router index to reduce false Knowledge Gaps caused by repository search misses.