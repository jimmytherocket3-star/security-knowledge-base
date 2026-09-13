# Crime & Terrorism Incident Management Reference

**Document ID:** SEC-SYSTEM-CRIME-TERROR-001  
**Title:** แผนบริหารจัดการเหตุการณ์อาชญากรรมและการก่อการร้าย  
**Version:** 1.0  
**Status:** Approved Reference  
**Owner:** KB Owner  
**Effective Date:** 2026-09-13  

---

## 1. Scope

เอกสารนี้บันทึกข้อมูลที่ KB Owner อนุมัติจากไฟล์ `แผนการจัดการเหตุอาชญากรรม,ก่อการร้าย.md` ซึ่งระบุว่าเป็นระเบียบปฏิบัติมาตรฐาน (SOP) ของโครงการ One Bangkok สำหรับแผนบริหารจัดการเหตุการณ์อาชญากรรมและการก่อการร้าย.

ข้อมูลต้นทางที่ได้รับเป็นข้อมูลสรุประดับภาพรวม จึงเก็บเฉพาะสิ่งที่ต้นทางรองรับและไม่สร้างขั้นตอนปฏิบัติเพิ่มเติม.

---

## 2. Approved Knowledge

SOP ครอบคลุมการรับมือเหตุการณ์รุนแรงหลัก 2 กรณี:

1. **การใช้ยานพาหนะเป็นอาวุธพุ่งชนบุคคล**
2. **การใช้อาวุธมีคมทำร้ายร่างกาย**

เนื้อหาครอบคลุมในระดับภาพรวมถึง:

- การกำหนดหน้าที่และความรับผิดชอบของหน่วยงานที่เกี่ยวข้อง เช่น **IMT** และ **DCC**
- แนวทางการป้องกัน การตอบสนอง และการควบคุมสถานการณ์
- เป้าหมายเพื่อลดความสูญเสียต่อชีวิตและทรัพย์สิน
- การกำหนดคำนิยามของพื้นที่เขตอันตราย
- การใช้เทคโนโลยีด้านความปลอดภัย เช่น **CCTV** และ **Video Analytic**
- การสนับสนุนการประสานงานกับเจ้าหน้าที่ตำรวจและหน่วยงานภายนอก

---

## 3. Knowledge Gaps / Source Limitations

Source summary ที่ได้รับยังไม่ให้รายละเอียดเพียงพอสำหรับยืนยัน:

- Trigger / เกณฑ์ประกาศเหตุของแต่ละกรณี
- Declaration Authority / ผู้มีอำนาจประกาศหรือยุติเหตุ
- ขั้นตอนปฏิบัติแบบลำดับ Workflow
- หน้าที่เฉพาะของ IMT, DCC หรือหน่วยงานอื่นในแต่ละขั้น
- ชื่อ/ประเภท/ขอบเขตของพื้นที่เขตอันตราย
- วิธีการแบ่งหรือเปลี่ยนระดับพื้นที่
- Radio Channel / Communication Protocol
- MOZART Event Type, Case workflow, Task หรือ SLA
- CCTV / Video Analytic detection criteria หรือ response workflow
- ขั้นตอน Lockdown, Evacuation, Shelter, Re-entry หรือ All Clear
- ขั้นตอนและ Authority ในการประสาน/ส่งมอบเหตุให้ตำรวจ
- Medical / casualty management workflow
- แบบฟอร์ม รายงาน หรือ Closure Criteria

---

## 4. AI Guardrails

- ห้ามสร้าง Trigger, Authority, Workflow หรือขั้นตอนเชิงยุทธวิธีจากความรู้ทั่วไปแล้วนำเสนอว่าเป็น SOP ของ One Bangkok.
- ห้ามตีความว่าเหตุยานพาหนะพุ่งชนหรืออาวุธมีคมจะเปิดใช้ **Code Sierra**, Emergency Code, Threat Level, Lockdown หรือ Evacuation โดยอัตโนมัติ เว้นแต่ Approved/Active source ระบุความสัมพันธ์นั้นโดยตรง.
- ห้ามใช้ข้อมูลจาก Code Sierra หรือ Threat Response Protocol มาเติมช่องว่างของ SOP นี้โดยอัตโนมัติ.
- IMT และ DCC ให้ใช้ตาม Canonical terminology ที่ Approved/Active แต่ห้ามสร้างอำนาจเฉพาะของ SOP นี้จากนิยามทั่วไป.
- CCTV และ Video Analytic ระบุได้เฉพาะว่าต้นทางกล่าวถึงการใช้เพื่อสนับสนุนการจัดการ/ประสานเหตุ; ห้ามสร้าง detection rule หรือ automation ที่ต้นทางไม่ได้ระบุ.
- หากผู้ใช้ถามรายละเอียดที่ Source ไม่รองรับ ให้ตอบ **Knowledge Gap** และไม่เดา.

---

## 5. Source

KB Owner supplied and approved `แผนการจัดการเหตุอาชญากรรม,ก่อการร้าย.md` on 2026-09-13.

---

## 6. Change Log

- **v1.0 — 2026-09-13** — Initial Approved Reference created from KB Owner-approved source summary.