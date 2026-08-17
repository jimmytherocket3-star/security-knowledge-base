# Canonical Terminology

**Document ID:** KB-SYS-003  
**Title:** Canonical Terminology  
**Version:** 1.1  
**Status:** Active  
**Owner:** KB Owner  
**Primary AI Operator:** ChatGPT  
**Effective Date:** 2026-08-17  

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
| **Code M** | Medical Emergency | เหตุฉุกเฉินทางการแพทย์ |
| **Emergency Channel** | — | ช่องวิทยุสื่อสารสำหรับเหตุฉุกเฉิน โดยใช้ตัวย่อ **EMER1** |
| **EMER1** | Emergency Channel | ช่องวิทยุสื่อสารที่ใช้สำหรับเหตุฉุกเฉิน |
| **Incident** | — | เหตุ |
| **Case** | — | กรณี |

---

## 3. AI Interpretation Rules

### 3.1 SS

เมื่อพบคำว่า **SS** ในเอกสารของ KB ให้ตีความตามมาตรฐานนี้ว่า **Security Supervisor**

### 3.2 SOC

เมื่อพบคำว่า **SOC** ให้ตีความว่า **Security Operation Center** ซึ่งเป็นทีมที่คอยบริหารจัดการเหตุด้าน Security ผ่าน CCTV

### 3.3 FCC

เมื่อพบคำว่า **FCC** ให้ตีความว่า **Fire Command Center** ซึ่งประกอบด้วยทีม รปภ. และ Fireman ที่อยู่ตามพื้นที่ Retail

### 3.4 EOT

เมื่อพบคำว่า **EOT** ให้ตีความว่า **Emergency Operation Team** ซึ่งเป็นทีมสำหรับเผชิญเหตุฉุกเฉินที่เกี่ยวข้องกับ Security

### 3.5 DCC

เมื่อพบคำว่า **DCC** ให้ตีความว่า **District Command Centre**

### 3.6 Code M

เมื่อพบคำว่า **Code M** ให้ตีความว่า **Medical Emergency / เหตุฉุกเฉินทางการแพทย์**

### 3.7 Emergency Channel / EMER1

คำว่า **Emergency Channel** และ **EMER1** ให้ถือว่าอ้างถึงช่องวิทยุสื่อสารสำหรับเหตุฉุกเฉินตามคำจำกัดความของ KB

### 3.8 Incident / Case

- **Incident** = เหตุ
- **Case** = กรณี

เอกสารอื่นสามารถกำหนดรายละเอียดเชิงกระบวนการของ Incident หรือ Case เพิ่มเติมได้ แต่ต้องไม่ขัดแย้งกับคำจำกัดความกลางนี้

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
