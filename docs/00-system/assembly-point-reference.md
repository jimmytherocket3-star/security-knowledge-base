---
document_id: SEC-SYS-ASSEMBLY-001
title: One Bangkok Assembly Point Reference
version: 1.0
status: Approved Reference
owner: KB Owner
updated: 2026-09-08
source: User-provided One Bangkok map image approved by KB Owner
---

# One Bangkok Assembly Point Reference

## Purpose

เอกสารนี้บันทึกข้อมูลจุดรวมพล (Assembly Point) ที่มองเห็นได้จากแผนผัง One Bangkok ซึ่ง KB Owner ให้ข้อมูลและอนุมัติเมื่อ 2026-09-08

## Confirmed Assembly Point Information

จากแผนผังพบสัญลักษณ์ **Assembly Point สีเขียวจำนวน 3 บริเวณหลัก**:

1. บริเวณฝั่ง **The Storeys / Wireless Road**
2. บริเวณพื้นที่สีเขียวส่วนกลาง **One Bangkok Park**
3. บริเวณฝั่ง **Parade / Rama IV Road**

## Building-to-Assembly-Point Mapping

**Knowledge Gap:** ภาพต้นฉบับไม่ได้ระบุตารางหรือข้อความที่จับคู่โดยตรงว่าอาคารแต่ละแห่ง เช่น Tower 3, Tower 4, Tower 5, Parade, The Storeys, Forum หรืออาคารอื่น ต้องไปยัง Assembly Point ใดโดยเฉพาะ

ดังนั้น AI ต้องไม่อนุมาน Building → Assembly Point จากตำแหน่งบนแผนผังเพียงอย่างเดียว

ตัวอย่าง: หากถามว่า `Tower 5 จุดรวมพลอยู่ที่ไหน` เอกสารนี้เพียงอย่างเดียวยังไม่เพียงพอที่จะยืนยันจุดรวมพลของ Tower 5 ต้องถือเป็น Knowledge Gap จนกว่าจะมีข้อมูลที่ได้รับอนุมัติซึ่งจับคู่อาคารกับจุดรวมพลโดยตรง

## Fire Truck Parking Information — Separate from Assembly Points

ตัวเลขสีเหลือง **1–5** ในภาพเป็นข้อมูล `จุดจอดรถดับเพลิงสำหรับอาคาร` และต้องไม่ตีความว่าเป็นหมายเลข Assembly Point

ข้อมูลที่อ่านได้จากตารางในภาพ:

| หมายเลข | จุดจอดรถดับเพลิงสำหรับอาคาร | สถานที่ |
|---|---|---|
| 1 | วัน แบงค็อก ทาวเวอร์โฟร์, พาเหรด และเดอะ สตอรี่ส์ | จุดรับ-ส่ง อาคารเดอะ สตอรี่ส์ ทางเข้า 2 |
| 2 | วัน แบงค็อก ทาวเวอร์ทรี | ถนนพระรามที่ 4 ใกล้ทางเข้าที่ 3 |
| 3 | วัน พาวเวอร์ | ด้านหลังอาคาร วัน พาวเวอร์ |
| 4 | วัน แบงค็อก ฟอรั่ม | ด้านหลังอาคาร วัน แบงค็อก ฟอรั่ม |
| 5 | วัน แบงค็อก ทาวเวอร์ ไฟว์ | จุดรับ-ส่ง อาคาร โพสต์ ไนน์ทีน ทเวนตี้เอท |

> หมายเหตุจากภาพ: ทางโครงการจะมีการอำนวยความสะดวกด้านการจราจรและนำทางสำหรับรถดับเพลิงที่เข้ามาประจำจุดที่กำหนดไว้

## Retrieval / Answer Rules

- `Assembly Point` = จุดรวมพลสำหรับกระบวนการ Evacuation ตาม Canonical Terminology
- ใช้เอกสารนี้เพื่อยืนยันตำแหน่ง Assembly Point ที่แสดงในแผนผังเท่านั้น
- ห้ามสร้าง Building-to-Assembly-Point mapping จากความใกล้/ตำแหน่งบนแผนผัง
- ตัวเลข 1–5 เป็น Fire Truck Parking Points ไม่ใช่ Assembly Point numbers
- หากคำถามต้องการจุดรวมพลของอาคารเฉพาะ และยังไม่มี approved mapping ให้ตอบ `⚠️ KNOWLEDGE GAP — ไม่พบข้อมูลใน KB`
- ข้อมูล Fire Truck Parking ไม่เปลี่ยนแปลง Code 3 authority หรือ Evacuation workflow

## Change Log

- v1.0 — 2026-09-08 — Created from KB Owner-approved One Bangkok assembly point / fire truck parking map reference.
