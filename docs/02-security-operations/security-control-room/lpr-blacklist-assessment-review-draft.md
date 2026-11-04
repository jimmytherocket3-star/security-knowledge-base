# SOC LPR Blacklist Dashboard — Assessment Review and Training Pack

**Document ID:** SEC-SOC-LPR-001  
**Version:** 0.1  
**Status:** Draft — NOT an approved LPR SOP or certification examination  
**Owner:** KB Owner  
**Date:** 2026-11-04  
**Source A:** User upload `เอกสารฉบับนี้เป็น แนวข้อสอบและเฉลยส.md` (a one-paragraph overview; not 60 question texts).  
**Source B:** User upload `เอกสารฉบับนี้เป็น แนวข้อสอบและเฉลยส(1).md` (44-line summary of assessment, dashboard screenshot and operating principles).  
**Cross-check:** `docs/00-system/terminology.md` v1.9 Active; `docs/00-system/soc-basic-legal-awareness-reference.md` Approved Internal Training Reference; `docs/00-system/source-conflict-register.md` (no LPR-specific entry found).

## 1. Source comparison

| Topic | Source A | Source B | Assessment |
|---|---|---|---|
| Title | SOC LPR Blacklist Dashboard assessment | SOC Knowledge Assessment: LPR Blacklist Dashboard | Consistent topic |
| Multiple choice | 60 items | 60 items, 60 points | Consistent |
| Scenario essays | 4 scenarios | 4 scenarios, 10 points each | Consistent |
| Total/pass | 100 / 80 | 100 / at least 80 | Consistent |
| Detailed answer keys | Says keys and explanations exist | Summarizes principles, not full answer key | **Not supplied in these two uploaded files** |
| Assessment topics | Evidence, uncertainty, SOP coordination | OCR, live images, PDPA, Contact Matrix, offline cameras, escalation | Source B is more detailed; not contradiction |
| Critical error rule | Not specified | Blacklist modification, unauthorized disclosure, unsupported closure, failure to escalate | Source B only; verification needed |
| Solo-work clearance | Not specified | Vital Knowledge and no Critical Error | Source B only; verification needed |
| Dashboard counts | Not specified | 117 blacklisted people, 2 watchlisted, 26 construction, 7 blacklisted plates, 18 whitelisted plates | **Screenshot snapshot only; never present as live totals** |

## 2. Accuracy and SOP verification

**Supported by both uploaded summaries:** 60 MCQ, 4 scenario essays, total 100, pass 80, evidence-based judgment, separate confirmed facts from uncertain facts.

**Supported by Source B only (not independently verified as an approved SOP):**
- Blacklist Match is an alert, not proof of driver's identity or current wrongdoing.
- Verify plate/image/camera/time and OCR uncertainty; avoid overclaiming.
- Route notifications through the location-specific Contact Matrix; require field acknowledgement, follow-up, escalation when needed.
- Acknowledged does not equal incident resolved; closure requires verified field outcome under applicable SOP.
- Unauthorized blacklist edits/disclosure, unverified closure, or ignored risk described as Critical Errors.
- Whitelist status does not eliminate independent safety risks.
- Scoring essays: 5 dimensions, each 0–2, across 4 essays.
- Clearance for independent work requires Vital Knowledge and no Critical Error.

**KB cross-check:** Canonical terminology supports SOC Operator duties, CCTV, Virtual Patrol and Mozart-related terminology, but does **not** establish LPR-specific workflow or Contact Matrix. Approved SOC Legal Awareness training supports restricting public disclosure of CCTV imagery and following organizational CCTV Request SOP; it does not itself approve LPR access rights, retention or LPR case-closure workflow. No LPR-specific conflict entry found in the checked conflict register.

**Open verification items (do not infer):** actual 60 questions/answers; actual 4 scenario answer keys; active LPR SOP and revision; approved Contact Matrix with recipient/channel/backups; blacklist edit/approval authority; access controls and retention; technical alert status definitions; precise Vital Knowledge/Critical Error evaluation and appeal rules; dashboard timestamp/data provenance.

## 3. Training outline (derived from Source B; instructional draft)

1. Dashboard orientation: individual vs vehicle categories; historical screenshot figures are not live counts.
2. Alert verification: source camera, capture timestamp, plate characters, OCR limitations, list status and live scene.
3. Fact vs uncertainty: vehicle match does not identify driver or prove current offence.
4. Communications: only necessary information, location-specific authorized recipients, acknowledgement, follow-up and escalation.
5. Safety/PDPA: need-to-know access, no unauthorized images or blacklist changes.
6. Case handling: time-ordered log, field result, evidence-based closure; Acknowledged ≠ Resolved.
7. Technical fallback: offline/frozen camera and stale data; report technical issue, use authorized alternate observation, do not disable alerts without authority.

## 4. Practice exercises — NEW instructional examples, not source exam items

**Exercise A (Blacklist match):** The plate appears to match an active blacklist and live vehicle image is consistent; driver identity unknown. Explain what is verified vs unknown, how to notify per approved Contact Matrix, and what field confirmation is needed before closure.

**Exercise B (OCR ambiguity):** Reflection obscures characters and multiple similar plates appear. Explain checks for image/time/camera and how to report uncertain matching without declaring a positive match.

**Exercise C (Whitelist and obstruction):** A whitelisted vehicle blocks an emergency access route. Explain why whitelist status does not remove the safety issue, which on-scene verification to request, and how to track reopening of the route.

**Exercise D (Camera offline):** Live image is unavailable and blacklist records may be stale. Explain technical vs incident uncertainty, escalation to system owner and supervisor, authorized backup observation, and prohibition on unauthorized alert/list edits.

**Practice answer rubric (Source B):** For each exercise, score 0–2 on (1) fact/uncertainty separation, (2) camera/time/image/risk checks, (3) SOP/Contact Matrix recipient and message, (4) acknowledgement/follow-up/escalation, (5) chronological log and verified closure. Max 10 per exercise; 40 for all four. Do not use this as a formal pass/fail or solo-work clearance without approved examination source.

## 5. Sample response framework (NOT an approved SOP)

> เวลา [เวลา] ระบบ LPR แสดง Alert ที่กล้อง [จุด/รหัส] ทะเบียนที่ระบบอ่านได้ [ข้อมูล] โดย [ยืนยันจากภาพ/ยังอ่านไม่ชัด]. ขณะนี้ยังไม่ยืนยัน [ตัวผู้ขับ/สถานะรายการ/การเคลื่อนที่]. ขอให้ผู้รับผิดชอบตาม Contact Matrix ตรวจสอบพื้นที่และยืนยันผลกลับ SOC; SOC จะบันทึกเวลา ผู้รับแจ้ง ผลตรวจ และติดตามจนได้หลักฐานเพียงพอตาม SOP ก่อนปิดเหตุ

## 6. Owner review checklist

- [ ] Supply complete exam items and original keys to permit question-by-question verification.
- [ ] Verify LPR SOP and location Contact Matrix from current approved originals.
- [ ] Verify access/PDPA/retention and edit authority from system owner.
- [ ] Verify critical error and independent-duty certification rules.
- [ ] Confirm historical screenshot data and capture date.
- [ ] Approve training pack separately from operational SOP and formal assessment.

**Revision history:** v0.1 (2026-11-04) — source comparison, evidence limits, verification gaps and separately labeled practice exercises.
