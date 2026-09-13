# Fire Pump & Generator — External Standards Reference

**Document ID:** SEC-SYSTEM-TESTING-EXT-001  
**Version:** 1.0  
**Status:** Approved External Reference  
**Owner:** KB Owner  
**Effective Date:** 2026-09-13  

---

## 1. Scope and Source Classification

ข้อมูลชุดนี้ได้รับอนุมัติจาก KB Owner เพื่อใช้เป็น **External Standards Reference** สำหรับเติมบริบททางเทคนิคของ Fire Pump และ Generator.

**สำคัญ:** ข้อมูลนี้เป็นผลจากการค้นคว้ามาตรฐานภายนอกที่อ้างถึง NFPA 20, NFPA 25, NFPA 110 และมาตรฐาน วสท. ที่เกี่ยวข้อง ไม่ใช่ข้อกำหนดที่ยืนยันว่าปรากฏอยู่ใน One Bangkok SOP `OB-SOP-LW-0003`.

ดังนั้นห้ามใช้เอกสารนี้เพื่อกล่าวว่า One Bangkok กำหนดค่าหรือความถี่เหล่านี้ เว้นแต่มี Approved/Active internal source ยืนยันเพิ่มเติม.

---

## 2. Fire Pump — External Technical Reference

### No-Flow / Churn Test
- Diesel engine: source summary states test **weekly**, run at least **30 minutes**.
- Electric motor: source summary states test **monthly**, run at least **10 minutes**.
- Purpose described by source: verify pressure and automatic starting.

### Annual Flow Test
Source summary states testing at three flow points:
- **0% — Shutoff**
- **100% — Rated**
- **150% — Peak**

Source summary states net pressure at each test point must not be lower than **95%** of the manufacturer's original performance curve, expressed as allowing no more than 5% deterioration.

### Pressure Rating Criteria
Source summary states:
- At **150% flow**, pressure must not fall below **65%** of rated pressure.
- At **0% flow / Churn**, total pressure must not exceed **140%** of rated pressure.

---

## 3. Generator — External Technical Reference

### Weekly Inspection
Source summary lists checks for:
- Fuel level
- Engine oil
- Coolant
- Battery
- Exhaust system

### Monthly Load Test
Source summary states:
- At least **once per month**.
- Run under actual/load condition for at least **30 minutes**.
- Load at least **30% of rated kW**, or achieve exhaust temperature according to manufacturer specification as described in the source summary.

### Type 10 Transfer Time
Source summary states that for critical/high-rise applications described in the source, generator and ATS should be capable of starting and supplying power within **10 seconds**.

### Annual Load Bank
Source summary states that if the monthly test cannot achieve **30% building load**, an annual Load Bank test is required for **1.5 hours**.

---

## 4. Relationship to Internal One Bangkok Reference

Internal Approved Reference `statutory-equipment-testing-reference.md` records that:
- Generator information is not provided in the approved OB-SOP-LW-0003 source summary.
- Fire Pump numerical Flow/Pressure Pass/Fail values are not provided in that SOP summary.

This External Reference provides technical research context only. It **does not convert those internal SOP gaps into confirmed One Bangkok requirements**.

---

## 5. AI Guardrails

- Always identify this material as **External Standards Reference** when answering a One Bangkok/Skills Hunter question from these values.
- Do not present NFPA-derived values here as an internal One Bangkok SOP requirement.
- Do not state that One Bangkok adopts NFPA 110 requirements unless an Approved internal source explicitly establishes that adoption.
- Do not infer that Type 10 applies to every One Bangkok building or generator.
- Do not merge external Generator frequencies or Fire Pump numerical acceptance criteria into OB-SOP-LW-0003 without separate internal evidence and KB Owner approval.
- If an internal Approved/Active source conflicts with this external reference, prioritize the internal Approved/Active source for One Bangkok operational answers and flag the conflict.
- Exact current legal/standards compliance should be separately verified against authoritative/current standards when required.

---

## 6. Source Notes

KB Owner supplied and approved `ข้อมูลมาตรฐานสากลการทดสอบอุปกรณ์.md` on 2026-09-13. The supplied research summary cites NFPA 20, NFPA 25, NFPA 110 and related standards, and includes links to third-party technical guides/research material.

---

## 7. Change Log

- **v1.0 — 2026-09-13** — Initial Approved External Reference for Fire Pump and Generator testing criteria.