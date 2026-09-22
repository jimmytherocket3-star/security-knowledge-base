---
document_id: SEC-KB-EMAIL-SIGNATURE-001
title: Global Email Signature and Company Banner Standard
version: 1.0
status: Approved
owner: KB Owner
scope: All User Email Drafting / Signature / Company Banner
approved: 2026-09-22
updated: 2026-09-22
---

# Global Email Signature and Company Banner Standard

## 1. Purpose

กำหนดมาตรฐานส่วนท้ายอีเมลสำหรับอีเมลทุกประเภทที่ AI ร่าง สร้าง Draft หรือเตรียมส่งในนามผู้ใช้

มาตรฐานนี้เป็นกติกากลาง และใช้ร่วมกับมาตรฐานอีเมลเฉพาะประเภท เช่น Guard Tour และ Contact Center

## 2. Mandatory Application

สำหรับ **อีเมลทุกฉบับของผู้ใช้** ให้แสดงลายเซ็นและแบนเนอร์บริษัทตามลำดับที่กำหนดในเอกสารนี้ เว้นแต่ผู้ใช้สั่งให้ใช้อีเมล/ลายเซ็นรูปแบบอื่นสำหรับงานนั้นโดยชัดเจน

กติกานี้ใช้กับ:
- Gmail Draft
- อีเมลที่เตรียมส่ง
- อีเมล Guard Tour
- อีเมล Contact Center
- อีเมลรายงาน SOC
- อีเมลอื่นใดที่ AI ร่างในนามผู้ใช้

## 3. Approved User Signature

ใช้ข้อมูลดังนี้:

**Best Regards,**

Sittipong Homjai | สิทธิพงษ์ หอมใจ  
SOC Operator - Security Operation Centre (SOC)  
Senses Property Management Company Limited

Mobile : 085-112-8002  
Mail : sittipong.h@senses.co.th

## 4. Approved Company Banner

หลังบรรทัด Mobile / Mail ต้องแสดง **แบนเนอร์โลโก้ Senses Property Management Company Limited** เป็นรูปภาพจริงแบบ inline image

Approved source image supplied by KB Owner:
- File name: `SENSES Rev (3).jpg`
- Approved date: 2026-09-22
- Purpose: Company email signature banner
- Placement: Immediately after the user's Mobile / Mail lines

องค์ประกอบที่มองเห็นในภาพต้นฉบับ:
- โลโก้ `SENSES PROPERTY MANAGEMENT`
- ข้อความ `Senses Property Management Company Limited`
- ที่อยู่ `90 CW Tower, Tower A, Unit A1801, 18th Floor, Ratchadaphisek Road, Huai Khwang, Huai Khwang, Bangkok 10310, Thailand`
- หมายเลข `+66 2643 7595`
- เว็บไซต์ `www.senses.co.th`

## 5. Banner Rendering Rule

- ต้องใช้รูปภาพจริงแบบ **inline image**
- ตำแหน่งต้องอยู่ **ต่อจากข้อมูลติดต่อของผู้ใช้ (Mobile / Mail)**
- ห้ามใช้ข้อความ placeholder แทนภาพเมื่อไฟล์ภาพต้นฉบับพร้อมใช้งาน
- ห้ามสร้างภาพใหม่ เลียนแบบ เปลี่ยนสี เปลี่ยนข้อความ ครอป หรือแก้ดีไซน์โดยไม่ได้รับอนุมัติ
- ถ้าไฟล์ภาพต้นฉบับไม่สามารถเข้าถึงได้ในบริบทปัจจุบัน ต้องแจ้งผู้ใช้ตามจริง และห้ามอ้างว่าได้แทรกโลโก้แล้ว
- การมีลายเซ็นข้อความเพียงอย่างเดียวไม่ถือว่าครบมาตรฐาน หากภาพแบนเนอร์ต้นฉบับพร้อมใช้งาน

## 6. Required Order

ส่วนท้ายอีเมลต้องเรียงดังนี้:

1. Best Regards
2. ชื่อผู้ใช้
3. ตำแหน่ง
4. บริษัท
5. Mobile
6. Mail
7. Company Signature Banner — `SENSES Rev (3).jpg`

## 7. Gmail Draft Rule

เมื่อ AI สร้างหรือแก้ Gmail Draft:
- ต้องพยายามใส่แบนเนอร์ต้นฉบับเป็น inline image เมื่อเครื่องมือรองรับและไฟล์พร้อมใช้งาน
- ห้ามส่งอีเมลจริงจนกว่าผู้ใช้จะสั่งส่งอย่างชัดเจน
- หากข้อจำกัดของเครื่องมือทำให้ไม่สามารถฝัง inline image ได้ ให้แจ้งข้อจำกัดนั้นอย่างตรงไปตรงมา
- ห้ามอ้างว่า Draft มีแบนเนอร์ หากไม่ได้แทรกภาพจริง

## 8. Relationship to Other Email Standards

หากมาตรฐานอีเมลเฉพาะประเภทมีส่วนลายเซ็นหรือ Company Banner ให้ตีความร่วมกับเอกสารนี้

เอกสารนี้เป็นมาตรฐานกลางสำหรับ **ลายเซ็นและแบนเนอร์ในอีเมลทุกประเภทของผู้ใช้** ส่วนโครงสร้างเนื้อหาเฉพาะงานให้ใช้มาตรฐานของงานนั้นต่อไป

## 9. AI Decision Rule

**Every user email must end with the approved Sittipong signature followed immediately by the approved Senses company banner, unless the user explicitly instructs otherwise for that email. Never claim the banner is present unless the actual image has been inserted.**
