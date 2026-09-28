---
document_id: KB-SYS-CONTACT-CENTER-EMAIL-001
title: Contact Center Email Writing Standard
version: 1.1
status: Active
owner: KB Owner
approved: 2026-09-28
---

# Contact Center Email Writing Standard

## 1. Purpose

Define the approved format for emails reporting after-hours Contact Centre calls handled by the Security Operation Centre (SOC).

This standard is separate from the Guard Tour Email Writing Standard. Do not merge or substitute the Guard Tour email format.

## 2. Primary Reference

The primary format reference is the KB Owner supplied file **รายงานการโอนสายเวลานอกเวลา.md** on 2026-09-28.

When drafting a new Contact Center email, preserve this reference's structure, terminology, order, and level of detail. Operational facts for each new email must come from the applicable case/source material. Do not copy historical case facts into a new report.

## 3. Approved Email Routing

**From:** Sittipong Homjai <sittipong.h@senses.co.th>  
**To:** contactcenter@onebangkok.com  
**CC:** _SENSES SOC Team <soc@senses.co.th>

## 4. Subject

Use exactly:

**รายงานการโอนสายเวลานอกเวลา จาก Contact Centre มายัง SOC**

## 5. Opening Structure

Use:

**เรียน ทีม Contact Center**

Then:

**ขอเรียนแจ้งสรุปรายการสายที่เข้ามายังศูนย์ความมั่นคงและความปลอดภัย (SOC) นอกเวลาทำการของ Contact Centre (22:30 – 08:00 น.) วันที่ [วันที่/ช่วงวันที่]**

Then define:

**Case:** รายการที่มีการบันทึกและเปิดเคสในระบบ Mozart เพื่อดำเนินการติดตาม  
**Inquiry:** การสอบถามทั่วไป ไม่มีการเปิดเคส

## 6. Required Case Table

Operational information must be presented in a table. Do not replace the table with a plain-text vertical field list.

Use these 9 columns in this exact order:

| No. | Date/Time | Caller Name | Contact No. | Type (case/Inquiry) | Topic | Case No. | Case Description | Action Required / Remark |
|---|---|---|---|---|---|---|---|---|

Each Case or Inquiry is one row.

Preserve source-supported narrative detail in **Case Description** and **Action Required / Remark**. Do not shorten away operationally relevant information merely to make the table smaller.

### Visual format

The approved visual reference uses:
- black table header background,
- white header text,
- visible borders,
- case/inquiry information arranged horizontally across the 9 columns.

When creating an HTML Gmail Draft, reproduce this structure and visual hierarchy as closely as the tool supports.

## 7. Content Fidelity Rules

Use only information supported by the applicable source/case material.

Do not invent or silently infer:
- Date/time
- Caller name
- Contact number
- Case/Inquiry classification
- Topic
- Case number
- Incident/location details
- Actions taken
- Follow-up status
- Resolution

Preserve established operational terminology such as SOC, FCC Retail, Mozart, Case, Inquiry, Location, and other terms when they appear in the source.

If information is missing, preserve the gap rather than manufacturing a value.

## 8. Contact Line After Table

After the table, use exactly:

**หากต้องการข้อมูลเพิ่มเติม สามารถติดต่อศูนย์ความมั่นคงและความปลอดภัย 02-483-5519 ได้ตลอด 24 ชั่วโมง**

## 9. Approved Closing and Signature Structure

Use:

**Best Regards,**

Sittipong Homjai | สิทธิพงษ์ หอมใจ  
SOC Operator - Security Operation Centre (SOC)  
Senses Property Management Company Limited

Mobile : 085-112-8002  
Mail :

Then place the approved Senses Property Management signature image according to the Full Email Signature Standard.

Do not insert placeholder text such as `[ข้อมูลการติดต่อ]` or `[โลโก้บริษัท]` into the actual email.

## 10. Inline Signature Image Limitation

If the connected Gmail drafting tool cannot insert the approved company signature image inline:
- do not claim it was inserted,
- do not substitute placeholder text,
- the KB Owner handles the inline signature image separately.

This limitation does not change the approved email format.

## 11. Draft Creation Rules

When the KB Owner requests a Contact Center Draft:

1. Read the applicable case/source information completely enough to populate the required fields.
2. Set To = `contactcenter@onebangkok.com`.
3. Set CC = `soc@senses.co.th`.
4. Use the approved subject exactly.
5. Use the approved opening and Case / Inquiry definitions.
6. Render all records in the approved 9-column table, preferably HTML.
7. Preserve source-supported Case Description and Action Required / Remark detail.
8. Add the SOC 24-hour contact line.
9. Add the approved closing and signature structure.
10. Do not send unless the KB Owner explicitly instructs sending.
11. Leave inline company signature-image handling to the KB Owner when the tool cannot insert it.

## 12. Quality Check Before Draft Creation

Confirm:
- To and CC are populated correctly
- Subject matches the approved subject
- Reporting date/period is correct
- Case/Inquiry definitions are present
- Table contains exactly the approved 9 columns in the approved order
- Each record is represented as one table row
- Case details match the source
- Action Required / Remark matches the source
- No unsupported facts have been added
- SOC 24-hour contact line is present
- Signature structure is correct
- Email remains distinct from the Guard Tour template

## 13. Source and Approval

Primary reference: **รายงานการโอนสายเวลานอกเวลา.md**, supplied and approved by the KB Owner on 2026-09-28.

The reference establishes:
- the subject,
- sender/recipient pattern,
- opening,
- after-hours window,
- Case and Inquiry definitions,
- 9-column case table,
- SOC contact line,
- closing and signature structure.

## 14. Revision History

| Version | Status | Change |
|---|---|---|
| 1.0 | Superseded | Initial Contact Center Email Writing Standard based on visual reference. |
| 1.1 | Active | Established รายงานการโอนสายเวลานอกเวลา.md as Primary Reference and tightened source fidelity, table structure, signature order, and pre-draft quality checks. |
