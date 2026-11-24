---
document_id: SEC-INSTR-METHOD-001
title: Instructor-provided SOC operational methodologies
version: "0.1"
status: Draft
owner: KB Owner
source_classification: Instructor-Provided Knowledge
updated: 2026-11-24
---
# Instructor-provided SOC operational methodologies

Public-screened, condensed training reference from SOC-Knowledge-main.zip, source provenance confirmed by KB Owner. Import authorized 2026-11-24. Source documents themselves are draft. This is not an approved site SOP, nor a replacement for canonical terminology. Site-specific examples, personnel, system mappings and deployment details intentionally excluded.

## Operational Problem Decomposition Framework
Source: 00-governance/methodologies/operational-problem-decomposition-framework.md (2026-07-26).
- Define problem, verify current condition, scope and risk; identify stakeholders and consult process/product/system owners.
- Define acceptance criteria, run limited pilot, collect evidence, assess accuracy, workload, failure modes and operational impact.
- Decide reject/revise/further pilot/rollout, assign owner, monitor and capture lessons learned.
- Do not start with a preferred technology and seek a problem to justify it. Address verified operational control gaps; future-proofing does not replace current controls.
- Measure success, false alerts, missed events, unclassifiable results, workload, escalation impact, maintainability, ownership and support dependencies.

## Solution Acceptance and UAT Framework
Source: 00-governance/standards/solution-acceptance-and-uat-framework.md (2026-07-26).
- Configuration success is not operational acceptance; screenshots alone are insufficient.
- Test relevant end-to-end service chain, expected vs actual results, pass/fail and timestamped evidence.
- Include negative tests, exception handling, missing/delayed/duplicate events, mapping errors and unavailable playback where applicable.
- Verify role permissions, ownership, defect severity, retest criteria, rollback/workaround/escalation and post-go-live monitoring.
- Distinguish configuration owner, tester, acceptance authority, final approver and support owner. Vendor evidence alone is insufficient.

## Mission Readiness Under Uncertainty — selected general concepts
Source: 00-governance/methodologies/mission-readiness-under-uncertainty.md (2026-07-27).
- Fixed Core Readiness: reversible low-risk preparatory work without configuration or permission changes.
- Scenario Modules: clearly label assumptions.
- Final Confirmed-Parameter Overlay: apply confirmed parameters before actual execution.
- Distinguish Confirmed, Unconfirmed, Assumption, Pending Verification, Approval Required and Decision Status.
- Preserve source, timestamp and applicable date separately. Disclose conflicts without selecting a winner; distinguish estimates from verified actuals.
- Search with exact terms and synonyms, read relevant original records and cross-check available sources; report coverage limitations.

## Change log
0.1 — 2026-11-24 — Initial public-screened knowledge extract; not full source import. KB Owner authorized import, not promotion to Active SOP.
