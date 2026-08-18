---
document_id: SEC-CODE-1-001
title: Code 1 — Fire Alarm Notification and Verification
version: 0.4
status: Draft
owner: KB Owner
primary_ai_operator: ChatGPT
---

# Code 1 — Fire Alarm Notification and Verification

## 1. Current Definition

**Code 1** คือการแจ้งเตือนอัคคีภัยที่มาจากบุคคล ระบบ หรืออุปกรณ์ตรวจจับ โดยมีเป้าหมายของขั้นตอนคือ **VERIFY** หรือการตรวจสอบและพิสูจน์เหตุ

## 2. Trigger Sources

Code 1 สามารถเริ่มจากการแจ้งเตือนอัคคีภัยจาก:

- บุคคลแจ้งเหตุ
- ระบบแจ้งเตือนอัคคีภัย
- อุปกรณ์ตรวจจับ เช่น:
  - **Smoke Detector** — อุปกรณ์ตรวจจับควัน
  - **Heat Detector** — อุปกรณ์ตรวจจับความร้อน

เมื่อ SOC ได้รับแจ้งเหตุอัคคีภัยจากบุคคลหรือระบบ ให้ SOC เป็นผู้ประกาศ Code 1

## 3. Goal

**VERIFY** — ตรวจสอบและพิสูจน์ว่าเหตุที่ได้รับแจ้งเกิดขึ้นจริงหรือไม่

## 4. Authority

**SOC (Security Operation Center)** เป็นผู้มีอำนาจประกาศ Code 1 และเป็นผู้มีอำนาจยกเลิก Code 1 เมื่อผลการตรวจสอบยืนยันว่าไม่พบเหตุไฟไหม้หรือกลุ่มควัน

SOC เป็นผู้มีอำนาจประกาศ **Code 2** เมื่อมีหลักฐานยืนยันว่าเกิดเหตุจริงตามเกณฑ์ในเอกสารนี้

## 5. Case Creation and Event Recording

- **กรณีได้รับแจ้งจากบุคคล:** SOC เปิด Case ทันทีหลังจากได้รับแจ้ง
- **กรณีแจ้งเตือนผ่านอุปกรณ์/ระบบ:** ระบบ **Mozart** สร้าง Case ขึ้นในระบบโดยอัตโนมัติ
- หลังจากมี Case แล้ว SOC มีหน้าที่บันทึกและอัปเดตเหตุการณ์ผ่านระบบ Mozart ตามข้อมูลที่ได้รับแจ้ง หรือข้อมูลที่ SOC Monitor ผ่านระบบ CCTV

## 6. CAT / SLA

Code 1 จัดอยู่ในประเภท **CAT 1**

| Category | SLA |
|---|---:|
| CAT 1 | ภายใน 5 นาที |
| CAT 2 | ภายใน 10 นาที |
| CAT 3 | ภายใน 15 นาที |

สำหรับ **Code 1 / CAT 1** ค่า SLA หมายถึงระยะเวลาที่ SOC ต้อง **Acknowledge Case ในระบบ Mozart ภายใน 5 นาที**

### SLA Start

- กรณีบุคคลแจ้งเหตุ: เริ่มนับเมื่อ **SOC ได้รับแจ้ง**
- กรณีระบบ/อุปกรณ์แจ้งเตือน: เริ่มนับเมื่อ **Case ถูกสร้างขึ้นอัตโนมัติในระบบ Mozart**

### SLA Stop

สิ้นสุดเมื่อ **SOC Acknowledge Case ในระบบ Mozart** โดยระยะเวลาจาก SLA Start ถึง SLA Stop ต้องไม่เกิน 5 นาที

> SLA 5 นาทีนี้เป็น SLA สำหรับการ Acknowledge Case ไม่ใช่ข้อกำหนดว่าต้อง Verify เหตุให้เสร็จภายใน 5 นาที

## 7. Fixed SOC Workflow

ลำดับการดำเนินการของ Code 1 เป็นลำดับตายตัวดังนี้:

1. SOC ได้รับแจ้งเหตุ / Case ถูกสร้าง
2. SOC เปิดหรือ Acknowledge Case ในระบบ Mozart ตามแหล่งที่มาของการแจ้ง
3. SOC ประกาศ Code 1
4. SOC แจ้ง DCC (District Command Centre) เพื่อรับทราบ
5. SOC แจ้ง EOT ให้ Standby
6. SOC ส่ง รปภ. และช่างเข้าตรวจสอบพื้นที่ที่ได้รับแจ้ง
7. SOC ตรวจสอบ / Monitor เหตุผ่าน CCTV
8. SOC บันทึกและอัปเดตเหตุการณ์ผ่านระบบ Mozart ตามข้อมูลที่ได้รับแจ้งและข้อมูลจากการ Monitor CCTV
9. ทีมหน้างานทำการ Verify / พิสูจน์พื้นที่จริง
10. ดำเนินการตามผลการ Verify: ยกระดับเป็น Code 2 เมื่อยืนยันเหตุจริง หรือยกเลิก Code 1 เมื่อไม่พบเหตุ

## 8. DCC Notification

SOC สามารถแจ้ง DCC ผ่าน:

- โทรศัพท์ภายใน **5510**
- กลุ่ม **LINE DCC**

ข้อมูลที่ SOC ต้องรายงาน ได้แก่:

- สถานที่ / พื้นที่ที่ได้รับแจ้ง
- จุด Alarm
- ขั้นตอนการปฏิบัติ ณ ขณะนั้นว่าอยู่ในขั้นตอนใด
- จอ CCTV ที่ SOC กำลัง Monitor จุดที่ได้รับแจ้ง

## 9. EOT Standby

- EOT Standby ที่ **ห้องปฏิบัติงานของทีม EOT**
- ระหว่าง Standby ทีม EOT ต้อง **สวมชุดผจญเพลิง** เพื่อเตรียมความพร้อม หากสถานการณ์ยกระดับจาก Code 1 เป็น Code 2

## 10. Verification and Decision Criteria

SOC ส่ง **รปภ. และช่าง** เข้าตรวจสอบพื้นที่ที่ได้รับแจ้ง และ SOC ตรวจสอบ/Monitor เหตุผ่าน CCTV

### 10.1 Confirmed Incident — Escalate to Code 2

SOC เป็นผู้ประกาศ Code 2 เมื่อยืนยันว่าพบเหตุจริง เช่น:

- พบเหตุไฟไหม้จริง แม้ไฟจะดับไปแล้ว
- พบควัน
- CCTV เห็น/ยืนยันเหตุ
- รปภ. ยืนยันเหตุจากพื้นที่ พร้อมส่งภาพหรือวิดีโอเพื่อแสดงหลักฐาน

เมื่อยืนยันเหตุจริง ให้เข้าสู่กระบวนการ **Code 2**

### 10.2 No Incident Found — Cancel Code 1

หากตรวจสอบแล้วไม่พบเหตุไฟไหม้หรือกลุ่มควัน:

1. SOC สั่งยกเลิก Code 1
2. SOC แจ้ง EOT ให้ยกเลิกการ Standby Code 1
3. SOC แจ้ง DCC เพื่อรับทราบ
4. SOC สอบถามทีมช่างถึงสาเหตุของการแจ้งเตือนผิดพลาด
5. SOC แจ้งสาเหตุของการแจ้งเตือนผิดพลาดให้ EOT และ DCC รับทราบ ไม่ว่าการแจ้งเตือนนั้นจะมาจากระบบหรือบุคคล
6. **FMC หรือ SOC** เลือกสถานะ `False Alarm`
7. **FMC หรือ SOC** ใส่ `Findings / Resolution`
8. **FMC หรือ SOC** ปิด Case

## 11. Decision Flow

```text
Fire Alarm Notification
        │
        ├── Person ──► SOC receives report / creates Case
        │                 │
        │                 └── CAT 1 SLA starts
        │
        └── Device/System ──► Mozart auto-creates Case
                              │
                              └── CAT 1 SLA starts
        │
        ▼
SOC Acknowledge Case in Mozart ≤ 5 minutes
        │
        ▼
Declare CODE 1
        │
        ▼
Notify DCC
        │
        ▼
Notify EOT to Standby
        │
        ▼
Dispatch Security + Technician
        │
        ▼
Check / Monitor CCTV + Record events in Mozart
        │
        ▼
      VERIFY
        │
   ┌────┴────┐
   │         │
Confirmed   No fire / smoke found
   │         │
   ▼         ▼
CODE 2    SOC cancels CODE 1
             │
             ├── EOT cancels Standby
             ├── Notify DCC
             ├── Determine false-alarm cause with technician
             ├── Notify EOT + DCC of cause
             └── FMC or SOC: False Alarm + Findings / Resolution + Close Case
```

## 12. Roles — Current Confirmed Knowledge

### SOC

- รับแจ้งเหตุอัคคีภัยจากบุคคลหรือระบบ
- เปิด Case เมื่อได้รับแจ้งจากบุคคล
- Acknowledge Case ใน Mozart ตาม CAT 1 SLA
- ประกาศและยกเลิก Code 1
- แจ้ง DCC
- แจ้ง EOT ให้ Standby / ยกเลิก Standby
- ส่ง รปภ. และช่างเข้าตรวจสอบพื้นที่
- ตรวจสอบและ Monitor เหตุผ่าน CCTV
- บันทึกและอัปเดตเหตุการณ์ใน Mozart
- ประกาศ Code 2 เมื่อยืนยันเหตุจริง
- สอบถามทีมช่างถึงสาเหตุของการแจ้งเตือนผิดพลาด และแจ้ง EOT/DCC
- สามารถเลือก False Alarm, ใส่ Findings / Resolution และปิด Case

### Mozart

- สร้าง Case โดยอัตโนมัติเมื่อเป็นการแจ้งเตือนผ่านอุปกรณ์/ระบบ
- เป็นระบบที่ SOC ใช้ Acknowledge, บันทึก และอัปเดตเหตุการณ์ของ Case

### DCC

- รับทราบ Code 1 และข้อมูลสถานการณ์จาก SOC
- รับทราบการยกเลิก Code 1 และสาเหตุของการแจ้งเตือนผิดพลาด

### EOT

- Standby ที่ห้องปฏิบัติงานของทีม EOT
- สวมชุดผจญเพลิงระหว่าง Standby เพื่อเตรียมพร้อมสำหรับ Code 2
- ยกเลิก Standby เมื่อ SOC ยกเลิก Code 1

### รปภ. และช่าง

- เข้าตรวจสอบและพิสูจน์พื้นที่ที่ได้รับแจ้ง

### FMC

- สามารถเลือกสถานะ False Alarm, ใส่ Findings / Resolution และปิด Case

## 13. AI Guardrails

- AI ต้องไม่ตีความว่า CAT 1 SLA 5 นาทีหมายถึงต้อง Verify เหตุให้เสร็จภายใน 5 นาที
- AI ต้องใช้ SLA Start/Stop ตามที่กำหนดในเอกสารนี้
- AI ต้องไม่ใช้ข้อมูลเดิมที่ระบุว่า Code 1 ไม่มี SLA หรือใช้หลักการ 8 นาที เนื่องจากข้อมูลดังกล่าวถูกแทนที่ด้วย CAT 1 SLA 5 นาทีแล้ว
- AI ต้องไม่สร้างเกณฑ์การประกาศ Code 2 เพิ่มเติมจากที่ได้รับการยืนยันในเอกสารนี้

## 14. Source Notes

Knowledge ฉบับนี้จัดทำจากข้อมูลที่ KB Owner ให้โดยตรง รวมกับเอกสาร Code 1 และ Fire Alarm Activation Flow ที่ KB Owner ให้เป็นแหล่งข้อมูลประกอบ โดยใช้ **DCC — District Command Centre** ตาม Canonical Terminology

## 15. Change Log

| Version | Change | Approved By |
|---|---|---|
| 0.1 | Initial Code 1 knowledge draft; added fire-alarm trigger sources and Smoke/Heat Detector definitions | KB Owner |
| 0.2 | Confirmed SOC authority to declare Code 1; DCC acknowledgement; EOT Standby; Security and Technician dispatched to verify reported area | KB Owner |
| 0.3 | Added fixed SOC workflow; Case creation rules for person/device alerts; Mozart automatic Case creation and SOC event recording/monitoring workflow | KB Owner |
| 0.4 | Added CAT/SLA rules, DCC communication, EOT readiness, Code 2 escalation criteria, Code 1 cancellation, False Alarm and Case closure workflow | KB Owner |
