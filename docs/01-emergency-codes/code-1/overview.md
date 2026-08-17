---
document_id: SEC-CODE-1-001
title: Code 1 — Fire Alarm Notification and Verification
version: 0.1
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

เมื่อระบบหรืออุปกรณ์มีการ Activation ให้เข้าสู่กระบวนการตรวจสอบตาม Code 1

## 3. Goal

**VERIFY** — ตรวจสอบและพิสูจน์ว่าเหตุที่ได้รับแจ้งเกิดขึ้นจริงหรือไม่

## 4. Current Known Actions

ข้อมูลที่ได้รับในปัจจุบันระบุการดำเนินการหลักดังนี้:

1. รับการแจ้งเตือนอัคคีภัยจากบุคคล ระบบ หรืออุปกรณ์
2. ตรวจสอบเหตุทันที
3. SOC ตรวจสอบผ่าน CCTV
4. ส่งเจ้าหน้าที่/ทีมเข้าพิสูจน์พื้นที่จริง
5. ประสาน EOT ให้ Standby
6. รายงาน DCC (District Command Centre)
7. หากพบหรือมีเจ้าหน้าที่หน้างานยืนยันเหตุเพลิงไหม้ ให้เข้าสู่กระบวนการ Code 2

## 5. Known Decision Flow

```text
Fire Alarm Notification
        │
        ├── Person
        ├── System
        └── Detection Device
              ├── Smoke Detector
              └── Heat Detector
        │
        ▼
      CODE 1
        │
        ▼
      VERIFY
        │
        ├── SOC checks CCTV
        ├── Dispatch team to verify area
        ├── EOT Standby
        └── Report DCC
        │
        ▼
Confirmed fire / on-site confirmation
        │
        ▼
      CODE 2
```

## 6. Knowledge Gaps

ข้อมูลต่อไปนี้ยังไม่มีรายละเอียดที่ได้รับการยืนยันเพียงพอ จึงไม่กำหนดเป็น SOP ในเอกสารฉบับนี้:

- ผู้มีอำนาจประกาศ/เปิด Code 1
- ลำดับงานโดยละเอียดของ SOC
- ระยะเวลาที่กำหนดสำหรับการ Verify
- ผู้มีหน้าที่ส่งทีมเข้าพื้นที่โดยเฉพาะ
- จุด Standby และช่องทางการประสาน EOT
- รูปแบบการรายงาน DCC
- ขั้นตอนเมื่อพิสูจน์แล้วไม่พบเหตุ
- เกณฑ์การยกระดับ Code 1 ไป Code 2 ที่ละเอียดกว่าการยืนยันเหตุเพลิงไหม้

AI ต้องไม่เติมรายละเอียดในหัวข้อเหล่านี้จากการคาดเดา

## 7. Source Notes

Knowledge ฉบับนี้จัดทำจากข้อมูลที่ KB Owner ให้โดยตรง รวมกับเอกสาร Code 1 และ Fire Alarm Activation Flow ที่ KB Owner ให้เป็นแหล่งข้อมูลประกอบ โดยมีการแก้คำอ้างอิงศูนย์บัญชาการเป็น **DCC — District Command Centre** ตามคำยืนยันของ KB Owner

## 8. Change Log

| Version | Change | Approved By |
|---|---|---|
| 0.1 | Initial Code 1 knowledge draft; added fire-alarm trigger sources and Smoke/Heat Detector definitions | KB Owner |
