---
document_id: SEC-SYS-SKILLS-HUNTER-001
title: Skills Hunter — Knowledge System Identity
version: 1.0
status: Active
owner: KB Owner
scope: Knowledge System Branding / AI Retrieval
updated: 2026-09-08
---

# Skills Hunter

## Definition

**Skills Hunter** = ชื่อเรียกระบบ Knowledge Base ของผู้ใช้สำหรับจัดเก็บ ค้นหา เชื่อมโยง และนำ Approved Knowledge มาใช้ โดยมี GitHub repository `jimmytherocket3-star/security-knowledge-base` เป็นแหล่งข้อมูลหลัก

## Technical Identity

- Display / conversational name: **Skills Hunter**
- Technical system: **Security Knowledge Base**
- GitHub repository: `jimmytherocket3-star/security-knowledge-base`
- Repository name and existing file paths remain unchanged.

## Usage

เมื่อผู้ใช้กล่าวว่า:
- `ค้นใน Skills Hunter`
- `หาใน Skills Hunter`
- `บันทึกเข้า Skills Hunter`
- `ตรวจสอบจาก Skills Hunter`

ให้ตีความว่าเป็นการอ้างถึง Knowledge Base เดียวกับ repository `jimmytherocket3-star/security-knowledge-base` และให้ใช้กฎ Retrieval / Governance เดิมทั้งหมด

## Governance

1. Skills Hunter เป็น Branding Layer ของ Knowledge Base เดิม ไม่ใช่ Knowledge Base แยกชุดใหม่
2. Approved/Active Knowledge และ source priority เดิมยังคงมีผล
3. การสร้าง แก้ไข หรือลบข้อมูลใน Skills Hunter ต้องได้รับการอนุมัติจาก KB Owner ก่อน
4. ห้ามเปลี่ยน Emergency SOP, Authority, Terminology หรือ operational facts เพียงเพราะเปลี่ยนชื่อระบบ
5. Repository และ path เดิมยังคงใช้เพื่อรักษาความต่อเนื่องของ AI retrieval และ routing

## Answer Label

ชื่อแสดงผลสำหรับคำตอบที่ตรวจสอบจากระบบนี้สามารถใช้:

**✅ SKILLS HUNTER — APPROVED**

โดยมีความหมายเทียบเท่า source-status เดิม **✅ KB APPROVED** และไม่ได้เปลี่ยนมาตรฐานการตรวจสอบแหล่งข้อมูล

## Change Log

- **v1.0 — 2026-09-08:** KB Owner approved the Skills Hunter branding layer for the existing Security Knowledge Base.
