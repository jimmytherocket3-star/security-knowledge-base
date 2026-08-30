---
document_id: SEC-CODE-3-001
title: Code 3 — General Alarm and Evacuation
version: 0.2
status: Draft
owner: KB Owner
primary_ai_operator: ChatGPT
---

# Code 3 — General Alarm and Evacuation

## 1. Goal and Definition

**Code 3 = Evacuation / การอพยพ**

เป้าหมายหลักของ Code 3 คือ **Life Safety — ความปลอดภัยในชีวิต** โดยผู้ใช้อาคารเข้าสู่กระบวนการอพยพไปยัง **Assembly Point** ตามสถานการณ์และคำสั่งที่เกี่ยวข้อง

## 2. Approved Code 3 Triggers

Code 3 สามารถเริ่มได้จาก 2 เส้นทางหลัก และ **ไม่จำเป็นต้องรอให้ EOT หรือ สดพ.บ่อนไก่ไม่สามารถควบคุมเพลิงได้ก่อน**

### 2.1 System Trigger — General Alarm

ระบบเข้าสู่สถานะ **General Alarm** ตาม System Escalation Timeline

### 2.2 Command Trigger

ผู้มีอำนาจสามารถประเมินสถานการณ์และตัดสินใจเข้าสู่ Code 3 / Evacuation ได้ทันที โดยไม่จำเป็นต้องรอให้การระงับเหตุล้มเหลว

ผู้มีอำนาจที่ได้รับการยืนยันใน Knowledge ชุดนี้อยู่ภายใต้โครงสร้าง IMT ได้แก่ Incident Commander, Building Manager, DCC และสำหรับพื้นที่ Retail คือ DM Retail ตามพื้นที่รับผิดชอบ

Code 3 ไม่จำเป็นต้องดำเนินตาม Code 1 → Code 2 → Code 3 ตามลำดับทุกเหตุ หากมี System Trigger หรือ Command Trigger ที่ถูกต้องสามารถเข้าสู่ Code 3 ได้

## 3. IMT and Evacuation Authority

**IMT = Incident Management Team**

ในขอบเขต Knowledge ที่ได้รับการยืนยัน IMT ประกอบด้วยผู้มีบทบาทในการบริหารและตัดสินใจเหตุฉุกเฉิน ได้แก่:

- Incident Commander
- Building Manager
- DCC
- พื้นที่ Retail: DM Retail

การตัดสินใจเข้าสู่ Code 3 ไม่ได้มีเงื่อนไขบังคับว่าต้องรอให้ EOT หรือสถานีดับเพลิงควบคุมเหตุไม่ได้ก่อน

## 4. General Alarm

**General Alarm** คือสัญญาณเตือนภัยขั้นสุดท้ายทั่วทั้งอาคาร ซึ่งทำงานโดยอัตโนมัติหากระบบตรวจจับพบเหตุเพลิงไหม้แล้วไม่มีการกดหน่วงเวลาหรือตอบสนองใด ๆ (Action) จากผู้ควบคุมตู้ FACP หรือผู้ Monitor โปรแกรม

### 4.1 System Escalation Timeline

- Step 1 = Code 1
- Step 2 = Code 2
- Step 3 = Code 3

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

รวมเวลาตั้งแต่ระบบเริ่มตรวจจับจนถึง General Alarm = **10 นาที** ในกรณีไม่มีการกดหน่วงเวลาหรือ Action จากผู้ควบคุม FACP หรือผู้ Monitor โปรแกรม

> System Escalation Timeline 5+3+2 นาทีเป็นคนละกลไกกับ Code 1 CAT 1 SLA 5 นาทีสำหรับ SOC Acknowledge Case ใน Mozart และห้ามตีความปะปนกัน

## 5. Automatic Building-System Actions at General Alarm

เมื่อระบบเข้าสู่ General Alarm ระบบอาคารทำงานโดยอัตโนมัติตาม Knowledge ที่ได้รับการยืนยัน:

- **PA Override / Strobe** — Alarm และเสียงประกาศทำงานทั่วทั้งอาคาร และ Strobe Light ทำงาน
- **AHU** — OFF All Zone
- **Door Unlock** — Magnetic Door, Access Control, Fire Exit และ Turnstile ปลดล็อก/เปิดตามฟังก์ชัน General Alarm
- **Elevator** — ลง Standby ชั้น G
- **Emergency Lighting** — เปิดระบบไฟฉุกเฉินและไฟเส้นทางหนีไฟ
- ผู้ใช้อาคารเข้าสู่กระบวนการ Evacuation ไปยัง Assembly Point

## 6. SOC Responsibilities and Emergency Communication

SOC ยังคงทำหน้าที่ Monitor, Coordinate, Communicate และ Update Case ในระหว่าง Code 3

### 6.1 Emergency Radio

- **Primary Channel: EMER_1**
- **Backup Channel: EMER_2** — ใช้เมื่อ EMER_1 เกิดปัญหา

EMER_2 ไม่ใช่ช่องที่เลือกใช้ทั่วไปใน Code 3 แต่เป็นช่องสำรองเมื่อ EMER_1 มีปัญหา

SOC ประสานข้อมูลกับหน่วยงานที่เกี่ยวข้อง เช่น EOT, DCC, BMO/ฝ่ายบริหารอาคาร, Engineering และหน่วยงานตอบโต้เหตุที่เกี่ยวข้อง

คำว่า **DEC** ที่ปรากฏในข้อมูลร่างก่อนหน้าเป็นคำที่ไม่ถูกต้องสำหรับ Workflow นี้ ให้ใช้ **DCC**

## 7. Security Responsibilities

เจ้าหน้าที่ รปภ. สนับสนุนการอพยพ ได้แก่ การนำผู้ใช้อาคารออกจากพื้นที่ การควบคุมทางเข้า-ออก การป้องกันการย้อนกลับเข้าอาคาร การตรวจสอบพื้นที่/ชั้น การช่วยเหลือผู้ที่ต้องการความช่วยเหลือ และการดูแลเส้นทางไปยัง Assembly Point ตามหน้าที่

### 7.1 PCS

**รปภ. PCS รับผิดชอบภายในอาคาร รวมถึงพื้นที่ Retail**

### 7.2 G4S

**รปภ. G4S รับผิดชอบภายนอกอาคาร** โดยมีหน้าที่:

- ดูแลการอพยพภายนอกอาคาร
- สนับสนุนการจัดการจราจร
- แนะนำเส้นทางให้ลูกค้าและผู้เช่าไปยัง Assembly Point อย่างถูกต้อง

PCS และ G4S เป็นชื่อบริษัทต้นสังกัดของ รปภ. ไม่ใช่ชื่อ Emergency Response Team

## 8. Assembly Point and Accountability

BMO รับผิดชอบจัดตั้งกองอำนวยการเหตุฉุกเฉินที่ Assembly Point

สำหรับพื้นที่อาคาร Building Manager เป็นผู้ควบคุมหลัก โดยมี Engineering/FMC สนับสนุนข้อมูลด้านเทคนิค โครงสร้างอาคาร และระบบวิศวกรรม

### 8.1 Evacuee Accountability

BMO รับผิดชอบหลักในการจัดตั้งระบบตรวจสอบจำนวนผู้อพยพและข้อมูลผู้ติดค้าง โดย EOT สนับสนุนด้านการอพยพ ผู้บาดเจ็บ และข้อมูลผู้ติดค้าง

เมื่อพบ Missing Person หรือผู้ติดค้าง ข้อมูลจะถูกส่งเข้าสู่กระบวนการบริหารเหตุผ่าน SOC / DCC / IMT

## 9. EOT Roles

| Team | Role |
|---|---|
| **Echo (E)** | เข้าเผชิญเหตุ Code 2 |
| **Oscar (O)** | Search & Rescue |
| **Tango (T)** | Medic |

### 9.1 Oscar — Search & Rescue Handover

ก่อน **สดพ.บ่อนไก่** มาถึง ทีม Oscar สามารถเข้า Search & Rescue ได้ หากสถานการณ์ยังอยู่ในระดับที่ควบคุมได้

เมื่อ **สดพ.บ่อนไก่ (สถานีดับเพลิงบ่อนไก่)** มาถึงพื้นที่เกิดเหตุและเตรียมพร้อมเริ่มปฏิบัติงานในพื้นที่เกิดเหตุแล้ว EOT ต้องส่งต่อภารกิจ Search & Rescue ในพื้นที่เกิดเหตุให้ สดพ.บ่อนไก่เป็นผู้ดำเนินการ

การเข้าสู่ Code 3 โดยตัวมันเองไม่ใช่เหตุให้ Oscar ต้องหยุด Search & Rescue ทันที

## 10. SOC BCP Activation and Operational Continuity

BCP เป็น Business Continuity ของ SOC และไม่ได้จำกัดเฉพาะ Code 3

SOC สามารถย้ายไป BCP เมื่อเกิด Code 2 หรือเหตุฉุกเฉินอื่นที่ส่งผลต่อความปลอดภัยหรือความสามารถในการใช้งานของศูนย์ SOC เช่น อาคาร One Power ถูกโจมตี

> Code 2 ไม่ได้หมายความว่า SOC ต้องย้าย BCP ทุกเหตุโดยอัตโนมัติ การย้าย BCP ต้องสัมพันธ์กับความจำเป็นในการออกจากหรือไม่สามารถใช้ศูนย์ปฏิบัติการหลักได้

### 10.1 BCP Location

**BCP Room อยู่ที่ชั้น B1 ใกล้ Load 1 ใต้อาคาร Parade / The Storeys**

### 10.2 BCP Transition

เมื่อ SOC ต้องอพยพจากศูนย์ปฏิบัติการ:

1. SOC นำกระเป๋าฉุกเฉินที่มีอุปกรณ์ IT ไปด้วย
2. เดินทางไปยัง BCP Room
3. เชื่อมต่ออุปกรณ์กับคอมพิวเตอร์ที่อยู่ใน BCP Room
4. เชื่อมต่อระบบที่จำเป็น
5. Run CCTV, Mozart, Radio และระบบอื่นที่เกี่ยวข้อง
6. กลับมาปฏิบัติงานด้านการประสานงานและบริหารเหตุให้ต่อเนื่องโดยเร็วที่สุด

## 11. Recovery / All Clear

ก่อนเข้าสู่ Recovery ต้องยืนยันว่าควบคุมสถานการณ์ได้ และตรวจสอบสถานะผู้อพยพ/ผู้ติดค้างตามกระบวนการ

จากนั้นดำเนินการ Joint Safety Assessment เพื่อตรวจสอบความปลอดภัยของพื้นที่ โครงสร้าง ระบบ Safety และระบบ Engineering ที่เกี่ยวข้อง

### 11.1 All Clear Authority

- **พื้นที่ Building — Building Manager** เป็นผู้มีอำนาจสั่ง All Clear
- **พื้นที่ Retail — DM Retail** เป็นผู้มีอำนาจสั่ง All Clear

เมื่อได้รับ All Clear และได้รับการยืนยันว่าปลอดภัย ให้ดำเนินการกลับสู่ Normal State และ Re-entry ตามคำสั่งของผู้มีอำนาจ

## 12. SOC Post-Incident and Case Closure

หลังเหตุการณ์เข้าสู่ Normal State แล้ว SOC ต้อง:

1. รวบรวมข้อมูลสถานการณ์
2. สรุปเหตุการณ์
3. Update รายละเอียด Case
4. บันทึก Resolution
5. Resolve Case ในระบบ Mozart

## 13. AI Guardrails

1. ห้ามตีความว่า Code 3 ต้องรอให้ EOT หรือ สดพ.บ่อนไก่ควบคุมเพลิงไม่ได้ก่อน
2. Code 3 สามารถเกิดจาก General Alarm หรือ Command Trigger ของผู้มี Authority ได้
3. ไม่จำเป็นต้องผ่าน Code 1 → Code 2 → Code 3 ตามลำดับทุกเหตุ
4. System Escalation Timeline 5+3+2 = 10 นาที ห้ามนำไปปะปนกับ Code 1 CAT 1 SLA
5. EMER_1 เป็น Primary Emergency Radio Channel; EMER_2 เป็น Backup เมื่อ EMER_1 มีปัญหา
6. DEC ไม่ใช่ Role ใน Workflow นี้ ให้ใช้ DCC
7. คำย่อที่ถูกต้องคือ สดพ.บ่อนไก่ = สถานีดับเพลิงบ่อนไก่
8. Oscar สามารถ Search & Rescue ก่อน สดพ.บ่อนไก่พร้อมปฏิบัติงานได้ หากสถานการณ์ยังควบคุมได้
9. เมื่อ สดพ.บ่อนไก่พร้อมเริ่มปฏิบัติงานในพื้นที่เกิดเหตุ ให้ส่งต่อ Search & Rescue ในพื้นที่เกิดเหตุ
10. PCS รับผิดชอบภายในอาคารรวมถึง Retail; G4S รับผิดชอบภายนอกอาคาร
11. All Clear Authority: Building = Building Manager; Retail = DM Retail
12. BCP ไม่ใช่กระบวนการเฉพาะ Code 3 และ Code 2 ทุกเหตุไม่ได้ทำให้ SOC ต้องย้าย BCP โดยอัตโนมัติ
13. AI ต้องไม่สร้างรายชื่อบุคคลเฉพาะเป็น IMT Authority หากไม่ได้รับการอนุมัติจาก KB Owner

## 14. Change Log

| Version | Change | Approved By |
|---|---|---|
| 0.1 | Initial approved Code 3 knowledge: two triggers, General Alarm definition, 5+3+2 system escalation timeline, automatic building-system actions and evacuation linkage | KB Owner |
| 0.2 | Expanded approved Code 3: Life Safety goal, IMT/authority, EMER_1/EMER_2, security roles, Assembly Point accountability, EOT roles and Search & Rescue handover, SOC BCP, Recovery/All Clear and Case Closure | KB Owner |
