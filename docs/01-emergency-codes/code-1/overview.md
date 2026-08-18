---
document_id: SEC-CODE-1-001
title: Code 1 — Fire Alarm Notification and Verification
version: 0.3
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

**SOC (Security Operation Center)** เป็นผู้มีอำนาจประกาศ Code 1 เมื่อ SOC ได้รับแจ้งเหตุอัคคีภัยจากบุคคลหรือระบบ

## 5. Case Creation and Event Recording

เมื่อ SOC ได้รับแจ้งเหตุ ให้ดำเนินการด้าน Case ดังนี้:

- **กรณีได้รับแจ้งจากบุคคล:** SOC เปิด Case ทันทีหลังจากได้รับแจ้ง
- **กรณีแจ้งเตือนผ่านอุปกรณ์:** ระบบ **Mozart** สร้าง Case ขึ้นในระบบโดยอัตโนมัติ
- หลังจากมี Case แล้ว SOC มีหน้าที่บันทึกและอัปเดตเหตุการณ์ผ่านระบบ Mozart ตามข้อมูลที่ได้รับแจ้ง หรือข้อมูลที่ SOC Monitor ผ่านระบบ CCTV

## 6. Fixed SOC Workflow

ลำดับการดำเนินการของ Code 1 เป็นลำดับตายตัวดังนี้:

1. SOC ได้รับแจ้งเหตุ / Case ถูกสร้าง
2. SOC ประกาศ Code 1
3. SOC แจ้ง DCC (District Command Centre) เพื่อรับทราบ
4. SOC แจ้ง EOT ให้ Standby
5. SOC ส่ง รปภ. และช่างเข้าตรวจสอบพื้นที่ที่ได้รับแจ้ง
6. SOC ตรวจสอบ / Monitor เหตุผ่าน CCTV
7. SOC บันทึกและอัปเดตเหตุการณ์ผ่านระบบ Mozart ตามข้อมูลที่ได้รับแจ้งและข้อมูลจากการ Monitor CCTV
8. ทีมหน้างานทำการ Verify / พิสูจน์พื้นที่จริง
9. หากพบหรือมีเจ้าหน้าที่หน้างานยืนยันเหตุเพลิงไหม้ ให้เข้าสู่กระบวนการ Code 2

## 7. Known Decision Flow

```text
Fire Alarm Notification
        │
        ├── Person ──► SOC creates Case immediately
        │
        └── Device/System ──► Mozart creates Case automatically
        │
        ▼
       SOC
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
  Check / Monitor CCTV
        │
        ├── SOC records/updates events in Mozart
        │
        ▼
      VERIFY
        │
        ▼
Confirmed fire / on-site confirmation
        │
        ▼
      CODE 2
```

## 8. Roles — Current Confirmed Knowledge

### SOC

- รับแจ้งเหตุอัคคีภัยจากบุคคลหรือระบบ
- เปิด Case ทันทีเมื่อได้รับแจ้งจากบุคคล
- เป็นผู้ประกาศ Code 1
- แจ้ง DCC เพื่อรับทราบ
- แจ้ง EOT ให้ Standby
- ส่ง รปภ. และช่างเข้าตรวจสอบพื้นที่
- ตรวจสอบและ Monitor เหตุผ่าน CCTV
- บันทึกและอัปเดตเหตุการณ์ในระบบ Mozart ตามข้อมูลที่ได้รับแจ้งหรือข้อมูลจากการ Monitor CCTV

### Mozart

- สร้าง Case โดยอัตโนมัติเมื่อเป็นการแจ้งเตือนผ่านอุปกรณ์
- เป็นระบบที่ SOC ใช้บันทึกและอัปเดตเหตุการณ์ของ Case

### DCC

- รับทราบการประกาศ Code 1 จาก SOC

### EOT

- Standby ระหว่างที่ทีมหน้างานเข้าตรวจสอบพื้นที่

### รปภ. และช่าง

- เข้าตรวจสอบและพิสูจน์พื้นที่ที่ได้รับแจ้ง

## 9. Knowledge Gaps

ข้อมูลต่อไปนี้ยังไม่มีรายละเอียดที่ได้รับการยืนยันเพียงพอ จึงไม่กำหนดเป็น SOP ในเอกสารฉบับนี้:

- ระยะเวลาที่กำหนดสำหรับการ Verify
- จุด Standby และรายละเอียดการปฏิบัติของ EOT ระหว่าง Standby
- ช่องทาง/รูปแบบการแจ้ง DCC
- ขั้นตอนเมื่อพิสูจน์แล้วไม่พบเหตุ
- เกณฑ์และผู้มีอำนาจยกระดับ Code 1 ไป Code 2 ที่ละเอียดกว่าการยืนยันเหตุเพลิงไหม้
- ขั้นตอนการปิด Code 1 / ปิด Case

AI ต้องไม่เติมรายละเอียดในหัวข้อเหล่านี้จากการคาดเดา

## 10. Source Notes

Knowledge ฉบับนี้จัดทำจากข้อมูลที่ KB Owner ให้โดยตรง รวมกับเอกสาร Code 1 และ Fire Alarm Activation Flow ที่ KB Owner ให้เป็นแหล่งข้อมูลประกอบ โดยมีการแก้คำอ้างอิงศูนย์บัญชาการเป็น **DCC — District Command Centre** ตามคำยืนยันของ KB Owner

## 11. Change Log

| Version | Change | Approved By |
|---|---|---|
| 0.1 | Initial Code 1 knowledge draft; added fire-alarm trigger sources and Smoke/Heat Detector definitions | KB Owner |
| 0.2 | Confirmed SOC authority to declare Code 1; DCC acknowledgement; EOT Standby; Security and Technician dispatched to verify reported area | KB Owner |
| 0.3 | Added fixed SOC workflow; Case creation rules for person/device alerts; Mozart automatic Case creation and SOC event recording/monitoring workflow | KB Owner |
