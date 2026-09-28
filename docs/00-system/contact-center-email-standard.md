---
document_id: KB-SYS-CONTACT-CENTER-EMAIL-001
title: Contact Center Email Writing Standard
version: 1.0
status: Active
owner: KB Owner
approved: 2026-09-28
---

# Contact Center Email Writing Standard

## 1. Purpose

Define the approved format for emails reporting after-hours Contact Centre calls handled by the Security Operation Centre (SOC).

This standard is **separate from the Guard Tour Email Writing Standard**. Do not merge or substitute the Guard Tour email format.

Guard Tour standard:
`docs/00-system/guard-tour-email-standard.md`

## 2. Approved Email Routing

**From:** Sittipong Homjai <sittipong.h@senses.co.th>  
**To:** contactcenter@onebangkok.com  
**CC:** _SENSES SOC Team <soc@senses.co.th>

## 3. Subject

Use:

**รายงานการโอนสายเวลานอกเวลา จาก Contact Centre มายัง SOC**

## 4. Opening Structure

Use:

**เรียน ทีม Contact Center**

Then report the after-hours calls received by SOC using the established wording:

**ขอเรียนแจ้งสรุปรายการสายที่เข้ามายังศูนย์ความมั่นคงและความปลอดภัย (SOC) นอกเวลาทำการของ Contact Centre (22:30 – 08:00 น.) วันที่ [วันที่/ช่วงวันที่]**

Then define:

**Case:** รายการที่มีการบันทึกและเปิดเคสในระบบ Mozart เพื่อดำเนินการติดตาม  
**Inquiry:** การสอบถามทั่วไป ไม่มีการเปิดเคส

## 5. Required Case Table

Operational information must be presented as a table. Do **not** replace the approved table with a plain-text vertical field list.

The table contains these 9 columns in this order:

| No. | Date/Time | Caller Name | Contact No. | Type (case/Inquiry) | Topic | Case No. | Case Description | Action Required / Remark |
|---|---|---|---|---|---|---|---|---|

### Table visual format

The approved reference uses:
- Black header background
- White header text
- Visible cell borders
- One case/inquiry per row
- Case Description and Action Required / Remark as narrative cells

When creating an HTML Gmail Draft, preserve this table structure and visual hierarchy as closely as the drafting tool supports.

## 6. Content Rules

Use only information supported by the case/source material.

Do not invent:
- Caller details
- Contact number
- Case number
- Incident location
- Actions taken
- Follow-up status
- Resolution
- Times

Keep operational terms such as SOC, FCC Retail, Mozart, Case, Inquiry, Location, and other established terms where supported by the source.

If required information is unavailable, do not silently create it.

## 7. Contact Line After Table

After the table, use:

**หากต้องการข้อมูลเพิ่มเติม สามารถติดต่อศูนย์ความมั่นคงและความปลอดภัย 02-483-5519 ได้ตลอด 24 ชั่วโมง**

## 8. Approved Signature Structure

After the contact line, use the approved full signature:

**Best Regards,**

Sittipong Homjai | สิทธิพงษ์ หอมใจ  
SOC Operator - Security Operation Centre (SOC)  
Senses Property Management Company Limited

Mobile : 085-112-8002  
Mail :

[Approved Senses Property Management signature image]

sittipong.h@senses.co.th

The approved company signature image is positioned after the personal/company contact information and before the final email link/address, matching the KB Owner's reference email.

Do not insert placeholders such as `[ข้อมูลการติดต่อ]` or `[โลโก้บริษัท]` into the actual email.

## 9. Gmail Drafting Limitation

If the connected Gmail drafting tool cannot reproduce the approved inline company signature image, do not claim that the image has been inserted.

The KB Owner currently handles the inline signature image separately.

This tool limitation does not change the approved Contact Center email layout.

## 10. Draft Creation Rules

When the KB Owner requests a Contact Center email Draft:

1. Set To = `contactcenter@onebangkok.com`.
2. Set CC = `soc@senses.co.th`.
3. Use the approved subject.
4. Use the approved opening and Case / Inquiry definitions.
5. Render case data in the approved 9-column table, preferably HTML.
6. Preserve the Case Description and Action Required / Remark information from the source.
7. Add the SOC 24-hour contact line.
8. Add the approved full signature structure.
9. Do not send unless the KB Owner explicitly instructs sending.
10. Leave the inline Senses signature image for the KB Owner when the drafting tool cannot insert it.

## 11. Approved Reference

Primary visual reference: Contact Center email example supplied by the KB Owner on 2026-09-28.

The reference shows:
- Subject: `รายงานการโอนสายเวลานอกเวลา จาก Contact Centre มายัง SOC`
- To: Contact Center
- CC: SENSES SOC
- Introductory after-hours reporting text
- Case and Inquiry definitions
- Black-header 9-column case table
- SOC contact line
- Full personal/company signature
- Inline Senses Property Management signature artwork
- Final email address

This Contact Center standard must remain distinct from the Guard Tour Email Writing Standard.

## 12. Revision History

| Version | Status | Change |
|---|---|---|
| 1.0 | Active | Initial approved Contact Center Email Writing Standard based on KB Owner visual reference. |
