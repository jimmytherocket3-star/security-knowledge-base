---
document_id: SEC-CODE-3-001
title: Code 3 — General Alarm and Evacuation
version: 0.1
status: Draft
owner: KB Owner
primary_ai_operator: ChatGPT
---

# Code 3 — General Alarm and Evacuation

## 1. Definition

**Code 3 = Evacuation / การอพยพ**

เมื่อเข้าสู่ Code 3 ผู้ใช้อาคารต้องอพยพออกจากพื้นที่ไปยัง **จุดรวมพล (Assembly Point)** เพื่อความปลอดภัย

## 2. Approved Code 3 Triggers

Code 3 มี Trigger 2 ทาง:

### 2.1 System Trigger

ระบบเข้าสู่สถานะ **General Alarm**

### 2.2 Command Trigger

SOC ได้รับแจ้งจาก:

- DCC
- Incident Commander (ผบ.เหตุฉุกเฉิน)

## 3. General Alarm

**General Alarm** คือสัญญาณเตือนภัยขั้นสุดท้ายทั่วทั้งอาคาร ซึ่งจะทำงานโดยอัตโนมัติหากระบบตรวจจับพบเหตุเพลิงไหม้แล้วไม่มีการกดหน่วงเวลาหรือตอบสนองใด ๆ (Action) จากผู้ควบคุมตู้ FACP หรือผู้ Monitor โปรแกรม

## 4. System Escalation Timeline

Mapping ของ Step และ Code:

- **Step 1 = Code 1**
- **Step 2 = Code 2**
- **Step 3 = Code 3**

Timeline ที่ได้รับการยืนยัน:

```text
Fire Detection
     │
     │ 5 minutes
     ▼
CODE 1 / Step 1
     │
     │ +3 minutes
     ▼
CODE 2 / Step 2
     │
     │ +2 minutes
     ▼
CODE 3 / Step 3
     │
     ▼
GENERAL ALARM
```

รวมเวลาตั้งแต่ระบบเริ่มตรวจจับจนถึง General Alarm = **10 นาที** ในกรณีที่ไม่มีการกดหน่วงเวลาหรือ Action จากผู้ควบคุม FACP หรือผู้ Monitor โปรแกรม

> System Escalation Timeline นี้เป็นคนละกลไกกับ Code 1 CAT 1 SLA 5 นาทีสำหรับ SOC Acknowledge Case ใน Mozart และห้ามตีความปะปนกัน

## 5. Automatic Building-System Actions at General Alarm

เมื่อระบบเข้าสู่ General Alarm ระบบป้องกันอัคคีภัยของอาคารจะสั่งการทำงานโดยอัตโนมัติ:

### 5.1 PA Override / Strobe

สัญญาณเตือนภัยและเสียงประกาศตามสายทำงานทั่วทั้งอาคารทุกโซน และ Strobe Light / ไฟกระพริบฉุกเฉินทำงาน

### 5.2 AHU

AHU ปิดการทำงานทั้งหมดทุกโซน (**OFF All Zone**)

### 5.3 Door Unlock

ประตูที่มีระบบ Magnetic, Access Control, ประตูหนีไฟ และ Turnstile ถูกปลดล็อกโดยอัตโนมัติและเปิดค้าง

### 5.4 Elevator

ลิฟต์วิ่งลงไปจอด Standby ที่ชั้น G

### 5.5 Emergency Lighting

Emergency Lighting และไฟในเส้นทางบันไดหนีไฟเปิดทำงานทั้งหมด

## 6. Evacuation

เมื่อเข้าสู่ General Alarm / Code 3 ผู้ใช้อาคารต้องอพยพออกจากพื้นที่ไปยังจุดรวมพล (Assembly Point)

รายละเอียดการควบคุมการอพยพ เส้นทาง จุดรวมพลเฉพาะพื้นที่ การตรวจนับ และการสิ้นสุด Code 3 ยังไม่ได้กำหนดในเอกสารฉบับนี้

## 7. Incident Commander

**Incident Commander = ผบ.เหตุฉุกเฉิน**

- พื้นที่อาคาร — BMO (Building Manager)
- พื้นที่ Retail — DM Retail (Direct Manager Retail)

Incident Commander หรือ DCC สามารถเป็น Command Trigger ให้ SOC เข้าสู่กระบวนการ Code 3 ได้

## 8. AI Guardrails

- Code 3 มี Trigger ที่อนุมัติ 2 ทาง: General Alarm หรือการแจ้งจาก DCC / Incident Commander
- ห้ามใช้เงื่อนไข `EOT ควบคุมเหตุไม่ได้ → Fire Brigade Support → สถานการณ์รุนแรง` เป็น Trigger หรือเงื่อนไขพิจารณา Code 3
- ห้ามนำ System Escalation Timeline 5+3+2 นาทีไปตีความเป็น Code 1 CAT 1 SLA
- ห้ามเติมรายละเอียดการอพยพที่ยังไม่ได้รับการยืนยันจาก KB Owner

## 9. Change Log

| Version | Change | Approved By |
|---|---|---|
| 0.1 | Initial approved Code 3 knowledge: two triggers, General Alarm definition, 5+3+2 system escalation timeline, automatic building-system actions and evacuation linkage | KB Owner |
