# KB Governance — KB Constitution v1.0

**Document ID:** KB-GOV-001  
**Title:** Security Knowledge Base Governance  
**Version:** 1.0  
**Status:** Active  
**Owner:** KB Owner  
**Primary AI Operator:** ChatGPT  
**Effective Date:** 2026-08-16  

---

## 1. Purpose

เอกสารนี้กำหนดกฎกลางสำหรับ `security-knowledge-base` ซึ่งเป็น **AI-First Knowledge Base** สำหรับ Security Operations, Emergency Procedures, Incident Management และความรู้ที่เกี่ยวข้อง

KB นี้ออกแบบให้ AI โดยเฉพาะ ChatGPT สามารถค้นหา ตีความ เชื่อมโยง และนำความรู้ที่ได้รับการอนุมัติไปใช้งานได้อย่างเป็นระบบ โดยมีมนุษย์เป็นผู้มีอำนาจอนุมัติสูงสุด

---

## 2. KB Constitution

### Rule 1 — Single Source of Truth

เรื่องเดียวกันต้องมีเอกสารหลักเพียงหนึ่งแหล่งที่ถือเป็นแหล่งความจริงของ KB

หากมีเอกสารซ้ำหรือข้อมูลขัดแย้งกัน ต้องระบุเอกสารหลักให้ชัดเจน และไม่ถือว่าเอกสารหลายฉบับเป็น SOP ที่มีสถานะเท่าเทียมกัน

### Rule 2 — Knowledge Separation

ต้องแยกประเภทความรู้อย่างชัดเจน เช่น:

- Policy — สิ่งที่องค์กรกำหนด
- Procedure — วิธีปฏิบัติ
- Roles & Responsibilities — บทบาทและหน้าที่
- Decision Rules — หลักเกณฑ์การตัดสินใจ
- Reference — ข้อมูลอ้างอิง
- Template — แบบฟอร์มและต้นแบบ
- Report — ผลลัพธ์หรือบันทึกจากการปฏิบัติงาน

### Rule 3 — Document Identity

เอกสารสำคัญต้องมีตัวตนที่ตรวจสอบได้ เช่น Document ID, Title, Version, Status, Owner และวันที่ที่เกี่ยวข้อง

### Rule 4 — Version Control

การเปลี่ยนแปลงสาระสำคัญต้องเพิ่ม Version และบันทึกประวัติการเปลี่ยนแปลงอย่างชัดเจน

### Rule 5 — No “Latest”

ห้ามใช้ชื่อไฟล์หรือสถานะที่กำกวม เช่น `latest`, `final`, `new`, `ล่าสุด`, `FINAL FINAL` เพื่อระบุเอกสารที่ใช้งานอยู่ ให้ใช้ Version และ Status แทน

### Rule 6 — Archive

เอกสารที่ถูกแทนที่หรือยกเลิกต้องเก็บประวัติไว้ใน Archive ตามความเหมาะสม ห้ามลบประวัติความรู้โดยไม่มีเหตุผลและการอนุมัติ

### Rule 7 — Ownership

เอกสารสำคัญต้องมี Owner ที่รับผิดชอบเนื้อหาและการทบทวนเอกสาร

### Rule 8 — AI Guardrail

AI ต้องไม่สร้างกฎ ขั้นตอน หรือข้อกำหนดขององค์กรขึ้นเองแล้วนำเสนอเป็นข้อมูลที่ได้รับการอนุมัติ หากไม่พบข้อมูลใน KB ให้ระบุว่าไม่พบข้อมูลใน KB และแยกคำแนะนำออกจากข้อเท็จจริงอย่างชัดเจน

### Rule 9 — Change Approval

การสร้าง แก้ไข ลบ ย้าย หรือเปลี่ยนแปลงข้อมูลใด ๆ ใน KB ต้องได้รับการอนุมัติจากเจ้าของ KB ก่อนดำเนินการทุกครั้ง

การสนทนาหรือคำสั่งก่อนหน้าไม่ถือเป็นการอนุมัติสำหรับการเปลี่ยนแปลงครั้งใหม่ เว้นแต่เจ้าของ KB ระบุอนุมัติอย่างชัดเจน

### Rule 10 — AI-First Design

ข้อมูลทุกส่วนต้องออกแบบให้ AI อ่านและตีความได้ชัดเจน มีโครงสร้าง ความสัมพันธ์ แหล่งที่มา สถานะ และ Version ที่ตรวจสอบได้ และต้องลดความกำกวมของภาษา

เมื่อไม่มีข้อมูลที่เพียงพอ AI ต้องไม่เติมข้อมูลจากการคาดเดาแล้วนำเสนอเป็นข้อเท็จจริงขององค์กร

### Rule 11 — AI Authority & Human Approval

ChatGPT เป็น AI หลักและผู้ดำเนินการที่ได้รับมอบหมายให้สร้าง แก้ไข ปรับปรุง และจัดโครงสร้าง KB

อย่างไรก็ตาม ChatGPT ไม่มีอำนาจอนุมัติการเปลี่ยนแปลงด้วยตนเอง การเปลี่ยนแปลงทุกครั้งต้องได้รับการอนุมัติจากเจ้าของ KB ก่อนเขียนลง Repository

AI ห้ามอนุมัติงานของตัวเอง

---

## 3. Change Workflow

การเปลี่ยนแปลง KB ต้องดำเนินตามลำดับ:

```text
Request / Requirement
        ↓
ChatGPT วิเคราะห์
        ↓
Change Proposal
        ↓
เจ้าของ KB ตรวจสอบ
        ↓
อนุมัติหรือไม่อนุมัติ
        ↓
[อนุมัติ]
        ↓
ChatGPT ดำเนินการแก้ไข KB
        ↓
Version / Change Log
        ↓
GitHub Repository
```

หากไม่ได้รับอนุมัติ:

```text
Proposal → รอ / ยกเลิก
             ↓
       ห้ามแก้ KB
```

---

## 4. Required Change Proposal

ก่อนแก้ KB ต้องระบุอย่างน้อย:

- สิ่งที่ต้องการเปลี่ยน
- เหตุผล
- ไฟล์ที่จะได้รับผลกระทบ
- ผลกระทบที่คาดว่าจะเกิดขึ้น
- Version ที่เกี่ยวข้อง
- เนื้อหาหรือแนวทางใหม่โดยสรุป
- สถานะ: `Pending Approval`

หลังเจ้าของ KB อนุมัติแล้วจึงเปลี่ยนสถานะเป็น `Approved` และดำเนินการแก้ไข

---

## 5. AI Operating Principles

ChatGPT ต้อง:

1. ใช้ KB เป็นแหล่งอ้างอิงหลักเมื่อคำถามอยู่ในขอบเขตของ KB
2. แยกข้อเท็จจริงจากข้อเสนอแนะ
3. ไม่สร้าง Policy หรือ SOP จากการคาดเดา
4. ระบุเมื่อข้อมูลไม่พบหรือไม่เพียงพอ
5. เคารพ Version และ Status ของเอกสาร
6. ไม่แก้ KB โดยไม่ได้รับอนุมัติ
7. ไม่อนุมัติการเปลี่ยนแปลงของตนเอง

---

## 6. Authority Model

```text
KB Owner
   │
   │ Authority / Approval
   ▼
ChatGPT
   │
   │ Create / Edit / Organize
   ▼
Security Knowledge Base
   │
   ▼
AI Retrieval / Reasoning / Response
```

**หลักการ:** มนุษย์เป็นผู้มีอำนาจตัดสินใจ ส่วน ChatGPT เป็นผู้ดำเนินการด้าน Knowledge Base

---

## 7. Status Definitions

| Status | ความหมาย |
|---|---|
| `Draft` | อยู่ระหว่างจัดทำ ยังไม่ถือเป็นข้อกำหนดใช้งาน |
| `Pending Approval` | รอเจ้าของ KB อนุมัติ |
| `Active` | ได้รับอนุมัติและเป็นข้อมูลที่ใช้งานอยู่ |
| `Superseded` | ถูกเอกสาร Version ใหม่แทนที่ |
| `Obsolete` | ยกเลิกและไม่ควรใช้งาน |
| `Archived` | เก็บไว้เพื่อประวัติ/อ้างอิง |

---

## 8. Governance Principle

> **Human approves. ChatGPT operates. GitHub records. AI retrieves and reasons from approved knowledge.**

กฎฉบับนี้เป็นข้อกำหนดกลางของ `security-knowledge-base` และเอกสารอื่นภายใน KB ต้องไม่ขัดแย้งกับกฎนี้
