# Canonical Terminology

**Document ID:** KB-SYS-003  
**Title:** Canonical Terminology  
**Version:** 1.4  
**Status:** Active  
**Owner:** KB Owner  
**Primary AI Operator:** ChatGPT  
**Effective Date:** 2026-08-30  

---

## 1. Purpose

เอกสารนี้เป็นแหล่งความจริงกลาง (Canonical Source) สำหรับคำศัพท์ คำย่อ และคำจำกัดความที่ใช้ใน `security-knowledge-base`

AI โดยเฉพาะ ChatGPT ต้องยึดคำจำกัดความในเอกสารนี้เมื่อประมวลผลข้อมูลภายใน KB และต้องไม่ตีความคำย่อเหล่านี้ขึ้นใหม่โดยไม่มีข้อมูลหรือการอนุมัติจาก KB Owner

---

## 2. Canonical Terms

| Term | Full Name | คำจำกัดความมาตรฐาน |
|---|---|---|
| **SS** | Security Supervisor | Security Supervisor ผู้รับผิดชอบงานในบทบาท Security Supervisor |
| **SOC** | Security Operation Center | ทีมที่คอยบริหารจัดการเหตุด้าน Security ผ่าน CCTV |
| **FCC** | Fire Command Center | ทีม Fire Command Center ประกอบด้วยทีม รปภ. และ Fireman ที่อยู่ตามพื้นที่ Retail |
| **EOT** | Emergency Operation Team | ทีมสำหรับเผชิญเหตุฉุกเฉินที่เกี่ยวข้องกับ Security |
| **DCC** | District Command Centre | District Command Centre |
| **IMT** | Incident Management Team | กลุ่มผู้มีบทบาทในการบริหารและตัดสินใจเหตุฉุกเฉิน; ในขอบเขต Knowledge ที่อนุมัติประกอบด้วย Incident Commander, Building Manager, DCC และสำหรับพื้นที่ Retail คือ DM Retail ตามพื้นที่รับผิดชอบ |
| **CI** | Common Infrastructure | พื้นที่ลานจอดรถหรือพื้นที่ภายนอกอาคาร |
| **SMT** | Security Manage Traffic Team | ทีมที่เน้นการดูแลการจราจรและพื้นที่ภายนอกอาคารเป็นหลัก |
| **BMO** | Building Manager | Building Manager; ทำหน้าที่ Incident Commander / ผบ.เหตุฉุกเฉิน สำหรับพื้นที่อาคาร |
| **DM Retail** | Direct Manager Retail | Direct Manager Retail; ทำหน้าที่ Incident Commander / ผบ.เหตุฉุกเฉิน สำหรับพื้นที่ Retail และเป็น All Clear Authority ของพื้นที่ Retail |
| **Incident Commander** | — | ผบ.เหตุฉุกเฉิน; เป็นหนึ่งในผู้มีบทบาทด้านการบริหารและตัดสินใจเหตุฉุกเฉินใน IMT |
| **Echo (E)** | — | ชื่อทีมย่อยของ EOT สำหรับการเข้าเผชิญเหตุ Code 2 |
| **Oscar (O)** | — | ชื่อทีมย่อยของ EOT ทำหน้าที่ Search & Rescue |
| **Tango (T)** | — | ชื่อทีมย่อยของ EOT ทำหน้าที่ Medic |
| **FACP** | Fire Alarm Control Panel | ตู้ควบคุมระบบแจ้งเตือนอัคคีภัย |
| **PA** | Public Announcement | ระบบเสียงประกาศ |
| **Strobe** | Strobe Light | ไฟกระพริบฉุกเฉิน |
| **AHU** | Air Handle Unit | ระบบควบคุมแอร์ภายในอาคาร |
| **Access Control** | — | ระบบควบคุมการเข้า-ออก |
| **General Alarm** | — | สัญญาณเตือนภัยขั้นสุดท้ายทั่วทั้งอาคาร และเป็น System Trigger ของ Code 3 ตามเอกสาร Code 3 |
| **PCS** | — | ชื่อบริษัทต้นสังกัดของเจ้าหน้าที่ รปภ.; รับผิดชอบภายในอาคารรวมถึงพื้นที่ Retail ตาม Knowledge Code 3 |
| **G4S** | — | ชื่อบริษัทต้นสังกัดของเจ้าหน้าที่ รปภ.; รับผิดชอบภายนอกอาคาร สนับสนุนการอพยพภายนอก การจราจร และการนำทางไป Assembly Point ตาม Knowledge Code 3 |
| **Mozart** | — | ระบบที่ใช้สำหรับจัดการ Case และบันทึก/อัปเดตเหตุการณ์ของ SOC; เมื่อเป็นการแจ้งเตือนผ่านอุปกรณ์ ระบบ Mozart จะสร้าง Case โดยอัตโนมัติ |
| **Code M** | Medical Emergency | เหตุฉุกเฉินทางการแพทย์ |
| **Emergency Channel** | — | ช่องวิทยุสื่อสารสำหรับเหตุฉุกเฉิน |
| **EMER_1** | Emergency Channel — Primary | ช่องวิทยุสื่อสารฉุกเฉินหลักสำหรับ Code 3 |
| **EMER_2** | Emergency Channel — Backup | ช่องวิทยุสื่อสารฉุกเฉินสำรอง ใช้เมื่อ EMER_1 เกิดปัญหา |
| **สดพ.บ่อนไก่** | สถานีดับเพลิงบ่อนไก่ | สถานีดับเพลิงบ่อนไก่; เมื่อมาถึงพื้นที่เกิดเหตุและเตรียมพร้อมเริ่มปฏิบัติงานในพื้นที่เกิดเหตุ ให้ EOT ส่งต่อภารกิจ Search & Rescue ในพื้นที่เกิดเหตุให้ สดพ.บ่อนไก่ ตาม Code 3 |
| **BCP Room** | Business Continuity Plan Room | ศูนย์ปฏิบัติการสำรองของ SOC อยู่ชั้น B1 ใกล้ Load 1 ใต้อาคาร Parade / The Storeys |
| **Assembly Point** | — | จุดรวมพลสำหรับผู้ใช้อาคารในกระบวนการ Evacuation |
| **All Clear** | — | คำสั่งอนุญาตให้เข้าสู่กระบวนการกลับสู่สภาวะปกติหลังการประเมินความปลอดภัย; Building ใช้ Building Manager เป็น Authority และ Retail ใช้ DM Retail |
| **Incident** | — | เหตุ |
| **Case** | — | กรณี |

---

## 3. AI Interpretation Rules

เมื่อพบคำศัพท์ในรายการ Canonical Terms ให้ AI ใช้ความหมายตามตารางนี้เป็นมาตรฐานกลาง และใช้รายละเอียดเชิงกระบวนการจากเอกสาร Emergency Code ที่เกี่ยวข้อง

### 3.1 IMT / Emergency Authority

IMT = Incident Management Team ในขอบเขต Knowledge ที่ได้รับการอนุมัติ ประกอบด้วย Incident Commander, Building Manager, DCC และสำหรับพื้นที่ Retail คือ DM Retail ตามพื้นที่รับผิดชอบ

AI ต้องไม่สร้างรายชื่อบุคคลเฉพาะหรือเพิ่ม Authority อื่นเข้า IMT เองโดยไม่มีการอนุมัติจาก KB Owner

### 3.2 EOT Subteams

- Echo = เข้าเผชิญเหตุ Code 2
- Oscar = Search & Rescue
- Tango = Medic

Echo, Oscar และ Tango เป็นชื่อทีมย่อยของ EOT ไม่ใช่หน่วยงานแยกจาก EOT

### 3.3 Emergency Radio

สำหรับ Code 3:

- EMER_1 = Primary Emergency Radio Channel
- EMER_2 = Backup Emergency Radio Channel เมื่อ EMER_1 เกิดปัญหา

### 3.4 สดพ.บ่อนไก่

คำย่อที่ถูกต้องคือ **สดพ.บ่อนไก่ = สถานีดับเพลิงบ่อนไก่**

คำว่า `สตพ.บ่อนไก่` ที่พบในข้อมูลร่างเก่าไม่ใช่คำย่อมาตรฐานของ KB

### 3.5 BCP Room

BCP Room เป็นศูนย์ปฏิบัติการสำรองของ SOC ชั้น B1 ใกล้ Load 1 ใต้อาคาร Parade / The Storeys ใช้เพื่อรักษาความต่อเนื่องในการปฏิบัติงานเมื่อจำเป็นต้องออกจากหรือไม่สามารถใช้ศูนย์ปฏิบัติการหลักได้

BCP ไม่ใช่กระบวนการเฉพาะ Code 3 และ Code 2 ทุกเหตุไม่ได้หมายความว่า SOC ต้องย้าย BCP โดยอัตโนมัติ

### 3.6 PCS / G4S

PCS และ G4S เป็นชื่อบริษัทต้นสังกัดของเจ้าหน้าที่ รปภ. ไม่ใช่ชื่อ Emergency Response Team

ใน Code 3 PCS รับผิดชอบภายในอาคารรวมถึงพื้นที่ Retail ส่วน G4S รับผิดชอบภายนอกอาคาร สนับสนุนการอพยพภายนอก การจราจร และการนำทางไป Assembly Point

### 3.7 All Clear

- Building: Building Manager เป็น All Clear Authority
- Retail: DM Retail เป็น All Clear Authority

### 3.8 General Alarm

General Alarm ให้ตีความตามเอกสาร Code 3 และเป็น System Trigger ของ Code 3

### 3.9 DCC / DEC Correction

Workflow ที่ได้รับการอนุมัติใช้ **DCC** คำว่า `DEC` ที่พบในข้อมูลร่าง Code 3 ก่อนหน้าเป็นคำที่ไม่ถูกต้องและต้องไม่สร้างเป็น Role ใหม่ใน KB

### 3.10 Mozart

Mozart เป็นระบบที่ SOC ใช้สำหรับจัดการ Case และบันทึก/อัปเดตเหตุการณ์ โดยในกรณีการแจ้งเตือนผ่านอุปกรณ์ ระบบสามารถสร้าง Case โดยอัตโนมัติ

### 3.11 Incident / Case

- Incident = เหตุ
- Case = กรณี

---

## 4. Canonical Source Rule

เมื่อเอกสารภายใน KB ใช้คำศัพท์หรือคำย่อที่อยู่ในรายการนี้ ให้ถือคำจำกัดความจากเอกสารนี้เป็นมาตรฐานกลาง

หากพบคำจำกัดความที่ขัดแย้งกันในเอกสารอื่น ให้ถือว่าเป็น **Terminology Conflict** และ ChatGPT ต้องเสนอให้ KB Owner ตรวจสอบก่อนแก้ไขเอกสารใด ๆ

---

## 5. Adding or Changing Terms

การเพิ่ม แก้ไข หรือลบคำศัพท์ในเอกสารนี้ถือเป็นการเปลี่ยนแปลง KB และต้องผ่าน Change Approval Workflow ตาม `kb-governance.md`

> **No approval, no terminology change.**

---

## 6. Change Log

| Version | Date | Change | Approved By |
|---|---|---|---|
| 1.0 | 2026-08-16 | Initial canonical terminology based on KB Owner definitions | KB Owner |
| 1.1 | 2026-08-17 | Added DCC — District Command Centre | KB Owner |
| 1.2 | 2026-08-18 | Added Mozart Case management, automatic device-alert Case creation, and SOC event recording definition | KB Owner |
| 1.3 | 2026-08-23 | Added approved Code 2/3 terminology: CI, SMT, BMO, DM Retail, Incident Commander, EOT subteams, FACP, PA, Strobe, AHU, Access Control, General Alarm, PCS and G4S | KB Owner |
| 1.4 | 2026-08-30 | Added approved Code 3 operational terminology and corrections: IMT, EMER_1, EMER_2, สดพ.บ่อนไก่, BCP Room, Assembly Point, All Clear, updated EOT/PCS/G4S roles and DEC→DCC guardrail | KB Owner |
