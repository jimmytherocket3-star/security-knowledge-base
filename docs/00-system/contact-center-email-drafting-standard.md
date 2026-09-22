---
document_id: SEC-KB-EMAIL-CONTACT-CENTER-001
title: Contact Center Email Drafting Standard
version: 1.1
status: Approved
owner: KB Owner
scope: SOC Email Drafting / Contact Center Handover
updated: 2026-09-22
---

# Contact Center Email Drafting Standard

## Purpose

กำหนดรูปแบบมาตรฐานสำหรับ AI ในการร่างอีเมลรายงานสายที่ Contact Centre โอนมายัง SOC นอกเวลาทำการ โดยต้องคงรูปแบบที่ผู้ใช้ตรวจสอบและอนุมัติแล้ว ทั้งโครงสร้างเนื้อหา ตาราง ลายเซ็น และแบนเนอร์บริษัท

## Approved Email Purpose

ใช้สำหรับอีเมลหัวข้อรายงานการโอนสายเวลานอกเวลา จาก Contact Centre มายัง SOC

รูปแบบหัวเรื่องมาตรฐาน:

`รายงานการโอนสายเวลานอกเวลา จาก Contact Centre มายัง SOC`

หากเป็นการทดสอบ ให้ใส่ `[TEST]` นำหน้าหัวเรื่องเมื่อผู้ใช้ร้องขอเท่านั้น

## Greeting

ใช้:

`เรียน ทีม Contact Center`

## Opening Paragraph

ใช้โครงสร้าง:

`ขอเรียนแจ้งสรุปรายการสายที่เข้ามายังศูนย์ความมั่นคงและความปลอดภัย (SOC) นอกเวลาทำการของ Contact Centre (22:30 – 08:00 น.) วันที่ DD/MM/YYYY`

วันที่ต้องอ้างอิงจากข้อมูลรายงานจริงของครั้งนั้น

## Case / Inquiry Definition

แสดงก่อนตาราง:

- **Case:** รายการที่มีการบันทึกและเปิดเคสในระบบ Mozart เพื่อดำเนินการติดตาม
- **Inquiry:** การสอบถามทั่วไป ไม่มีการเปิดเคส

## Required Table Format

ต้องใช้ตาราง 9 คอลัมน์ตามลำดับนี้:

| No. | Date/Time | Caller Name | Contact No. | Type (case/Inquiry) | Topic | Case No. | Case Description | Action Required / Remark |
|---|---|---|---|---|---|---|---|---|

### Column Rules

- **No.** — ลำดับรายการ
- **Date/Time** — วันที่และเวลาที่รับสาย
- **Caller Name** — ชื่อผู้ติดต่อ
- **Contact No.** — เบอร์โทรศัพท์ของผู้ติดต่อ
- **Type (case/Inquiry)** — ระบุ Case หรือ Inquiry ตามข้อมูลจริง
- **Topic** — สรุปประเด็นที่ติดต่อแบบกระชับ
- **Case No.** — เลขเคสใน Mozart หากมี; ถ้าแหล่งข้อมูลไม่ได้ให้เลขเคส ให้ใช้ `-` และห้ามสร้างเลขเคสเอง
- **Case Description** — รายละเอียดเหตุที่เพียงพอให้ติดตามต่อได้
- **Action Required / Remark** — การดำเนินการต่อ/หมายเหตุที่มีข้อมูลรองรับ

## Information Preservation Rules

1. ใช้เฉพาะข้อมูลที่ผู้ใช้หรือแหล่งข้อมูลให้มา
2. ห้ามเดาเลข Case No.
3. ห้ามสร้างชื่อ บุคคล เบอร์โทร เวลา สถานที่ สาเหตุ หรือผลการดำเนินการที่ไม่มีในข้อมูลต้นทาง
4. หากข้อมูลบางช่องไม่มี ให้ใช้ `-` หรือระบุว่าไม่พบข้อมูลตามความเหมาะสม
5. รักษาคำศัพท์ `Case`, `Inquiry`, `Mozart`, `SOC`, `Contact Centre` ตามรูปแบบมาตรฐาน
6. หากผู้ใช้ให้หลายรายการ ให้เพิ่มเป็นหลายแถวในตารางเดียว เว้นแต่ผู้ใช้สั่งให้แยกอีเมล

## Recipient-Contact Rule

ห้ามใส่ "ข้อมูลติดต่อกลับของผู้รับเรื่อง" หรือข้อมูลส่วนตัวของเจ้าหน้าที่ผู้รับสายเป็นส่วนท้ายของรายงาน เว้นแต่ผู้ใช้สั่งโดยตรง

ข้อมูลผู้ติดต่อในแต่ละ Case/Inquiry ให้แสดงเฉพาะในแถวข้อมูลที่เกี่ยวข้องตามตาราง

## Follow-up Contact Line

ก่อนลายเซ็น ใช้ข้อความ:

`หากต้องการข้อมูลเพิ่มเติม สามารถติดต่อศูนย์ความมั่นคงและความปลอดภัย 02-483-5519 ได้ตลอด 24 ชั่วโมง`

ห้ามเปลี่ยนเบอร์หรือข้อความนี้โดยไม่มีข้อมูลใหม่หรือคำสั่งจากผู้ใช้

## Approved Signature

ใช้ลายเซ็นนี้:

**Best Regards,**

Sittipong Homjai | สิทธิพงษ์ หอมใจ  
SOC Operator - Security Operation Centre (SOC)  
Senses Property Management Company Limited

Mobile : 085-112-8002  
Mail : sittipong.h@senses.co.th

## Company Signature Banner

หลังบรรทัด Mobile / Mail ต้องแสดง **แบนเนอร์โลโก้ Senses Property Management Company Limited** ตามต้นแบบที่ผู้ใช้อนุมัติ

องค์ประกอบที่มองเห็นในแบนเนอร์ต้นแบบ:
- โลโก้ `SENSES PROPERTY MANAGEMENT`
- ข้อความ `Senses Property Management Company Limited`
- ที่อยู่บริษัท
- หมายเลข `+66 2643 7595`
- เว็บไซต์ `www.senses.co.th`

### Banner Rendering Rule

- ใน Draft Gmail ให้ใช้รูปภาพจริงแบบ **inline image** ใต้ข้อมูล Mobile / Mail
- ห้ามใช้ข้อความ placeholder เช่น `[SENSES PROPERTY MANAGEMENT — Company Signature Banner]` แทนรูปภาพเมื่อมีไฟล์ภาพต้นฉบับพร้อมใช้งาน
- ใช้ไฟล์แบนเนอร์ที่ผู้ใช้อนุมัติเป็นต้นแบบ
- หากในบริบทปัจจุบันไม่มีไฟล์ภาพต้นฉบับที่เข้าถึงได้ ให้แจ้งผู้ใช้ก่อนว่าต้องการไฟล์ภาพเพื่อฝังเป็น inline image; ห้ามอ้างว่าใส่โลโก้จริงแล้ว
- ห้ามเปลี่ยนดีไซน์ สี ข้อความ หรือครอปโลโก้เองโดยไม่ได้รับอนุมัติ

## Gmail Draft Handling

1. สร้าง/แก้ Draft เท่านั้นเมื่อผู้ใช้ขอให้ร่างหรือทดสอบ
2. ห้ามส่งอีเมลจริงจนกว่าผู้ใช้จะสั่งส่งอย่างชัดเจน
3. หากผู้ใช้ขอ "เขียนเมล์ใหม่เพื่อทดสอบ" ให้สร้าง Draft ใหม่
4. หากผู้ใช้ขอ "แก้ Draft" ให้แก้ Draft ที่เกี่ยวข้อง ไม่สร้างฉบับใหม่โดยไม่จำเป็น
5. หลังแก้ Draft ให้ผู้ใช้ตรวจสอบก่อนนำรูปแบบใหม่ไปปรับ KB เว้นแต่ผู้ใช้อนุมัติ KB ไว้แล้ว

## Approved Layout Order

ลำดับส่วนของอีเมลต้องเป็น:

1. Subject
2. Recipient / CC ตามคำสั่ง
3. Greeting
4. Opening paragraph
5. Case / Inquiry definitions
6. Case/Inquiry table
7. Follow-up contact line
8. Best Regards signature
9. Mobile / Mail
10. Company signature banner as inline image

## AI Decision Rule

**Use the approved layout, preserve source facts, keep every Case/Inquiry traceable, and never invent missing case details. The company banner must be an actual inline image when the approved source image is available.**

## Final Verification Checklist

ก่อนถือว่า Draft พร้อมให้ผู้ใช้ตรวจ ให้ตรวจอย่างน้อย:

- [ ] Subject ถูกต้อง
- [ ] วันที่ตรงกับข้อมูลรายงาน
- [ ] Greeting ถูกต้อง
- [ ] Case / Inquiry definition ครบ
- [ ] ตารางมี 9 คอลัมน์และเรียงถูกต้อง
- [ ] Date/Time ถูกต้อง
- [ ] Caller Name ถูกต้อง
- [ ] Contact No. ถูกต้อง
- [ ] Type ถูกต้อง
- [ ] Topic ไม่แต่งข้อมูลเพิ่ม
- [ ] Case No. ไม่ถูกเดา
- [ ] Case Description ยึดข้อมูลต้นทาง
- [ ] Action Required / Remark ยึดข้อมูลต้นทาง
- [ ] ไม่มีข้อมูลติดต่อกลับของผู้รับเรื่องโดยไม่จำเป็น
- [ ] Follow-up contact line ใช้ 02-483-5519
- [ ] ลายเซ็น Sittipong Homjai / สิทธิพงษ์ หอมใจ ถูกต้อง
- [ ] Mobile และ Mail ถูกต้อง
- [ ] แบนเนอร์ Senses แสดงเป็น inline image จริงเมื่อมีไฟล์ต้นฉบับ
- [ ] ไม่ส่งอีเมลจริงหากผู้ใช้ยังไม่ได้สั่งส่ง

## Approval Record

รูปแบบนี้ได้รับการตรวจสอบจากผู้ใช้ผ่าน Draft Gmail และได้รับอนุมัติให้นำไปบันทึกใน Skills Hunter เมื่อวันที่ 2026-09-20.


## Global Email Signature and Banner Standard

สำหรับอีเมล Contact Center ทุกฉบับ ให้ใช้ลายเซ็นและ Company Banner ตาม `docs/00-system/email-signature-banner-standard.md`

- Approved source image: `SENSES Rev (3).jpg`
- วางแบนเนอร์ทันทีหลัง Mobile / Mail
- ใช้รูปภาพจริงแบบ inline image
- ห้ามใช้ placeholder หากไฟล์ต้นฉบับพร้อมใช้งาน
- ห้ามอ้างว่าได้ใส่โลโก้แล้วหากยังไม่ได้แทรกภาพจริง
