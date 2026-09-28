---
document_id: KB-SYS-GUARD-TOUR-EMAIL-001
title: Guard Tour Email Writing Standard
version: 1.1
status: Active
owner: KB Owner
approved: 2026-09-28
---

# Guard Tour Email Writing Standard

## 1. Purpose

Define the approved content structure and drafting rules for Guard Tour summary emails prepared for the KB Owner.

This standard is separate from the Contact Center Email Writing Standard. Do not mix the two templates.

## 2. Primary Reference

The primary content-format reference is the KB Owner supplied file **เมลล์การ์ดทัวร์.md** on 2026-09-28.

When drafting, preserve the reference structure and level of detail. Operational facts for a new email must come from the applicable Daily Guard Tour Report(s) and other confirmed source information. Do not copy old operational facts into a new date.

## 3. Email Routing

**From:** Sittipong Homjai <sittipong.h@senses.co.th>  
**To:** _SENSES SOC Team <soc@senses.co.th>  
**CC:** Not established. Do not infer or add CC recipients without confirmed information.

Populate `soc@senses.co.th` in the To field when the Draft is created.

## 4. Subject Format

Use:

**สรุปผลการปฏิบัติงาน Guard Tour อาคาร [ชื่ออาคาร] ประจำวันที่ [วันที่/ช่วงวันที่]**

Use the building/location name and date supported by the source report(s).

## 5. Opening

Use:

**เรียน ผู้เกี่ยวข้องทุกท่าน,**

Then:

**ขอนำส่งสรุปผลการปฏิบัติงาน Guard Tour อาคาร [ชื่ออาคาร] ประจำวันที่ [วันที่/ช่วงวันที่] โดยมีรายละเอียดดังนี้**

## 6. Building-Level Summary — Required

Before the round-by-round detail, provide:

**สรุปผล Guard Tour : [อาคาร/Location]**

Include, when supported:
- อาคาร (Location)
- แผนทั้งหมด (Planned): [x] Routes
- ดำเนินการสำเร็จ (Completed): [x] Routes
- ไม่สำเร็จ (Not Completed): [x] Routes
- ยกเลิก (Cancel): [x] Routes
- พบการ Skip จุดตรวจรวมทั้งหมด [x] จุด

Do not derive or invent counts that are not supported by the source material.

## 7. Round-by-Round Detail — Required

Use heading:

**รายละเอียดผลการตรวจแต่ละรอบ**

For every applicable round, show:

**รอบเวลา [HH.MM – HH.MM น.]**
- Status: [status]
- Skip: [x] จุด
- สาเหตุ: [confirmed reason]

Then show:

**จุดที่ Skip:**

List every confirmed Skip point for that round in the form:

**[ชื่อจุดตรวจ] — QR Code: [รหัส]**

If the source does not provide a QR code, use **QR Code: -** rather than inventing a code.

If the source does not establish the reason for a Skip, explicitly state that the reason is not established. Do not infer a reason from another point or another round.

Where the source contains an important inconsistency or unsupported Skip condition, include a concise **หมายเหตุ:** explaining exactly what is and is not confirmed.

## 8. Source Fidelity for Skip Reasons

A Skip reason may be written only when supported by:
- the applicable Daily Guard Tour Report / Remark,
- confirmed email information, or
- information explicitly confirmed by the KB Owner.

Examples of wording in the approved reference include Set up / event activity and rooftop flooding, but these are historical examples only. They must not be automatically reused for a different date or round.

If a report says Skip but provides no confirmed reason, preserve that as an information gap.

## 9. Skip Summary — Required

After all rounds, include:

**สรุปจำนวน Skip ทุกรอบ**

List each round and its Skip count, then state:

**รวมทั้งหมด [x] จุด Skip**

The total must reconcile with the round counts. If it does not, flag the discrepancy rather than silently changing the source.

## 10. Attachments

State:

**ทั้งนี้ ได้แนบ Daily Guard Tour Report จำนวน [x] ไฟล์ มาพร้อมอีเมลฉบับนี้ เพื่อประกอบการตรวจสอบและอ้างอิง**

Attach the applicable report file(s). The attachment count in the email must match the files actually attached.

## 11. Closing

Use:

**หากต้องการข้อมูลเพิ่มเติม สามารถแจ้งกลับมายัง SOC ได้ครับ**

Then:

**Best Regards,**

Sittipong Homjai l สิทธิพงษ์ หอมใจ  
SOC Operator - Security Operation Centre (SOC)  
Senses Property Management Company Limited

Mobile : 085-112-8002  
Mail : sittipong.h@senses.co.th

Then apply the approved Senses signature image according to:
`docs/00-system/email-signature-standard.md`

## 12. Inline Signature Image Limitation

If the connected Gmail drafting tool cannot insert the approved company signature image inline:
- do not use a placeholder such as `[โลโก้บริษัท]`,
- do not claim the image was inserted,
- the KB Owner handles the inline signature image separately.

## 13. Draft Creation Rules

When the KB Owner requests a Guard Tour email Draft:

1. Read the applicable Guard Tour Report(s) completely enough to establish the summary, every round, Skip counts, Skip points, QR codes, reasons, remarks, and attachment count.
2. Set To = `soc@senses.co.th` at Draft creation.
3. Do not infer CC.
4. Use the approved building-level summary first.
5. Follow with every round in chronological/report order.
6. For each round, include Status, Skip count, confirmed reason, and all Skip point names with QR codes.
7. Preserve gaps and inconsistencies; do not invent missing causes or codes.
8. Add the all-round Skip summary and reconcile the total.
9. State the correct number of attached Daily Guard Tour Reports.
10. Attach the applicable report(s).
11. Use the approved closing and full signature structure.
12. Do not send unless the KB Owner explicitly instructs sending.
13. Leave inline company signature-image handling to the KB Owner when the tool cannot insert it.

## 14. Quality Check Before Draft Creation

Confirm:
- Correct building/location and reporting date
- Correct Planned / Completed / Not Completed / Cancel counts
- Correct total Skip count
- Every applicable round included
- Skip count per round matches source
- Every listed Skip point is source-supported
- QR codes match source; missing QR shown as `-`
- Skip reasons are source-supported
- Notes identify unresolved discrepancies where needed
- Skip total reconciles
- Attachment count matches actual attachments
- To recipient is populated
- CC is not inferred
- Signature structure is correct

## 15. Revision History

| Version | Status | Change |
|---|---|---|
| 1.0 | Superseded | Initial Guard Tour Email Writing Standard. |
| 1.1 | Active | Rebuilt content structure from KB Owner approved เมลล์การ์ดทัวร์.md reference; added building summary, per-round Skip details and QR points, reason fidelity, all-round Skip reconciliation, attachment-count rule, and pre-draft quality check. |
