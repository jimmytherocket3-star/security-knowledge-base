# Canonical Terminology

**Document ID:** KB-SYS-003  
**Title:** Canonical Terminology  
**Version:** 1.3  
**Status:** Active  
**Owner:** KB Owner  
**Primary AI Operator:** ChatGPT  
**Effective Date:** 2026-08-23  

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
| **CI** | Common Infrastructure | พื้นที่ลานจอดรถหรือพื้นที่ภายนอกอาคาร |
| **SMT** | Security Manage Traffic Team | ทีมที่เน้นการดูแลการจราจรและพื้นที่ภายนอกอาคารเป็นหลัก |
| **BMO** | Building Manager | Building Manager; ทำหน้าที่ Incident Commander / ผบ.เหตุฉุกเฉิน สำหรับพื้นที่อาคาร |
| **DM Retail** | Direct Manager Retail | Direct Manager Retail; ทำหน้าที่ Incident Commander / ผบ.เหตุฉุกเฉิน สำหรับพื้นที่ Retail |
| **Incident Commander** | — | ผบ.เหตุฉุกเฉิน; พื้นที่อาคารคือ BMO และพื้นที่ Retail คือ DM Retail |
| **Echo (E)** | — | ชื่อทีมย่อยของ EOT สำหรับการเผชิญและระงับเหตุเพลิงไหม้ |
| **Oscar (O)** | — | ชื่อทีมย่อยของ EOT ทำหน้าที่ Search and Rescue ในพื้นที่เกิดเหตุเพลิงไหม้ |
| **Tango (T)** | — | ชื่อทีมย่อยของ EOT ทำหน้าที่ Medical และตั้ง Medical Point ณ จุดอพยพ |
| **FACP** | Fire Alarm Control Panel | ตู้ควบคุมระบบแจ้งเตือนอัคคีภัย |
| **PA** | Public Announcement | ระบบเสียงประกาศ |
| **Strobe** | Strobe Light | ไฟกระพริบฉุกเฉิน |
| **AHU** | Air Handle Unit | ระบบควบคุมแอร์ภายในอาคาร |
| **Access Control** | — | ระบบควบคุมการเข้า-ออก |
| **General Alarm** | — | สัญญาณเตือนภัยขั้นสุดท้ายทั่วทั้งอาคาร และเป็น System Trigger ของ Code 3 ตามเอกสาร Code 3 |
| **PCS** | — | ชื่อบริษัทต้นสังกัดของเจ้าหน้าที่ รปภ.; ใน Knowledge Code 2 รปภ. PCS รับผิดชอบพื้นที่ภายในอาคาร |
| **G4S** | — | ชื่อบริษัทต้นสังกัดของเจ้าหน้าที่ รปภ.; ใน Knowledge Code 2 รปภ. G4S รับผิดชอบพื้นที่ภายนอกอาคารและการอำนวยความสะดวกให้รถดับเพลิง |
| **Mozart** | — | ระบบที่ใช้สำหรับจัดการ Case และบันทึก/อัปเดตเหตุการณ์ของ SOC; เมื่อเป็นการแจ้งเตือนผ่านอุปกรณ์ ระบบ Mozart จะสร้าง Case โดยอัตโนมัติ |
| **Code M** | Medical Emergency | เหตุฉุกเฉินทางการแพทย์ |
| **Emergency Channel** | — | ช่องวิทยุสื่อสารสำหรับเหตุฉุกเฉิน โดยใช้ตัวย่อ **EMER1** |
| **EMER1** | Emergency Channel | ช่องวิทยุสื่อสารที่ใช้สำหรับเหตุฉุกเฉิน |
| **Incident** | — | เหตุ |
| **Case** | — | กรณี |

---

## 3. AI Interpretation Rules

เมื่อพบคำศัพท์ในรายการ Canonical Terms ให้ AI ใช้ความหมายตามตารางนี้เป็นมาตรฐานกลาง และใช้รายละเอียดเชิงกระบวนการจากเอกสาร Emergency Code ที่เกี่ยวข้อง

### 3.1 Incident Commander

- พื้นที่อาคาร: BMO (Building Manager)
- พื้นที่ Retail: DM Retail (Direct Manager Retail)

### 3.2 EOT Fire Response Subteams

- Echo = Fire Response
- Oscar = Search and Rescue ในพื้นที่เกิดเหตุเพลิงไหม้
- Tango = Medical และตั้ง Medical Point ณ จุดอพยพ

Echo, Oscar และ Tango เป็นชื่อทีมย่อยของ EOT ในการเผชิญเหตุเพลิงไหม้ ไม่ใช่หน่วยงานแยกจาก EOT

### 3.3 CI / SMT

CI หมายถึงพื้นที่ลานจอดรถหรือพื้นที่ภายนอกอาคาร และ SMT เป็นทีมที่เน้นการดูแลการจราจรและพื้นที่ภายนอกอาคารเป็นหลัก

### 3.4 PCS / G4S

PCS และ G4S เป็นชื่อบริษัทต้นสังกัดของเจ้าหน้าที่ รปภ. ไม่ใช่ชื่อ Emergency Response Team

### 3.5 General Alarm

General Alarm ให้ตีความตามเอกสาร Code 3 และเป็น System Trigger ของ Code 3

### 3.6 Mozart

Mozart เป็นระบบที่ SOC ใช้สำหรับจัดการ Case และบันทึก/อัปเดตเหตุการณ์ โดยในกรณีการแจ้งเตือนผ่านอุปกรณ์ ระบบสามารถสร้าง Case โดยอัตโนมัติ

### 3.7 Emergency Channel / EMER1

Emergency Channel และ EMER1 อ้างถึงช่องวิทยุสื่อสารสำหรับเหตุฉุกเฉินตาม KB

### 3.8 Incident / Case

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
