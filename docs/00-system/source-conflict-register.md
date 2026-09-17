---
document_id: KB-SYS-004
title: Skills Hunter Source Conflict Register
version: 1.1
status: Active
owner: KB Owner
scope: Conflict Tracking / AI Retrieval Control
effective_date: 2026-09-17
updated: 2026-09-17
---

# Skills Hunter Source Conflict Register

## Purpose and Authority

This register tracks explicitly identified disagreements between applicable Knowledge Base sources so Skills Hunter can disclose them without silently selecting a winner. Its **Active** status means the conflict-tracking and retrieval mechanism is approved for use. It does **not** approve either claim in a conflict record as the canonical fact. This register is not a source of newly decided operational facts and never replaces the original source documents.

The KB Owner alone approves additions, changes, reconciliation decisions, and issue-state changes in this register under `docs/00-system/kb-governance.md` and `docs/00-system/document-control.md`. AI must not resolve conflicts, promote a source, change an operational fact, or update this register on its own. Preserve the original claims, paths, source-declared statuses, decisions, and history for audit.

`Pending Reconciliation` is an **issue state**, not a formal document status. Formal document statuses remain those defined by KB governance and document control. An issue may be marked Resolved only after the KB Owner's approved decision and any required source and routing changes have been applied and checked; retain the record and its history.

## Conflict Record Fields

Each record identifies its Conflict ID, topic, conflict type, detected date, issue state, affected routes, and AI retrieval rule. For each source, record the path, document ID and version if supplied, source-declared status, precise location, and exact disputed claim. Keep canonical source, KB Owner decision, decision date, decision evidence, and resolution notes undetermined or blank until approved. Record dated issue and decision history without overwriting the original claims. Absence of a document ID or version must be stated rather than filled by inference.

## AI Retrieval Rule

Start with `KB-INDEX.md` and read the primary routed source. When a matching registered conflict exists, read every original source listed in the record directly. State each claim with its source path and status, disclose the unresolved conflict, and do not choose a canonical answer. A source-specific question may accurately quote that source, but must also disclose the registered disagreement. Use the Skills Hunter approved-source label only for attributed claims supported by their respective sources; use the Knowledge Gap label for a requested reconciled fact that remains unsupported. Do not infer a full name, role, authority, or operational instruction from the conflict record.

An issue is not created merely because a Draft differs from an Active canonical source, an External Reference has a different scope from an internal source, or an older reference omits a later approved addition. Preserve existing status priority, canonical precedence, source boundaries, and normal Knowledge Gap checks where no matching unresolved conflict exists.

## KB-CONFLICT-001 — One05 / ONE 05

| Field | Recorded evidence / state |
|---|---|
| Conflict ID | `KB-CONFLICT-001` |
| Topic | One05 / ONE 05 callsign-to-person label |
| Conflict Type | Personnel identity / callsign mapping |
| Detected Date | 2026-09-17 — documented during Skills Hunter retrieval review; not a claim about when the source disagreement first arose |
| Issue State | Pending Reconciliation |
| Source A | `docs/00-system/management-personnel-reference.md`; document ID `SEC-SYSTEM-PERSONNEL-001`; version `1.1`; source-declared status `Reference / Internal Personnel`; `Approved Personnel / Code Mapping` table, One05 row |
| Source A Claim | `| One05 | (คุณดิว) | วันศูนย์ห้า |` |
| Source A Boundary | Its Knowledge Gaps section says the full name for One05 is not supplied in the approved image. |
| Source B | `docs/08-reference/one-bangkok-executive-callsigns.md`; document ID not provided; version not provided; governance section states `Status: Approved`; callsign table, ONE 05 row |
| Source B Claim | `| ONE 05 | คุณนิว | — |` |
| Canonical Source | Undetermined |
| KB Owner Decision | Not yet decided |
| Decision Date | Not yet decided |
| Decision Evidence / Resolution Notes | Not yet provided |
| Affected Routes | `KB-INDEX.md` — One00–One05 personnel route and One05 query example |
| AI Retrieval Rule | Read both original sources; state both claims with provenance and their source-declared statuses; disclose the unresolved conflict. Do not select a winner or infer a full name, role, authority, or canonical identity. |

### Issue History

| Date | Event | Approval / result |
|---|---|---|
| 2026-09-17 | Created the first conflict record from the two existing One05 source claims. | KB Owner approved Phase 4B implementation; issue state is Pending Reconciliation. No canonical-source or identity decision was made. |

## KB-CONFLICT-002 — FCC expansion in Code M

| Field | Recorded evidence / state |
|---|---|
| Conflict ID | `KB-CONFLICT-002` |
| Topic | FCC acronym expansion in Code M context |
| Conflict Type | Terminology / organizational label |
| Detected Date | 2026-09-17 — identified during Code M Knowledge Gap closure and reconciliation review |
| Issue State | Pending Reconciliation |
| Source A | `docs/00-system/terminology.md`; document ID `KB-SYS-003`; version `1.9`; source-declared status `Active`; Canonical Terms table, FCC row |
| Source A Claim | `FCC = Fire Command Center` |
| Source B | `docs/01-emergency-codes/code-m/overview.md`; document ID `SEC-CODE-M-001`; version `1.0`; source-declared status `Approved Reference`; §4 FCC source-boundary note |
| Source B Claim | The Code M source supplied by the KB Owner labels `FCC = Facility Control Center` while attributing Code M coordination actions to FCC. |
| Canonical Source | Undetermined for reconciliation of the Code M source wording; the existing canonical terminology remains unchanged pending a KB Owner decision. |
| KB Owner Decision | Conflict registration approved; terminology reconciliation not yet decided. |
| Decision Date | 2026-09-17 for conflict registration only |
| Decision Evidence / Resolution Notes | KB Owner approved the Code M change proposal on 2026-09-17. No decision was made to replace `Fire Command Center` or to adopt `Facility Control Center` as canonical. |
| Affected Routes | `KB-INDEX.md` — terminology route and Code M procedure route |
| AI Retrieval Rule | For general canonical terminology, read `docs/00-system/terminology.md`. For Code M, read `docs/01-emergency-codes/code-m/overview.md` and disclose that its supplied source used `Facility Control Center`. Do not silently change the canonical FCC expansion or reinterpret the Code M operational actions while reconciliation is pending. |

### Issue History

| Date | Event | Approval / result |
|---|---|---|
| 2026-09-17 | Registered the FCC expansion disagreement discovered during Code M Knowledge Gap closure. | KB Owner approved registration as part of the Code M change proposal; issue state Pending Reconciliation. No terminology winner selected. |

## Change Log

| Version | Date | Change | Approved By |
|---|---|---|---|
| 1.0 | 2026-09-17 | Created the conflict-tracking mechanism and unresolved `KB-CONFLICT-001`, preserving both One05 claims and their provenance. | KB Owner — Phase 4B implementation approval |
| 1.1 | 2026-09-17 | Added `KB-CONFLICT-002` for the unresolved FCC expansion disagreement in Code M; no canonical terminology decision made. | KB Owner — Code M change proposal approval |
