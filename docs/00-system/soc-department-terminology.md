# SOC Department Terminology — Source Comparison Register

**Document ID:** SEC-SOC-TERM-001  
**Version:** 0.1  
**Status:** Draft — KB Owner review required before promotion  
**Owner:** KB Owner  
**Date:** 2026-10-18  
**Source:** User-supplied `คำศัพท์ประจำแผนก.md` (64 numbered terms, additional unnumbered terms, duplicate numbering and entries).  
**Canonical reference:** `docs/00-system/terminology.md` v1.9 (Active).

## Purpose and evidence boundaries

This is a **review register**, not a new authoritative glossary or SOP. The supplied source is the basis for all candidate terms. The complete original descriptions remain in the user-supplied source file; this register retains **term names and comparison status**, rather than pretending to reproduce full original definitions. Before publishing an approved glossary with full definitions, import the complete source text without silent edits and reconcile conflicts.

- **Existing:** already represented in the Canonical Terminology; use canonical wording, not conflicting source expansions.
- **New:** candidate not present as its own canonical entry; requires definition and approval before becoming canonical.
- **Pending:** source conflicts with or expands approved terminology, or needs verification; do not use source as operational authority.
- Existing/New/Pending labels indicate comparison status, **not approval** of new definitions or workflows.
- The source contains duplicate number 8, unnumbered entries, and Technician appearing twice; counts below are **deduplicated concepts**, not numbered source rows.
- Do not infer roles, emergency authority, radio channels, SLAs, SOP steps, or building boundaries from terminology alone.

## Term-by-term comparison

| # | Source term | Review status | Notes |
|---:|---|---|---|
| 1 | SOC | Existing | Canonical spelling Center; source Centre |
| 2 | SOC Supervisor | Existing | — |
| 3 | SOC Operator | Existing | — |
| 4 | CCTV | New | — |
| 5 | Picture | Existing | Combined Picture / Video Retention |
| 6 | Video | Existing | Combined Picture / Video Retention |
| 7 | VMS | New | — |
| 8 | Distcher | Pending | Verify product spelling; possible Dispatcher |
| 9 | VP Facility Management – Integrated Operations Control | New | Authority claims require verification |
| 10 | Assistant VP Command Centre Operations | New | Authority claims require verification |
| 11 | ผู้มีอำนาจหรือผู้ที่มีสิทธิ์อนุญาต | New | Do not infer code-specific authority |
| 12 | CRM | Existing | — |
| 13 | Concierge / Reception | New | — |
| 14 | เจ้าพนักงานของรัฐ | New | — |
| 15 | เจ้าหน้าที่ตำรวจ | New | — |
| 16 | Common Infrastructure (CI) | Pending | Expanded area list not canonical |
| 17 | Zone 1 | Pending | Building list requires location-source verification |
| 18 | Zone 2 | Pending | Building list requires location-source verification |
| 19 | Zone 3 | Pending | Building list requires location-source verification |
| 20 | Zone 4 | Pending | Building list requires location-source verification |
| 21 | One Power (CUP) | New | — |
| 22 | Retail | New | Building lists require verification |
| 23 | Tower | New | Building lists require verification |
| 24 | Hotel | New | Building lists require verification |
| 25 | Condominium | New | Building lists require verification |
| 26 | Lost Property | New | — |
| 27 | Found Property | New | — |
| 28 | เจ้าของทรัพย์สิน | New | — |
| 29 | Claim of Ownership | New | — |
| 30 | ผู้ส่งมอบคืนทรัพย์สิน | New | — |
| 31 | ผู้แจ้ง / ผู้ร้องขอ | New | — |
| 32 | Code Seirra | Pending | Canonical spelling Code Sierra; operational scope requires SOP |
| 33 | Code Mike / Code M | Pending | Canonical Medical Emergency; expanded clinical definition not approved |
| 34 | Code Delta / Code D | Existing | No implied procedure or declaration authority |
| 35 | ผู้พบเหตุคนแรก | New | — |
| 36 | ผู้เคราะห์ร้าย | New | — |
| 37 | ผู้ประสบเหตุ | New | — |
| 38 | ผู้ก่อเหตุ | New | — |
| 39 | IC / Incident Commander | Existing | — |
| 40 | ERT | Existing | — |
| 41 | CMT | Existing | — |
| 42 | IMT | Pending | CAT1/CAT2 scope not approved |
| 43 | DCC | Existing | — |
| 44 | BMO | Existing | — |
| 45 | FMC | Existing | — |
| 46 | EOT | Existing | — |
| 47 | TMT | Existing | Not interchangeable with SMT |
| 48 | EMT | Existing | — |
| 49 | พยาบาล | New | — |
| 50 | Contact Centre | New | — |
| 51 | Safety | New | — |
| 52 | Technician | New | Repeated in source |
| 53 | Security Guard | New | — |
| 54 | Cleaner | New | — |
| 55 | Mozart | Existing | Source wider service scope; retain canonical |
| 56 | Event Type | New | — |
| 57 | เลขเคส | New | — |
| 58 | Video Analytic | Existing | — |
| 59 | Virtual Patrol | Existing | — |
| 60 | PA | Pending | SOC/FMC control authority not reconciled |
| 61 | Access Control | Existing | — |
| 62 | ภัยคุกคามระดับสีดำ | Pending | DCC response authority unverified |
| 63 | การปฐมพยาบาลเบื้องต้น | New | — |
| 64 | รถพยาบาล | New | — |
| 65 | DCC Alignment | Existing | — |
| 66 | FS | Existing | — |
| 67 | IBT | Existing | — |

**Review counts:** Existing 23; New 33; Pending 11; total 67 distinct mapped concepts. Duplicate source entries (e.g. CRM, Technician, police) are consolidated. 

## Priority reconciliation

1. **SOC:** supplied file uses *Security Operation Centre*, while Canonical v1.9 uses *Security Operation Center*; canonical spelling prevails pending owner decision.
2. **IMT:** supplied CAT 1 / CAT 2 scope is not an approved replacement for canonical IMT membership/authority.
3. **Code Sierra:** supplied spelling *Seirra* is incorrect; Run Hide Fight and other Code Sierra actions must come from its approved SOP, not the glossary excerpt.
4. **Code M:** expanded clinical definition does not replace *Medical Emergency* without specific approval.
5. **CI:** source lists Carpark, External Area, One Bangkok Park, Wireless Park and Loading Dock; do not silently expand canonical CI scope.
6. **PA:** source claims zone-wide announcement control from SOC and FMC; do not infer operational permissions without reconciliation.
7. **Black Threat:** do not treat the source claim about DCC high-level measures as approved response instructions.
8. **Zone 1–4:** compare the building lists against current approved location references before making them authoritative.
9. **Distcher:** preserve exact source spelling while verifying whether *Dispatcher* is intended.
10. **Management roles:** supplied VP/Assistant VP approval descriptions are not code-specific authorization.

## Next approval gate

KB Owner should review Pending items and candidate New definitions against approved SOP and location references. Once approved, prepare a separate full-definition SOC glossary using the **verbatim source definitions**, marking any corrections explicitly, and propose canonical changes individually. No automatic edits to `docs/00-system/terminology.md`.

## Revision history

- v0.1 (2026-10-18): initial comparison register created after KB Owner authorization; Draft only.
