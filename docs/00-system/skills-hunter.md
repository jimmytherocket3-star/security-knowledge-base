---
document_id: SEC-SYS-SKILLS-HUNTER-001
title: Skills Hunter — Knowledge System Identity
version: 1.1
status: Active
owner: KB Owner
scope: Knowledge System Branding / AI Retrieval
system_release_version: "2.0"
release_baseline_commit: "4a5a2bddf73498be9b2130f886be5b4ee189d1a3"
release_declared_on: 2026-09-17
updated: 2026-09-17
---

# Skills Hunter

## Definition

**Skills Hunter** = ชื่อเรียกระบบ Knowledge Base ของผู้ใช้สำหรับจัดเก็บ ค้นหา เชื่อมโยง และนำ Approved Knowledge มาใช้ โดยมี GitHub repository `jimmytherocket3-star/security-knowledge-base` เป็นแหล่งข้อมูลหลัก

## Technical Identity

- Display / conversational name: **Skills Hunter**
- Technical system: **Security Knowledge Base**
- GitHub repository: `jimmytherocket3-star/security-knowledge-base`
- Repository name and existing file paths remain unchanged.

## System Release — Skills Hunter 2.0

**Skills Hunter 2.0** is the current KB Owner-approved system release of the existing Security Knowledge Base's KB-first, centrally routed, status-aware retrieval system. This is a **system release version**, not a version assigned to every KB document.

The verified pre-declaration technical baseline is Git commit `4a5a2bddf73498be9b2130f886be5b4ee189d1a3`. The release baseline includes KB-first retrieval, central routing through `KB-INDEX.md`, direct reading of original sources, document-status-aware retrieval, Knowledge Gap handling, source provenance and integrity safeguards, and approval-before-write governance. It also includes registered-conflict detection and handling through `docs/00-system/source-conflict-register.md`: read the original sources, preserve their claims and statuses, disclose unresolved disagreement, and do not select a conflict winner automatically. Reconciliation decisions belong to the KB Owner.

### Version Boundaries

- **Skills Hunter 2.0** is the overall system/release version.
- **This document v1.1** is the version of the Skills Hunter identity and release declaration document.
- **`KB-INDEX.md` v1.9** is the routing-index document version, not the system release version.
- **Individual source document versions and statuses** remain independent. No source becomes v2.0 merely because the system release is 2.0.
- **A Git commit SHA** identifies a repository state. The baseline SHA above identifies the pre-declaration technical baseline, not the later release-declaration commit.

### Release Boundaries and Open Issue

Skills Hunter 2.0 does not mean all KB knowledge is complete, all source documents are Active, all conflicts or Knowledge Gaps are resolved, or every future answer is automatically correct. It does not ensure every future ChatGPT session has repository access or universal retrieval enforcement. Draft and Reference material retain their own statuses and scope; this release does not promote them to Approved/Active operational knowledge. AI gains no authority to modify the KB or reconcile conflicting sources.

`KB-CONFLICT-001` remains **Pending Reconciliation**, with **Canonical Source: Undetermined**. Skills Hunter 2.0 uses the active conflict-management mechanism but does not resolve the One05 identity disagreement. The original-source claims, issue state, and KB Owner decision record remain in `docs/00-system/source-conflict-register.md`.

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

- **v1.1 — 2026-09-17:** Formally declared Skills Hunter system release 2.0 and recorded the verified pre-declaration technical baseline `4a5a2bddf73498be9b2130f886be5b4ee189d1a3`, system/document version boundaries, and release limitations.
- **v1.0 — 2026-09-08:** KB Owner approved the Skills Hunter branding layer for the existing Security Knowledge Base.
