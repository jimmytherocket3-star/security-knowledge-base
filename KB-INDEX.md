---
document_id: SEC-KB-INDEX-001
title: Security Knowledge Base Retrieval Index
version: 1.0
status: Active
owner: KB Owner
scope: AI Retrieval / Repository Routing
updated: 2026-09-08
---

# Security Knowledge Base Retrieval Index

## Purpose

This file is the primary routing index for AI retrieval in `jimmytherocket3-star/security-knowledge-base`.

When answering a question from this KB, use this index to identify the most relevant source file and fetch/read that file directly. A failed GitHub search alone is not evidence that the KB lacks the information.

## Mandatory Retrieval Rule

1. Read this index first when the relevant KB file is not already known.
2. Route the question to the most relevant file below.
3. Fetch/read the target file directly rather than relying only on repository search.
4. Prefer the latest Approved/Active material when sources conflict, subject to document-specific status and guardrails.
5. If search returns no result, check the routed file directly before declaring a Knowledge Gap.
6. Declare a Knowledge Gap only after the relevant routed source has been checked and does not support the requested fact.
7. Never invent internal facts or silently replace missing internal KB information with external information.
8. KB create/edit/delete operations require explicit KB Owner approval before modification.

## Routing Table

| Question / Topic | Primary KB File | Retrieval Note |
|---|---|---|
| One00, One01, One02, One03, One04, One05; management personnel names/nicknames | `docs/00-system/management-personnel-reference.md` | Fetch directly for One00–One05 questions. Do not rely on search alone. |
| Building names, locations, Zone/Zoning, Loading 1–8, site labels | `docs/00-system/location-building-directory.md` | Use for approved location/building/loading mappings. |
| Internal/external emergency contacts, BMO, SOC, DCC, FMC, hotel contacts, First Aid | `docs/00-system/emergency-contact-directory.md` | Blank/unconfirmed values must not be guessed. |
| MOD duty schedule for May 2026 | `docs/00-system/mod-duty-schedule/2026-05.md` | Time-bound reference only; do not treat as permanent contact data. |
| Terminology, abbreviations, roles, EMER_1/EMER_2, BMO, DCC, IMT, EOT, SOC, FCC, General Alarm, Assembly Point | `docs/00-system/terminology.md` | Use canonical terminology definitions. |
| Canonical Code 1, Code 2, Code 3 definitions | `docs/01-emergency-codes/code-definitions.md` | Use as primary source for code definitions. |
| Code 1 detailed workflow/reference | `docs/01-emergency-codes/code-1/overview.md` | Check status/version and defer to canonical definitions where conflicting. |
| Code 2 detailed workflow/reference | `docs/01-emergency-codes/code-2/overview.md` | Check status/version and defer to canonical definitions where conflicting. |
| Code 3 / Evacuation procedure | `docs/01-emergency-codes/code-3/overview.md` | Use latest approved Code 3 procedure. |
| Code Sierra / Active Shooter | `docs/01-emergency-codes/code-sierra/overview.md` | Use current stored canonical document; do not silently apply unapproved corrections. |
| ONE89 Wireless residential fire evacuation drill 2026 | `docs/02-building-procedures/residential/one89-wireless/2026-fire-evacuation-drill.md` | Drill-specific/residential reference; do not generalize to all buildings. |
| GitHub KB-first retrieval behavior and source priority | `docs/00-system/github-kb-first-retrieval-policy.md` | Governs KB-first retrieval behavior. |
| Assistant persona / Kuroro | `docs/00-system/assistant-persona.md` | Persona only; does not alter SOP authority. |

## Query Routing Examples

- `One 04 ชื่ออะไร` → fetch `docs/00-system/management-personnel-reference.md`
- `One 00 ชื่ออะไร` → fetch `docs/00-system/management-personnel-reference.md`
- `Loading 5 เป็นของอาคารอะไร` → fetch `docs/00-system/location-building-directory.md`
- `Zone 3 มีอาคารอะไรบ้าง` → fetch `docs/00-system/location-building-directory.md`
- `เบอร์ SOC` → fetch `docs/00-system/emergency-contact-directory.md`
- `Code 3 คืออะไร` → fetch `docs/01-emergency-codes/code-definitions.md`, then `docs/01-emergency-codes/code-3/overview.md` if procedural detail is requested
- `Code Sierra` → fetch `docs/01-emergency-codes/code-sierra/overview.md`
- `จุดรวมพล ONE89 ตามแผนซ้อม` → fetch `docs/02-building-procedures/residential/one89-wireless/2026-fire-evacuation-drill.md`

## Source Priority

`Latest Approved/Active KB → Approved Reference KB → Knowledge Gap → External source only when explicitly requested or clearly separated`

A repository search miss does **not** move the answer directly to Knowledge Gap. The routed source file must be checked first.

## Guardrails

- This index routes retrieval; it does not create new SOP facts.
- File status and document-specific guardrails remain authoritative.
- Do not infer emergency authority from personnel/location/contact reference files.
- Do not normalize source spellings or aliases unless explicitly approved.
- Do not generalize drill-specific procedures into Core SOP.
- Do not modify this index or any routed KB file without explicit KB Owner approval.

## Change Log

- v1.0 — 2026-09-08 — Created as the central AI retrieval/router index to reduce false Knowledge Gaps caused by repository search misses.
