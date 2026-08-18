---
document_id: SEC-CODE-1-001
title: Code 1 — Fire Alarm Notification and Verification
version: 0.2
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

## 5. Current Known Actions

ข้อมูลที่ได้รับในปัจจุบันระบุการดำเนินการหลักดังนี้:

1. SOC รับการแจ้งเตือนอัคคีภัยจากบุคคล ระบบ หรืออุปกรณ์
2. SOC ประกาศ Code 1
3. SOC แจ้ง DCC (District Command Centre) เพื่อรับทราบ
4. SOC แจ้ง EOT ให้ Standby
5. ระหว่างที่ EOT Standby ให้ส่ง **รปภ. และช่าง** เข้าตรวจสอบพื้นที่ที่ได้รับแจ้ง
6. SOC ตรวจสอบเหตุผ่าน CCTV
7. ทีมหน้างานทำการ Verify / พิสูจน์พื้นที่จริง
8. หากพบหรือมีเจ้าหน้าที่หน้างานยืนยันเหตุเพลิงไหม้ ให้เข้าสู่กระบวนการ Code 2

## 6. Known Decision Flow

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
       SOC
        │
        ▼
  Declare CODE 1
        │
        ├── Notify DCC for acknowledgement
        ├── Notify EOT to Standby
        ├── Check CCTV
        └── Dispatch Security + Technician
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

## 7. Roles — Current Confirmed Knowledge

### SOC

- รับแจ้งเหตุอัคคีภัยจากบุคคลหรือระบบ
- เป็นผู้ประกาศ Code 1
- แจ้ง DCC เพื่อรับทราบ
- แจ้ง EOT ให้ Standby
- ประสานการส่ง รปภ. และช่างเข้าตรวจสอบพื้นที่
- ตรวจสอบเหตุผ่าน CCTV

### DCC

- รับทราบการประกาศ Code 1 จาก SOC

### EOT

- Standby ระหว่างที่ทีมหน้างานเข้าตรวจสอบพื้นที่

### รปภ. และช่าง

- เข้าตรวจสอบและพิสูจน์พื้นที่ที่ได้รับแจ้ง

## 8. Knowledge Gaps

ข้อมูลต่อไปนี้ยังไม่มีรายละเอียดที่ได้รับการยืนยันเพียงพอ จึงไม่กำหนดเป็น SOP ในเอกสารฉบับนี้:

- ลำดับงานย่อยโดยละเอียดของ SOC หลังประกาศ Code 1
- ระยะเวลาที่กำหนดสำหรับการ Verify
- จุด Standby และรายละเอียดการปฏิบัติของ EOT ระหว่าง Standby
- ช่องทาง/รูปแบบการแจ้ง DCC
- ขั้นตอนเมื่อพิสูจน์แล้วไม่พบเหตุ
- เกณฑ์และผู้มีอำนาจยกระดับ Code 1 ไป Code 2 ที่ละเอียดกว่าการยืนยันเหตุเพลิงไหม้
- ขั้นตอนการปิด Code 1 / ปิด Case

AI ต้องไม่เติมรายละเอียดในหัวข้อเหล่านี้จากการคาดเดา

## 9. Source Notes

Knowledge ฉบับนี้จัดทำจากข้อมูลที่ KB Owner ให้โดยตรง รวมกับเอกสาร Code 1 และ Fire Alarm Activation Flow ที่ KB Owner ให้เป็นแหล่งข้อมูลประกอบ โดยมีการแก้คำอ้างอิงศูนย์บัญชาการเป็น **DCC — District Command Centre** ตามคำยืนยันของ KB Owner

## 10. Change Log

| Version | Change | Approved By |
|---|---|---|
| 0.1 | Initial Code 1 knowledge draft; added fire-alarm trigger sources and Smoke/Heat Detector definitions | KB Owner |
| 0.2 | Confirmed SOC authority to declare Code 1; DCC acknowledgement; EOT Standby; Security and Technician dispatched to verify reported area | KB Owner |
