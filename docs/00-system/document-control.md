# Document Control Standard

**Document ID:** KB-SYS-002  
**Title:** Document Control Standard  
**Version:** 1.0  
**Status:** Active  
**Owner:** KB Owner  
**Primary AI Operator:** ChatGPT  
**Effective Date:** 2026-08-16  

---

## 1. Purpose

กำหนดมาตรฐานกลางสำหรับการระบุ จัดประเภท ควบคุม Version สถานะ เจ้าของ และประวัติการเปลี่ยนแปลงของเอกสารใน `security-knowledge-base`

มาตรฐานนี้มีเป้าหมายให้มนุษย์และ AI สามารถระบุได้ว่าเอกสารใดคือเอกสารหลัก เอกสารใดใช้งานอยู่ และเอกสารใดถูกแทนที่แล้ว

---

## 2. Required Metadata

เอกสารที่เป็น Policy, Procedure, Decision Rule หรือเอกสารปฏิบัติการสำคัญควรมี Metadata ด้านบนในรูปแบบ YAML:

```yaml
---
document_id: SEC-CODE-M-001
title: Code M — Medical Emergency Procedure
version: 1.0
status: Active
owner: Security Operations
effective_date: 2026-08-16
review_date: 2027-08-16
---
```

### Metadata ที่กำหนด

| Field | ความหมาย |
|---|---|
| `document_id` | รหัสเอกสารที่ไม่ซ้ำกัน |
| `title` | ชื่อเอกสาร |
| `version` | Version ปัจจุบัน |
| `status` | สถานะของเอกสาร |
| `owner` | ผู้/หน่วยงานรับผิดชอบ |
| `effective_date` | วันที่เริ่มมีผล |
| `review_date` | วันที่ควรทบทวน |

---

## 3. Document ID

Document ID ต้องไม่ซ้ำกันภายใน KB และควรสื่อถึงหมวดของเอกสาร

ตัวอย่าง:

```text
KB-SYS-001      Governance
KB-SYS-002      Document Control
SEC-CODE-M-001  Code M Procedure
SEC-COM-001     Communication Standard
SEC-INC-001     Incident Management
```

เมื่อสร้าง Document ID แล้ว ไม่ควรเปลี่ยน ID เพียงเพราะมีการแก้ Version

---

## 4. Versioning

ใช้หลัก Semantic Versioning แบบเรียบง่ายสำหรับเอกสาร:

### Major — `2.0`

ใช้เมื่อมีการเปลี่ยนแปลงโครงสร้างหรือหลักปฏิบัติที่มีผลอย่างมีนัยสำคัญ

### Minor — `1.1`

ใช้เมื่อมีการเพิ่มหรือปรับปรุงเนื้อหาโดยไม่เปลี่ยนหลักการหลักของเอกสาร

### Patch — `1.0.1`

ใช้สำหรับการแก้ไขคำผิด การสะกด การจัดรูปแบบ หรือการแก้ไขเล็กน้อยที่ไม่เปลี่ยนความหมายเชิงปฏิบัติการ

หากไม่แน่ใจว่าเป็น Major, Minor หรือ Patch ให้ ChatGPT เสนอการจัดประเภทและรอการอนุมัติจาก KB Owner

---

## 5. Status

สถานะต้องใช้ค่าที่กำหนดใน `kb-governance.md` ได้แก่:

- `Draft`
- `Pending Approval`
- `Active`
- `Superseded`
- `Obsolete`
- `Archived`

ห้ามสร้างสถานะใหม่โดยพลการโดยไม่ผ่านกระบวนการอนุมัติ KB

---

## 6. Change Log

เอกสารที่มีการเปลี่ยนแปลงสาระสำคัญต้องมี Change Log เช่น:

```markdown
## Change Log

| Version | Date | Change | Approved By |
|---|---|---|---|
| 1.0 | 2026-08-16 | Initial version | KB Owner |
```

การเปลี่ยนแปลงที่ยังไม่ได้รับอนุมัติห้ามบันทึกเป็น Version ที่ Active

---

## 7. Review

เอกสารที่มี `review_date` ต้องได้รับการทบทวนตามกำหนด โดยการทบทวนไม่ได้หมายความว่าเนื้อหาจะถูกแก้ไขโดยอัตโนมัติ

หากต้องแก้ไข ต้องเข้าสู่ Change Approval Workflow ตาม `kb-governance.md`

---

## 8. AI Document Handling Rules

ChatGPT ต้อง:

1. อ่าน Metadata ก่อนใช้เอกสารเป็นแหล่งอ้างอิง
2. ให้ความสำคัญกับเอกสาร `Active` มากกว่าเอกสาร `Superseded`, `Obsolete` หรือ `Archived`
3. ไม่ใช้เอกสารที่ไม่ได้รับการอนุมัติเป็นข้อกำหนดขององค์กร
4. ตรวจสอบ Version เมื่อมีเอกสารหลาย Version
5. ไม่เปลี่ยน Document ID โดยไม่ได้รับอนุมัติ
6. เสนอ Change Log ทุกครั้งที่มีการเปลี่ยนแปลงสาระสำคัญ
7. ขออนุมัติก่อนเขียนการเปลี่ยนแปลงลง Repository ทุกครั้ง

---

## 9. File Naming

ชื่อไฟล์ควรใช้รูปแบบ `lowercase-with-hyphen.md`

ตัวอย่างที่ถูกต้อง:

```text
procedure.md
decision-flow.md
communication-standard.md
incident-classification.md
```

หลีกเลี่ยง:

```text
FINAL.md
ล่าสุด.md
new-final.md
SOP FINAL FINAL.md
```

Version และ Status ต้องอยู่ใน Metadata ไม่ใช่ชื่อไฟล์

---

## 10. Source and Traceability

เมื่อเอกสารอ้างอิงข้อมูลจากเอกสารอื่นใน KB ต้องใช้ลิงก์หรือระบุ Document ID ของแหล่งข้อมูล เพื่อให้ AI สามารถย้อนกลับไปตรวจสอบต้นทางได้

ข้อมูลภายนอกที่นำเข้ามาเป็น Knowledge ใหม่ต้องผ่านการตรวจสอบและอนุมัติก่อนจึงจะถือเป็นข้อมูลของ KB

---

## 11. Approval Principle

> **No approval, no KB change.**

การสร้าง แก้ไข ลบ ย้าย หรือเปลี่ยนสถานะของเอกสารต้องอยู่ภายใต้ Change Approval Workflow ที่กำหนดใน `kb-governance.md`
