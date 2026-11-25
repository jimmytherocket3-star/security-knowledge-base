---
document_id: SEC-SYS-CAT-001
title: CAT Classification & Priority
version: '1.0'
status: Approved
owner: KB Owner
updated: 2026-11-25
scope: SOC incident and case classification
---

# CAT Classification & Priority

## 1. Approved definitions

KB Owner provided the following definitions and authorized their storage on 2026-11-25.

| Category | เกณฑ์การจำแนก Priority | English description | SLA reference |
|---|---|---|---|
| CAT 1 | มีความสูญเสียร้ายแรง หรือมีความเสี่ยงในระดับสูง | Serious Loss or High Risk | 5 นาที |
| CAT 2 | มีผลกระทบกับลูกค้าโดยตรง | Direct Customer Impact | 10 นาที |
| CAT 3 | มีผลกระทบกับลูกค้าทางอ้อม | Indirect Customer Impact | 15 นาที |

The Thai definitions are the owner-approved canonical classification criteria. English descriptions are translations for training. SLA values are retained from [Code 1 overview v0.4](../01-emergency-codes/code-1/overview.md), whose overall status is Draft; this reference does not promote that SOP to Approved.

## 2. SLA interpretation

Code 1 is CAT 1 in the Code 1 reference. For Code 1, SLA means Acknowledge Case in Mozart within 5 minutes, not completion of verification or resolution.
- Start: SOC receives a human report, or Mozart automatically creates a Case from a system/device alert.
- Stop: SOC Acknowledges the Case in Mozart.

Do not generalize these start/stop rules to other cases without confirmation.

## 3. Source boundaries and guardrails

- Use the owner-approved definitions above for CAT classification questions.
- Preserve the historical KC-05 quarantine in [SOC Orientation](soc-orientation-operational-reference.md). The new definitions are directly owner-supplied, not inferred from orientation wording.
- Do not infer incident-specific classification, overlap/tie-breaking rules, escalation authority, color standards, or closure criteria from the table alone.
- CAT 2/3 SLA start/stop and detailed case-to-category mapping remain unconfirmed.
- Do not equate CAT levels with Emergency Codes or Threat Levels.

## Change Log

- v1.0 — 2026-11-25 — KB Owner supplied CAT 1/2/3 definitions and explicitly authorized recording in Skills Hunter; retained existing SLA reference and its boundaries.
