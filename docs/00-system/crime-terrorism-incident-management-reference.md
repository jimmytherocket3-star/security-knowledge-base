# Crime & Terrorism Incident Management Reference

**Document ID:** SEC-SYSTEM-CRIME-TERROR-001  
**Title:** แผนบริหารจัดการเหตุการณ์อาชญากรรมและการก่อการร้าย  
**Source SOP:** OB-SOP-EP-0010 (source summaries include pages 11–19)  
**Version:** 1.2  
**Status:** Approved Reference  
**Owner:** KB Owner  
**Effective Date:** 2026-09-13  

---

## 1. Scope

Approved One Bangkok SOP reference for two incident scenarios:

1. การใช้ยานพาหนะเป็นอาวุธพุ่งชนบุคคล (**Car Plowed**)
2. การใช้อาวุธมีคมทำร้ายบุคคล (**Stabbing**)

This reference separates **Source-Supported Approved Knowledge** from **KB Owner-approved Proposed / Not Source-Confirmed operational structure**. Approval to retain a proposal does not mean OB-SOP-EP-0010 itself contains or mandates that proposal.

---

## 2. Car Plowed Workflow — Source-Supported

### 2.1 Notification & Verification
- ผู้พบเห็นหรือ Security Guard ประจำพื้นที่แจ้ง SOC.
- Security Guard ตรวจสอบเบื้องต้นและรายงานข้อมูล เช่น ทะเบียน สี ยี่ห้อ และทิศทางหลบหนี.
- SOC ตรวจ CCTV / Video Analytic เพื่อยืนยันและประเมินความรุนแรง.
- SOC เปิด Mozart: `Event Type: Security: Terrorist Attack (Car Plowed)` และแจ้ง DCC/หน่วยงานที่เกี่ยวข้องตามแผนสื่อสารฉุกเฉิน.

### 2.2 Response & Zone Control
- FCC เปิด PA แจ้งเตือนสถานการณ์ฉุกเฉิน.
- Technician เตรียมระบบภาพ/เสียงในห้อง DCC Alignment.
- IMT เข้าควบคุมและบัญชาการ ณ DCC Alignment.
- BMO จัดตั้งกองอำนวยการย่อย ณ One Power.
- FS ตรวจทะเบียนผ่าน LPR / Blacklist และแจ้งพื้นที่เสี่ยง Hot/Warm Zone ให้ SOC.
- TMT และ Security Guard ปิดกั้นพื้นที่ ควบคุมเส้นทางเข้า-ออก และจัดเส้นทางอพยพไป One Bangkok Park.
- หากสกัดยานพาหนะไม่ได้: TMT ขออนุมัติ DCC เพื่อเปิด **Hydraulic Bollard (HB) / Road Blocker (RB)** เพื่อสกัดไม่ให้เข้าสู่ Warm Zone / Safe Zone.

### 2.3 Police Handover & Control
- Security Guard คัดกรองหน่วยงานภายนอกที่ Main Entrance, Entrance 1, 2, 3, 5 และ Service Route โดยยืนยันทางวิทยุ POC กับ SOC.
- เมื่อตำรวจ/รถพยาบาลมาถึง TMT นำทางผ่าน **Gate 8** ไปยังกองอำนวยการย่อย One Power.
- ตำรวจรับมอบอำนาจควบคุมสถานการณ์ตามกฎหมาย; DCC/หน่วยงานภายในสนับสนุน.
- EOT ให้ข้อมูลและนำตำรวจเข้าจุดเกิดเหตุ.
- เมื่อตำรวจควบคุมสถานการณ์และยืนยันว่าเหตุยุติ ผู้บัญชาการเหตุการณ์จาก DCC ประกาศยุติเหตุการณ์.

### 2.4 Post-Incident & Closure
- EOT และพยาบาล/EMT ปฐมพยาบาลและลำเลียงผู้บาดเจ็บตาม `OB-SOP-SSHE-0007`.
- BMO ตรวจความเสียหายโครงสร้าง/ระบบพื้นฐานและบันทึกใน Mozart.
- SOC ตรวจหลักฐาน เช่น คลิป/บันทึกการสื่อสาร สื่อสารกลับสู่ภาวะปกติ และปิด Mozart case.
- TMT จัด Incident Report ตาม `OB-OW-WI-LW-0001`; DCC สรุปเหตุเสนอ IMT.
- IMT อนุมัติเปิดใช้พื้นที่และจัด Post-Incident Review.

---

## 3. Stabbing Workflow — Source-Supported

### 3.1 Notification & Verification
- ผู้พบเห็นแจ้ง SOC หรือ Security Guard.
- IBT หรือ Security Guard ตรวจสอบอย่างเร่งด่วน **โดยห้ามเข้าเผชิญหน้ากับผู้ก่อเหตุโดยตรง**.
- รายงานลักษณะผู้ก่อเหตุ พิกัดอาคาร/ชั้น/โซน ชนิดอาวุธ และจำนวนผู้บาดเจ็บให้ SOC.
- SOC ตรวจ CCTV / Video Analytic และเปิด Mozart: `Event Type: Security: Terrorist Attack (Stabbing)`.

### 3.2 Response & Zone Control
- SOC แจ้ง DCC และหน่วยงานที่เกี่ยวข้อง.
- DCC ควบคุม/สั่งการและกำหนด **Hot Zone / Warm Zone / Safe Zone** ตามความเสี่ยง.
- FCC เปิด PA; Technician เตรียม DCC Alignment; IMT เข้าห้องบัญชาการ.
- BMO ตั้งกองอำนวยการย่อย ณ อาคารเกิดเหตุ.
- IBT / Security Guard ปิดกั้นและควบคุมพื้นที่เพื่อจำกัดการเข้าถึง.
- Tenant/ร้านค้า: ปฏิบัติตาม PA, ล็อกประตูร้านชั่วคราว, ดูแลลูกค้า/พนักงานให้อยู่ในพื้นที่ปลอดภัย และไม่เผยแพร่ข้อมูลที่ยังไม่ยืนยัน.
- EOT/พยาบาล/EMT ปฐมพยาบาลและเคลื่อนย้ายผู้บาดเจ็บจาก Hot Zone ไป Safe Zone ตาม source summary.
- TMT ปิดกั้นพื้นที่และจัดเส้นทางอพยพไป One Bangkok Park หรือพื้นที่ปลอดภัยที่ DCC อนุมัติ.

### 3.3 Police Handover & Control
- Security Guard คัดกรองตำรวจ/รถพยาบาล ณ ทางเข้าและยืนยันผ่านวิทยุ POC กับ SOC.
- TMT นำทางจาก **Gate 8** ไปกองอำนวยการย่อย ณ อาคารเกิดเหตุ.
- ตำรวจรับมอบอำนาจควบคุมสถานการณ์ตามกฎหมาย.
- EOT นำทางตำรวจเข้าจุดเกิดเหตุ.
- เมื่อตำรวจระงับเหตุและยืนยันเหตุยุติ ผู้บัญชาการเหตุการณ์จาก DCC ประกาศยุติเหตุการณ์.

### 3.4 Post-Incident & Closure
ใช้กระบวนการตาม Car Plowed ใน source summary: รายงานผล, จัดส่งผู้ป่วย, BMO ประเมินความเสียหาย, SOC ตรวจหลักฐาน/ปิด Mozart, TMT/DCC ทำรายงานเสนอ IMT, IMT อนุมัติเปิดพื้นที่และ Post-Incident Review.

---

## 4. Source-Supported Authority / Roles

Source summary states:
- **SOC:** เปิดเคส/ยืนยันผ่าน CCTV/Video Analytic.
- **DCC:** ยกระดับ/สั่งการ/กำหนด Zone; source summary attributes approval of Bollard and evacuation to DCC in coordination context with IMT/ERT.
- **IMT:** command/strategic involvement at DCC Alignment; approves reopening; Post-Incident Review.
- **Police:** takes legal control of incident when on scene.
- **Incident commander from DCC:** announces incident termination after police confirmation.

Additional positions referenced by the SOP approval/responsibility sections:
1. **District Command Center Manager (DCC Manager)**
2. **Assistant Vice President, Facility Management Command Center Operations (AVP - FPMST)**
3. **Vice President - District Operations & Facility Management (VP - DOFM)**
4. **Deputy Director of Estate Management**

**Important:** The source does not establish from this information alone which of these positions is the specific DCC Incident Commander, nor does it provide a Succession Line / DoA Matrix.

---

## 5. Danger Zones — Source-Supported

- **Hot Zone:** พื้นที่เสี่ยงสูง/ยังมีภัยคุกคาม; access limited to operational personnel as described by source.
- **Warm Zone:** พื้นที่สนับสนุน/ปฐมพยาบาล/เตรียมพร้อม.
- **Safe Zone:** พื้นที่ปลอดภัย/จุดอพยพ; source gives One Bangkok Park as an example/route destination in these workflows.
- DCC determines zones according to risk.

No physical radius is specified in the source summary.

---

## 6. Communication & Police Handover — Source-Supported

- Communication mentioned: **POC radio** and **PA**.
- Incident information includes location and suspect/vehicle details and casualty count as applicable.
- External screening points listed: Main Entrance / Entrance 1, 2, 3, 5 / Service Route.
- TMT guide route begins at **Gate 8** to the applicable sub-command post.
- Police take legal incident control on arrival/entry as described by source.

---

## 7. Proposed Operational Structure — Approved to Retain, NOT Source-Confirmed

The following content came from the Draft Knowledge Base proposal supplied by the KB Owner. It is retained for future review but **must not be represented as an OB-SOP-EP-0010 requirement** unless separately confirmed by an approved source.

### 7.1 Proposed Incident Command Structure
- Proposed Tactical Incident Commander: **District Command Center Manager (DCC Manager)** for DCC operational command, PA command, and Bollard/Road Blocker approval.
- Proposed Strategic Commander: **VP - District Operations & Facility Management**, together with IMT, for escalation/strategic command.

### 7.2 Proposed DoA Matrix
| Priority | Tactical — DCC Commander | Strategic — IMT Leader |
|---|---|---|
| Primary | District Command Center Manager | VP - District Operations & Facility Management |
| 1st Alternate | AVP - Facility Management Command Center Operations | Deputy Director of Estate Management |
| 2nd Alternate | Security Supervisor (Duty Supervisor) | AVP - Facility Management Command Center Operations |

Proposed rule: if the preceding authority cannot be contacted within **3 minutes**, emergency decision authority would pass to the next level. **This 3-minute rule is a proposal, not a source-confirmed SOP requirement.**

### 7.3 Proposed SLA
- SOC Incident Verification: **≤ 2 minutes**.
- Mozart Case Opening & Escalation: **≤ 3 minutes**.
- Emergency Action — PA / Bollard: **≤ 5 minutes**.
- DCC Alignment Command Room Setup: **≤ 10–15 minutes**.

**Source status:** OB-SOP-EP-0010 uses wording equivalent to “ทันที” / “อย่างเร่งด่วน” in the supplied summary but does **not** state these numeric SLA values. Therefore all numeric SLA values above remain proposed only.

---

## 8. Remaining Knowledge Gaps

- Quantitative matrix distinguishing ordinary crime from `Terrorist Attack` classification.
- **Source-confirmed** DCC Incident Commander role title.
- **Source-confirmed** Delegation of Authority / Succession Line.
- **Source-confirmed numeric SLA**; source currently supports only urgent/immediate wording without numeric minutes.
- Mozart Form Template / required fields beyond stated Event Types.
- Physical radii for Hot/Warm/Safe Zones.
- Building-specific backup Warm/Safe Zone coordinates.
- Stabbing offender-control tactics are not provided; source leaves suppression/control to police and explicitly says IBT/Guard must not directly confront the offender.
- AED / First Aid equipment location map.
- Specific radio channel number.
- Direct police-station phone numbers in this SOP source.
- Standard Thai/English PA scripts.

---

## 9. AI Guardrails

- Always distinguish **Source-Supported Approved Knowledge** from **Proposed / Not Source-Confirmed** content.
- KB Owner approval of Section 7 authorizes retention of the proposal in Skills Hunter; it does **not** convert the proposal into an OB-SOP-EP-0010 requirement.
- Do not use proposed DCC Manager authority, DoA succession, 3-minute handoff rule, or numeric SLA as operational fact unless later supported by an approved source.
- **Stabbing:** never instruct IBT/Security Guard to directly confront, pursue, apprehend, or tactically engage the offender; source explicitly prohibits direct confrontation.
- Do not invent offender-control tactics; source assigns incident suppression/control to police.
- Do not automatically equate Car Plowed/Stabbing with **Code Sierra**, other Emergency Codes, or Threat Levels beyond the Mozart Event Types explicitly stated here.
- Do not import Code Sierra or Threat Response Protocol authority/workflow into this SOP without an Approved linkage.
- Do not invent Hot/Warm/Safe physical radii, radio channel, PA script, Mozart fields, or other missing values.
- One Bangkok Park is source-supported in these workflows; do not generalize it as the universal Assembly Point for every building/emergency.
- Preserve source distinction between Car Plowed sub-command at One Power and Stabbing sub-command at the affected building.
- Where source support remains absent, mark **Knowledge Gap**.

---

## 10. Sources

- `แผนการจัดการเหตุอาชญากรรม,ก่อการร้าย.md` — KB Owner approved 2026-09-13.
- `แผนการจัดการเหตุอาชญากรรม,ก่อการร้าย0.1.md` — KB Owner approved 2026-09-13; workflow summary derived from OB-SOP-EP-0010 pages 11–19.
- `แผนการจัดการเหตุอาชญากรรม,ก่อการร้าย0.2.md` — KB Owner approved 2026-09-13; contains source-supported management position references plus explicitly proposed Incident Command / DoA / SLA structure.

---

## 11. Change Log

- **v1.0 — 2026-09-13** — Initial Approved Reference from high-level source summary.
- **v1.1 — 2026-09-13** — Added approved Car Plowed and Stabbing workflows, authority/zone/communication details, police handover, closure workflow, and explicit remaining Knowledge Gaps.
- **v1.2 — 2026-09-13** — Added source-supported management position references and retained proposed Incident Command / DoA / SLA content under an explicit `Proposed / Not Source-Confirmed` classification.