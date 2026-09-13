# Crime & Terrorism Incident Management Reference

**Document ID:** SEC-SYSTEM-CRIME-TERROR-001  
**Title:** แผนบริหารจัดการเหตุการณ์อาชญากรรมและการก่อการร้าย  
**Source SOP:** OB-SOP-EP-0010 (source summaries include pages 11–19)  
**Version:** 1.4  
**Status:** Approved Reference  
**Owner:** KB Owner  
**Effective Date:** 2026-09-13  

---

## 1. Scope
Approved One Bangkok reference for **Car Plowed** and **Stabbing** incidents. This document strictly separates **Source-Supported Approved Knowledge** from **KB Owner-approved Proposed / Not Source-Confirmed** structures.

---

## 2. Source-Supported Workflow
### Car Plowed
- ผู้พบเห็น/Security Guard แจ้ง SOC; Guard ตรวจสอบและรายงานทะเบียน สี ยี่ห้อ ทิศทาง.
- SOC ตรวจ CCTV/Video Analytic และเปิด Mozart `Security: Terrorist Attack (Car Plowed)`; แจ้ง DCC/หน่วยงานที่เกี่ยวข้อง.
- FCC เปิด PA; Technician เตรียม DCC Alignment; IMT เข้าบัญชาการ; BMO ตั้ง กอ.ย่อย One Power.
- FS ตรวจ LPR/Blacklist; TMT/Security ปิดกั้นและจัดเส้นทางอพยพไป One Bangkok Park.
- หากสกัดไม่ได้ TMT ขอ DCC อนุมัติ Hydraulic Bollard/Road Blocker.
- TMT นำตำรวจ/รถพยาบาลผ่าน Gate 8 ไป กอ.ย่อย One Power; ตำรวจรับควบคุมเหตุ; EOT สนับสนุน/นำทาง.
- หลังตำรวจยืนยันเหตุยุติ ผู้บัญชาการเหตุการณ์จาก DCC ประกาศยุติ.
- EOT/พยาบาล/EMT ดูแลผู้บาดเจ็บตาม OB-SOP-SSHE-0007; BMO ประเมินความเสียหาย; SOC ตรวจหลักฐาน/ปิดเคส; TMT/DCC รายงาน; IMT อนุมัติเปิดพื้นที่และ Post-Incident Review.

### Stabbing
- ผู้พบเห็นแจ้ง SOC/Security Guard; IBT/Guard ตรวจสอบเร่งด่วน **โดยห้ามเผชิญหน้าผู้ก่อเหตุโดยตรง**.
- แจ้งลักษณะผู้ก่อเหตุ พิกัด ชนิดอาวุธ จำนวนผู้บาดเจ็บ; SOC ตรวจ CCTV/Video Analytic และเปิด Mozart `Security: Terrorist Attack (Stabbing)`.
- DCC ควบคุมและกำหนด Hot/Warm/Safe Zone; FCC PA; Technician เตรียม DCC Alignment; IMT เข้าบัญชาการ; BMO ตั้ง กอ.ย่อย ณ อาคารเกิดเหตุ.
- IBT/Security ปิดกั้นพื้นที่; Tenant/ร้านค้าปฏิบัติตาม PA ล็อกประตูชั่วคราวและดูแลผู้ที่อยู่ภายใน.
- EOT/พยาบาล/EMT เคลื่อนย้ายผู้บาดเจ็บตาม source summary; TMT จัดเส้นทางไป One Bangkok Park/พื้นที่ปลอดภัยที่ DCC อนุมัติ.
- TMT นำตำรวจจาก Gate 8 ไป กอ.ย่อย; ตำรวจรับควบคุมเหตุ; EOT นำทาง.
- หลังตำรวจยืนยันเหตุยุติ ผู้บัญชาการเหตุการณ์จาก DCC ประกาศยุติ; recovery/closure ตามกระบวนการข้างต้น.

---

## 3. Source-Supported Authority / Roles
- SOC: ยืนยันผ่าน CCTV/Video Analytic และเปิดเคส.
- DCC: สั่งการ/กำหนด Zone; source summary attributes Bollard/evacuation approval in DCC coordination context.
- IMT: command/strategic involvement, reopening approval, Post-Incident Review.
- Police: legal incident control on scene.
- Incident commander from DCC: termination announcement after police confirmation.

Positions referenced in SOP approval/responsibility sections:
1. District Command Center Manager (DCC Manager)
2. Assistant Vice President, Facility Management Command Center Operations (AVP - FPMST)
3. Vice President - District Operations & Facility Management (VP - DOFM)
4. Deputy Director of Estate Management

The source does not establish which position is the specific DCC Incident Commander or a succession line.

---

## 4. Source-Supported Danger Zones / Communication
- Hot Zone: high-risk/active-threat area as described by source.
- Warm Zone: support/first-aid/readiness area.
- Safe Zone: safe/evacuation area; One Bangkok Park appears as a workflow destination/example.
- DCC determines zones according to risk; no physical radius stated.
- Communication mentioned: POC radio and PA.
- External screening: Main Entrance / Entrance 1, 2, 3, 5 / Service Route.
- TMT guides from Gate 8 to the applicable sub-command post.

---

## 5. Mozart — Source-Supported Recording Information
OB-SOP-EP-0010 identifies Mozart as a central service/security/building incident-management system and supports recording/receiving information including incident date/time, reporter, Security Event Category, Car Plowed/Stabbing Event Types, location, suspect/vehicle details, casualty/severity, Danger Zone, PA/action information, barrier/bollard actions, external-agency handover, BMO assessment, evidence, incident report reference, resolution, and IMT reopening approval.

**Important:** OB-SOP-EP-0010 does not provide the complete Mozart screen/form schema. These are source-supported information requirements/references, not confirmation of exact proposed field labels, UI control types, phases, or screen layout.

---

## 6. Mozart Platform Overview — Approved Source-Supported Reference
Source: **คู่มือการใช้งาน MOZART** supplied and approved by the KB Owner on 2026-09-13.

The available source summary supports the following platform-level facts:
- MOZART is a platform used by Security Operations Center personnel.
- **Case Management** covers the incident lifecycle from receiving/reporting an incident through case/work closure.
- MOZART acts as a **central information hub** connecting control-center personnel and field operational teams so they can work from a shared situational picture.
- The guide also covers **video functions**, **personnel/resource management**, and **loading/receiving-parking-area management**.
- The guide organizes/prioritizes incident content according to **frequency and impact level**, with examples including fire alarms and medical emergencies, to support correct and rapid response to critical situations.

### Evidence Boundary
The currently approved source material is a one-line high-level summary of the MOZART manual. It does **not** expose or verify:
- Actual Mozart screen names/layout.
- Complete form schema.
- Exact field labels.
- UI control/data types.
- Mandatory vs optional fields.
- Dropdown values/status lists.
- Permissions/workflow configuration.

Therefore this source strengthens the **Mozart Platform Overview** but does **not close the Actual Mozart Form Schema/UI Knowledge Gap**.

---

## 7. Proposed / Not Source-Confirmed — Incident Command, DoA, SLA
Approved to retain for future review only:
- Proposed Tactical IC: DCC Manager.
- Proposed Strategic Commander: VP - DOFM with IMT.
- Proposed Tactical DoA: DCC Manager → AVP FPMST → Security Supervisor (Duty Supervisor).
- Proposed Strategic DoA: VP DOFM → Deputy Director Estate Management → AVP FPMST.
- Proposed automatic handoff if prior authority unreachable within 3 minutes.
- Proposed SLA: SOC verification ≤2 min; Mozart opening/escalation ≤3 min; PA/Bollard ≤5 min; DCC Alignment setup ≤10–15 min.

None of these proposed role assignments, succession rules, or numeric SLA values are source-confirmed OB-SOP-EP-0010 requirements.

---

## 8. Proposed Mozart Form Structure — Approved to Retain, NOT System-Confirmed
Approved four-phase operational-design proposal:
1. Case Creation & Initial Verification.
2. Emergency Response & Action Log.
3. Facility Inspection & Damage Assessment.
4. Case Closure & Evidence Attachment.

Proposed fields include Case ID, Incident Date & Time, Reporter Info, Event Category/Type, Location, Threat/Suspect Details, Casualty & Severity, IC, Danger Zone, PA Log, Barrier/Bollard, External Agency Handover, Police Unit, BMO Inspection, Area Safety Clearance, Evidence, Incident Report Reference, Resolution Summary, IMT Re-opening Approval and Case Status.

The phase organization, exact field names, UI control types and `Case Status = Closed` remain **Proposed / Not System-Confirmed** until verified by actual Mozart screen/manual/configuration evidence.

---

## 9. Remaining Knowledge Gaps
- Quantitative matrix distinguishing ordinary crime from `Terrorist Attack` classification.
- Source-confirmed DCC Incident Commander role title.
- Source-confirmed DoA / Succession Line.
- Source-confirmed numeric SLA.
- **Actual Mozart Form Schema/UI**: exact field names, types, mandatory/optional status, phase/screen layout and valid status values remain unconfirmed.
- Physical radii for Hot/Warm/Safe Zones.
- Building-specific backup Warm/Safe Zone coordinates.
- Stabbing offender-control tactics; source says IBT/Guard must not directly confront offender and leaves control to police.
- AED / First Aid equipment location map.
- Specific radio channel number.
- Direct police-station phone numbers in this SOP source.
- Standard Thai/English PA scripts.

---

## 10. AI Guardrails
- Always distinguish Source-Supported facts from Proposed / Not Source-Confirmed material.
- KB Owner approval to retain a proposal does not convert it into an OB-SOP-EP-0010 or Mozart system requirement.
- The Mozart manual summary confirms platform-level capabilities only; do not use it to claim exact UI/schema details.
- Do not represent proposed Mozart phases, field labels/types or `Closed` option as actual system configuration without system evidence.
- Do not use proposed IC/DoA/SLA as operational fact without source confirmation.
- For Stabbing, never instruct IBT/Security Guard to directly confront, pursue, apprehend or tactically engage the offender.
- Do not invent offender-control tactics, zone radii, radio channels, PA scripts or missing Mozart fields.
- Do not automatically equate Car Plowed/Stabbing with Code Sierra or Threat Levels beyond stated Event Types.
- Do not generalize One Bangkok Park as the universal Assembly Point.
- Missing source support = Knowledge Gap.

---

## 11. Sources
- `แผนการจัดการเหตุอาชญากรรม,ก่อการร้าย.md` — approved 2026-09-13.
- `แผนการจัดการเหตุอาชญากรรม,ก่อการร้าย0.1.md` — approved 2026-09-13.
- `แผนการจัดการเหตุอาชญากรรม,ก่อการร้าย0.2.md` — approved 2026-09-13.
- `แผนการจัดการเหตุอาชญากรรม,ก่อการร้าย0.3.md` — approved 2026-09-13.
- `คู่มือการใช้งานMozart.md` — approved 2026-09-13; high-level Mozart platform/manual summary.

---

## 12. Change Log
- v1.0 — Initial Approved Reference.
- v1.1 — Added Car Plowed/Stabbing workflows and explicit gaps.
- v1.2 — Added source-supported management positions and Proposed IC/DoA/SLA structure.
- v1.3 — Added source-supported Mozart recording information and Proposed four-phase form design.
- **v1.4 — 2026-09-13** — Added approved source-supported Mozart Platform Overview from `คู่มือการใช้งานMozart.md`; retained Actual Mozart Form Schema/UI as Knowledge Gap.