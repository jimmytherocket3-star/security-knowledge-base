---
document_id: SEC-CODE-2-001
title: Code 2 — Confirmed Fire Incident and Response
version: 0.1
status: Draft
owner: KB Owner
primary_ai_operator: ChatGPT
---

# Code 2 — Confirmed Fire Incident and Response

## 1. Definition

**Code 2** คือเหตุเพลิงไหม้ที่ได้รับการยืนยันว่าเกิดขึ้นจริง ไม่ว่าเพลิงจะยังลุกไหม้อยู่หรือดับไปแล้วก็ตาม

## 2. Authority and Confirmation

**SOC (Security Operation Center)** เป็นผู้มีอำนาจประกาศ Code 2 หลังตรวจสอบและยืนยันว่าเป็นเหตุเพลิงไหม้จริง โดยใช้ข้อมูลจาก:

- CCTV
- รายงานจาก รปภ. ในพื้นที่
- รายงานจากช่างในพื้นที่ที่ได้รับแจ้งเหตุ

## 3. Notification after Code 2 Declaration

เมื่อ SOC ประกาศ Code 2 ให้ดำเนินการ:

1. แจ้ง EOT เพื่อรับทราบและเข้าระงับเหตุเพลิงไหม้
2. แจ้ง DCC เพื่อรับทราบ
3. แจ้งฝ่ายอาคารใกล้เคียงเพื่อรับทราบ

เกณฑ์ว่าอาคารใดถือเป็นอาคารใกล้เคียงและช่องทางการแจ้งยังไม่ได้รับการกำหนดใน Knowledge ชุดนี้ AI ต้องไม่เดาเอง

## 4. EOT Response

เมื่อได้รับแจ้ง Code 2 ทีม EOT ต้องสวมชุดกันไฟและออกปฏิบัติพร้อมกันทันที โดยแบ่งเป็น 3 ทีมย่อย:

| Team | Function |
|---|---|
| **Echo (E)** | ทีมเผชิญเหตุและระงับเหตุเพลิงไหม้ |
| **Oscar (O)** | Search and Rescue ในพื้นที่เกิดเหตุเพลิงไหม้ |
| **Tango (T)** | Medical และตั้ง Medical Point ณ จุดอพยพ |

หากยังมีเพลิงไหม้อยู่ EOT/Echo ต้องเข้าดับเพลิงอย่างเต็มที่ หากเพลิงดับไปแล้ว EOT ต้องตรวจสอบพื้นที่เกิดเหตุและพื้นที่โดยรอบว่ามีความเสี่ยงที่จะเกิดเพลิงไหม้ซ้ำหรือไม่

## 5. Emergency Communication — EMER1

Code 2 ใช้ช่องวิทยุ **EMER1** โดยมี:

- SOC
- DCC
- EOT
- SS ของ รปภ. ในพื้นที่

ตามประเภทพื้นที่:

- **CI (Common Infrastructure)** — เพิ่ม SMT ในช่อง EMER1
- **Retail** — เพิ่ม FCC ของ Retail นั้นในช่อง EMER1

## 6. Security and Area Control

รปภ. ในพื้นที่มีหน้าที่กันพื้นที่และช่วยเหลือเมื่อมีการอพยพบุคคลออกจากพื้นที่

- ภายในอาคาร — รปภ. สังกัด **PCS**
- ภายนอกอาคาร — รปภ. สังกัด **G4S**
- การนำทางและอำนวยความสะดวกให้รถดับเพลิง — รปภ. **G4S**

PCS และ G4S เป็นชื่อบริษัทต้นสังกัดของ รปภ. ไม่ใช่ชื่อ Emergency Response Team

## 7. SOC Responsibilities

ระหว่าง Code 2 SOC มีหน้าที่:

- Monitor CCTV
- Monitor Body Camera ที่ติดอยู่กับทีม EOT
- รับแจ้งและประสานงาน
- บันทึกและอัปเดต Case ผ่านระบบ Mozart
- สืบค้นหาสาเหตุของเพลิงไหม้โดยใช้ CCTV เป็นหลัก แม้เพลิงจะดับไปแล้ว

## 8. Incident Commander

**Incident Commander = ผบ.เหตุฉุกเฉิน** โดยขึ้นอยู่กับพื้นที่:

- พื้นที่อาคาร — **BMO (Building Manager)**
- พื้นที่ Retail — **DM Retail (Direct Manager Retail)**

## 9. Electrical Isolation and Water Suppression

กรณีเหตุเพลิงไหม้รุนแรงที่ EOT ร้องขอการตัดกระแสไฟเพื่อให้สามารถใช้น้ำระงับเหตุ:

1. EOT ร้องขอการตัดกระแสไฟฟ้า
2. SOC รับการยืนยันการตัดกระแสไฟจาก Incident Commander
3. SOC แจ้ง EOT ว่าได้รับการยืนยันการตัดกระแสไฟแล้ว
4. EOT ดำเนินการระงับเหตุด้วยน้ำตามสถานการณ์

## 10. External Fire Brigade Support

หาก EOT ไม่สามารถระงับเหตุและร้องขอกำลังสนับสนุน SOC มีหน้าที่ประสาน **สถานีดับเพลิงบ่อนไก่** เพื่อขอกำลังสนับสนุน

การร้องขอ Fire Brigade Support ไม่ใช่ Trigger ของ Code 3 โดยตัวมันเอง

## 11. Relationship to Code 3

Code 3 ไม่ได้ถูก Trigger จากเงื่อนไขว่า EOT ควบคุมเหตุไม่ได้หรือจากการร้องขอ Fire Brigade Support โดยอัตโนมัติ

Trigger ของ Code 3 ให้ยึดตามเอกสาร Code 3 โดยเฉพาะ

## 12. AI Guardrails

- หากยืนยันว่าเคยเกิดเพลิงไหม้จริง แม้เพลิงดับแล้ว ให้ถือเป็น Code 2
- CCTV เป็นแหล่งหลักสำหรับ SOC ในการสืบค้นหาสาเหตุเพลิงไหม้
- AI ต้องไม่สร้างเกณฑ์ Code 3 จากความรุนแรงของเหตุ การควบคุมเหตุไม่ได้ หรือการร้องขอ Fire Brigade Support นอกเหนือจาก Trigger ที่ได้รับการอนุมัติ
- AI ต้องไม่กำหนดอาคารใกล้เคียงหรือช่องทางการแจ้งอาคารใกล้เคียงเอง

## 13. Change Log

| Version | Change | Approved By |
|---|---|---|
| 0.1 | Initial approved Code 2 knowledge: confirmed fire definition, authority, EOT structure, EMER1, area control, SOC monitoring/investigation, Incident Commander, electrical isolation and external fire brigade support | KB Owner |
