---
title: ONE89 Wireless 2026 Fire Evacuation Drill
version: 0.1
status: Reference / Drill Scenario
building_type: Residential
building: ONE89 Wireless
drill_date: 2026-09-18
knowledge_scope: Residential Emergency Procedure Development Reference
---

# ONE89 Wireless 2026 Fire Evacuation Drill

> **Knowledge Classification:** Residential / Drill-Specific Reference
>
> เอกสารนี้จัดเก็บเป็นข้อมูลอ้างอิงสำหรับการพัฒนา **Residential Emergency Procedure** ในอนาคต ไม่ใช่ Core SOP และไม่ควรนำรายละเอียดเฉพาะการซ้อมไปใช้กับอาคารทุกประเภทโดยอัตโนมัติ

## 1. Purpose

จัดเก็บ Scenario และข้อมูลจากการประชุมเตรียมการซ้อม **Annual Fire Evacuation Drill 2026 at ONE89 Wireless** เพื่อใช้เป็นกรณีศึกษาและ Knowledge Reference สำหรับอาคารประเภท Residential

การซ้อมจริงกำหนดวันที่ **18 กันยายน 2569** โดยคาดการณ์เริ่ม Drill เวลา **15:00 น.**

## 2. Scenario Location

- Building: ONE89 Wireless
- Floor: ชั้น 25
- Area: Common Area / Corridor
- Simulated Event: Smoke / Fire Detection
- Evacuation Drill Flow: Code 1 → Code 2 → Code 3 → Assembly Point → All Clear

## 3. Participating / Related Teams

จากข้อมูลการประชุม มีหน่วยงานหรือทีมที่เกี่ยวข้อง ได้แก่:

- ONE89 Wireless
- Ritz-Carlton
- SOC
- EOT
- Safety
- DCC
- FCC / FMC
- Security
- Building Management
- Ritz-Carlton Emergency Team
- Fire and Rescue / Bon Kai Fire Station

## 4. Fire Alarm / Notification Concept

Scenario จำลองให้ Smoke Detection ตรวจจับควันในพื้นที่ ONE89 Wireless ชั้น 25 และส่งสัญญาณไปยัง FCC ของ ONE89 Wireless

มีฟังก์ชันเพิ่มเติมที่คาดว่าจะส่ง Notice ไปยัง FCC ของ Ritz-Carlton เพื่อรับทราบเหตุด้วย

### Recheck Required

ต้องตรวจสอบกับ FMC ก่อนวันซ้อมว่า:

- Fire Protection System ของ ONE89 Wireless และ Ritz-Carlton เชื่อมโยงกันอย่างไร
- Alarm / Notice ส่งไปยังทั้งสองอาคารหรือส่วนกลางจริงหรือไม่
- ลำดับการแจ้งเตือนที่เกิดขึ้นจริงจากระบบเป็นอย่างไร

ห้ามถือรายละเอียดส่วนนี้เป็น Confirmed System Function จนกว่าจะ Recheck แล้ว

## 5. Code 1 — Standby Phase

เมื่อเกิดสัญญาณ Code 1:

- EOT Standby
- Ritz-Carlton Emergency Team Standby
- ทีมที่เกี่ยวข้องเตรียมพร้อมตามแผนฉุกเฉิน
- ต้องตรวจสอบว่าทุกทีมที่เกี่ยวข้องเข้า Emergency Channel ครบถ้วน

### Recheck Required

ตรวจสอบ POC / Emergency Channel และรายชื่อทีมที่ต้องอยู่ในช่องก่อนวันซ้อมจริง

## 6. Code 2 — Joint Emergency Response

เมื่อยืนยัน Code 2:

- EOT และ Ritz-Carlton Emergency Team รายงานตัวต่อผู้บัญชาการเหตุฉุกเฉินของ ONE89 Wireless
- เตรียมจัดตั้งกองอำนวยการเหตุฉุกเฉินบริเวณหน้าอาคาร
- Response Teams เข้าพื้นที่โดยมีผู้นำทาง
- ใช้ Fireman Lift จากชั้น G บริเวณ Lobby เพื่อขึ้นไปชั้น 25 ตาม Scenario
- EOT และ Ritz-Carlton Emergency Team เข้าพื้นที่ร่วมกัน
- การ Command การเข้าระงับเหตุร่วมกันให้ยึด EOT เป็นทีมหลักตามข้อมูลการประชุม

### Coordination Risk

เนื่องจากมี Response Team มากกว่าหนึ่งทีมเข้าพื้นที่พร้อมกัน ต้องให้ความสำคัญกับ:

- Command Structure
- Radio Communication
- Team Identification
- Entry Coordination
- Task Assignment

เพื่อป้องกันคำสั่งซ้ำซ้อนหรือการประสานงานคลาดเคลื่อน

## 7. Code 3 / Evacuation

หลังจาก Code 2 Scenario จะดำเนินเข้าสู่ Code 3 และการอพยพตามแผน

การกดสัญญาณอพยพเป็นการดำเนินการของ ONE89 Wireless ตามลำดับการสื่อสารและการประสานงานของ SOC สำหรับ Drill นี้

Scenario มีการจำลองผู้สูญหายจำนวน **2 คน** เพื่อทดสอบการค้นหา การรายงานสถานะ และการช่วยเหลือผู้บาดเจ็บ/ผู้สูญหาย

## 8. General Alarm / System Timing

ข้อมูลการประชุมระบุลำดับการแจ้งเตือนของ ONE89 Wireless เป็น:

```text
5 → 3 → 2
```

คาดการณ์เริ่มทดสอบ Drill เวลา 15:00 น. และมีแผนให้สัญญาณดังประมาณ 5–7 นาทีเพื่อทดสอบระบบ

ข้อมูล 5-3-2 ในเอกสารนี้เป็นข้อมูลสำหรับ Scenario/Building Context ของ ONE89 Wireless และต้องไม่ถูกตีความแทน Core SOP โดยอัตโนมัติ

## 9. Emergency Vehicles / Drill Arrangement

EOT Support Vehicles:

- รถกอล์ฟ 1 คัน
- รถกระบะ 1 คัน

Bon Kai Fire Station:

- รถน้ำ 1 คัน

สำหรับ **การซ้อมครั้งนี้** รถดับเพลิงบ่อนไก่กำหนดให้จอดบริเวณ **Park Lane** แทนตำแหน่งหน้าอาคาร เพื่อลดผลกระทบด้านทัศนียภาพในวันซ้อม

> **Guardrail:** ตำแหน่ง Park Lane เป็น **Drill Arrangement** เท่านั้น ไม่ใช่ข้อกำหนดตำแหน่งรถดับเพลิงสำหรับเหตุจริง

## 10. Residential-Specific Roles Observed

Scenario นี้มีบทบาทที่ควรศึกษาเพิ่มเติมสำหรับการพัฒนา Residential Emergency Procedure เช่น:

- RM — Residential Manager
- OM — Operation Manager
- Concierge
- Floor Warden
- Building Management

บทบาทและ Authority เหล่านี้ต้องได้รับการวิเคราะห์และยืนยันเพิ่มเติมก่อนนำไปกำหนดเป็น Residential SOP มาตรฐาน

## 11. Assembly Point / Missing Persons Scenario

Scenario ประกอบด้วย:

- Floor Warden รายงานจำนวนผู้อพยพ
- จำลองผู้สูญหาย 2 ราย โดยพบครั้งสุดท้ายบริเวณชั้น 25
- ข้อมูลผู้สูญหายถูกส่งต่อไปยังทีมที่เกี่ยวข้อง
- จำลองการค้นพบผู้สูญหายทั้ง 2 ราย
- จำลองผู้บาดเจ็บ 1 ราย และผู้ไม่มีอาการบาดเจ็บ 1 ราย

ข้อมูลส่วนนี้สามารถใช้เป็น Reference สำหรับพัฒนา Residential Accountability / Search & Rescue Workflow ในอนาคต

## 12. Recovery / All Clear Scenario

Scenario หลังควบคุมเหตุประกอบด้วย:

- รายงานว่าสามารถควบคุมเพลิงได้
- ตรวจสอบความปลอดภัยและความเสียหายในพื้นที่
- กั้นพื้นที่ตามความจำเป็น
- ทีมที่เกี่ยวข้องรายงานเหตุการณ์และความเสียหาย
- เคลียร์พื้นที่
- Reset ระบบ
- แจ้งอาคารพร้อมกลับมาเปิดบริการตามปกติ
- แจ้ง IMT
- ยกเลิกสถานการณ์ฉุกเฉินและปิดการซ้อม

รายละเอียด Authority และ All Clear ต้องเทียบกับ Core KB ที่ได้รับอนุมัติแล้วก่อนนำไปใช้เป็น SOP จริง

## 13. Knowledge Gaps / Recheck Before Drill

1. ยืนยัน Fire Protection System linkage ระหว่าง ONE89 Wireless และ Ritz-Carlton
2. ยืนยัน Alarm / Notice routing ระหว่าง FCC ของทั้งสองอาคาร
3. ยืนยัน Incident Commander / Authority สำหรับวันซ้อมจริง
4. ยืนยัน Emergency Channel และรายชื่อหน่วยงานที่ต้องเข้า Channel
5. ยืนยัน Command Structure ระหว่าง EOT และ Ritz-Carlton Emergency Team
6. ยืนยัน Fireman Lift function และขั้นตอนการใช้งานใน Drill
7. ยืนยัน Evacuation Signal activation sequence
8. ยืนยันรายละเอียด System Timing 5-3-2 ของ ONE89 Wireless
9. ซักซ้อม Internal Communication ก่อนวัน Drill จริง

## 14. Knowledge Guardrails

AI ต้องแยกข้อมูลชุดนี้ออกเป็นสามระดับ:

```text
Core Emergency Knowledge
        │
        ├── Residential-Specific Knowledge
        │
        └── ONE89 Wireless 2026 Drill-Specific Scenario
```

- ห้ามนำ Drill Arrangement ไปกำหนดเป็น SOP จริงโดยอัตโนมัติ
- ห้ามนำ Residential-specific role ไปใช้กับ Retail หรืออาคารประเภทอื่นโดยไม่มี Knowledge รองรับ
- จุดที่ระบุ Recheck Required ต้องถือเป็น Unconfirmed Knowledge จนกว่าจะได้รับข้อมูลยืนยัน
- หากข้อมูล Scenario ขัดกับ Core KB ให้แสดง Conflict และขอการยืนยันจาก KB Owner ห้ามแก้ Core KB เอง
- การพัฒนา Residential Emergency Procedure จากเอกสารนี้ต้องผ่าน Proposal → KB Owner Review → Approval ก่อนเปลี่ยนเป็น SOP

## 15. Development Direction

เอกสารนี้สามารถใช้เป็นฐานสำหรับพัฒนา Knowledge ในอนาคต เช่น:

**Residential Emergency Procedure**

โดยศึกษาเพิ่มเติมเรื่อง:

- Residential Command Structure
- Fire Alarm / Notification
- Code 1 / Code 2 / Code 3 adaptation
- Residential Evacuation
- Floor Warden
- Resident Accountability
- Search & Rescue
- Assembly Point
- Multi-Building / Multi-Team Coordination
- Recovery / All Clear

## 16. Change Log

| Version | Status | Change |
|---|---|---|
| 0.1 | Reference / Drill Scenario | Initial ONE89 Wireless 2026 Fire Evacuation Drill reference for future Residential Emergency Procedure development |
