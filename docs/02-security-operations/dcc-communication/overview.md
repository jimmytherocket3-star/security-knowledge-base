---
document_id: SEC-DCC-COMM-001
title: DCC Communication & Notification Protocol — Operational Reference
version: 0.1
status: Draft
owner: KB Owner
scope: DCC Communication / Notification / Advance Notification / Urgent Notification
updated: 2026-09-30
---

# DCC Communication & Notification Protocol — Operational Reference

## 1. Status and Source Boundary
This document is a **Draft Operational Reference** derived from the KB Owner-supplied summary of **OB-SOP-DCC-0007 — Communication & Notification Protocol (Rev.02)**.

The supplied source states that OB-SOP-DCC-0007 defines DCC communication and notification for planned advance communication and urgent/unexpected situations. Missing facts are preserved as Knowledge Gaps and must not be inferred.

## 2. Purpose
Provide a controlled operational reference for DCC communication and notification, covering advance communication for planned activities and urgent notification for unexpected or time-sensitive events.

## 3. Notification Types
The source establishes two main types:

### 3.1 Advance Notification / Communication
Advance communication for planned activities, including examples such as:
- Event
- Area closure / improvement work
- Non-urgent maintenance

### 3.2 Urgent Notification / Notification
Notification for unexpected events or situations requiring communication within a limited time, including examples such as:
- Unexpected events
- Emergency maintenance
- Sudden schedule changes

Separate definitions for Planned, Emergency, and Unplanned are not established.

## 4. Trigger
The source-supported workflow begins when DCC receives information from a **Data Source**.

Specific additional trigger categories such as System Shutdown or Service Interruption are not established by the supplied source.

## 5. Initiator / Data Source
The Data Source sends information directly to DCC.

Examples identified by the source:
- FMC
- SOC
- Event team
- Tenant team
- Event organizer

Whether DCC may independently initiate the workflow based on its own detection is not established.

## 6. Authority / Review
### DCC Manager
DCC Manager reviews the draft for:
- Accuracy
- Completeness
- Appropriateness
- Language

### DOFM Escalation
If the information is confidential, may directly or indirectly affect the project, or requires consultation, DCC Manager escalates to **DOFM** for advice and direction before communication.

The source does not establish a separate approval authority by notification type or an emergency exception allowing publication before approval.

## 7. Recipients
The source describes recipients as **Relevant Stakeholders / relevant units**, with examples including:
- Operations
- Security team

A complete recipient matrix and event-specific recipient mapping are not established.

## 8. Communication Channels
The source refers to a designated communication platform/channel but does not identify specific channels such as Email, LINE, Radio, PA, or a Primary/Backup channel.

## 9. Advance Notification Workflow
1. DCC receives and records information from the Data Source.
2. DCC collects and checks completeness, including purpose, schedule, affected area, and relevant units.
3. If information is incomplete, DCC coordinates with the Data Source until the information is complete.
4. DCC prepares a draft message using the project's standard format.
5. DCC Manager reviews the draft.
6. If revision is required, the draft is returned for correction.
7. If the information is confidential, may affect the project, or requires consultation, DCC Manager escalates to DOFM for advice/direction before communication.
8. DCC publishes the information through the designated channel.
9. DCC follows and updates the situation when information changes until the event ends.

**Timing requirement:** Advance Notification must be sent at least **1 day before the event date**.

Confirm Receipt requirements are not established.

## 10. Urgent Notification Workflow
Urgent Notification uses the same source-supported workflow as Advance Notification.

**Timing requirement:** Relevant units must be notified within **30 minutes**.

Additional updates are sent during or after the event as necessary.

The source does not establish the first-recipient sequence or a formal Initial → Escalation → Final status model.

## 11. Required Message Content
The source identifies six required content components:
1. Notification subject
2. Event details
3. Date and time period
4. Affected area
5. Unit/contact for enquiries
6. Additional update plan, if applicable

A named template or standard Subject format is not established in the supplied source.

## 12. Escalation
Established:
- Confidential / project-impacting / consultation-required draft → DCC Manager escalates to DOFM for advice/direction before communication.

Not established:
- Escalation for no acknowledgement
- Escalation when severity increases
- Escalation when a communication system/channel fails

## 13. Acknowledgement / Confirmation
No formal recipient acknowledgement or Confirm Receipt process is established.

The source states that DCC follows the situation and operational results after communication.

## 14. Update Frequency
Updates are provided during or after the event as necessary, including when circumstances change or additional information becomes available, until the event ends.

No fixed minute/hour update interval is established.

## 15. Termination / Final Notification
The source states that once information has been published and updated as required until the event ends, that communication cycle is complete.

The source does not establish:
- All Clear authority
- A required Final Notification format
- A separate formal closure authority

## 16. Records and Evidence
Established:
- DCC records the information-receipt entry when information is received from the Data Source.

The source summary notes that the definition of Mozart was removed from Rev.01.

Not established:
- Specific evidence type such as Email, LINE screenshot, call log, or other retained communication evidence
- Retention requirement
- Evidence approval/verification workflow

## 17. Failure / Backup Communication
No backup communication procedure is established for failure of the primary communication system/channel.

## 18. Knowledge Gaps
1. Complete Recipient Mapping by event/notification type.
2. Specific Communication Channel and Primary/Backup Channel.
3. Recipient Acknowledgement / Confirm Receipt process.
4. Escalation workflow for no response, increasing severity, or communication-system failure.
5. Fixed Update Frequency, if required.
6. Final Notification / All Clear authority and format.
7. Specific Records/Evidence and retention requirements.
8. Whether DCC may initiate a notification independently from its own detection.
9. Named project message template / standard Subject format.
10. Separate approval rules or emergency exception, if any.

## 19. Guardrails
- Do not invent recipient lists beyond the source-supported examples.
- Do not infer Email, LINE, Radio, PA, POC, or any other specific communication channel.
- Do not infer a backup communication channel.
- Do not invent Confirm Receipt or acknowledgement requirements.
- Do not invent an All Clear / Final Notification authority.
- Do not convert the 30-minute Urgent Notification requirement into a different emergency-code SLA.
- Do not infer that DCC may bypass DCC Manager review in urgent cases.
- Preserve Advance Notification and Urgent Notification terminology from the source.
- Preserve Draft status until operational gaps are reviewed and the KB Owner explicitly approves promotion.

## 20. Source Traceability
Primary supplied source:
- KB Owner-provided summary based on **OB-SOP-DCC-0007 — Communication & Notification Protocol (Rev.02)**, supplied 2026-09-30.

## 21. Revision History
| Version | Status | Change |
|---|---|---|
| 0.1 | Draft | Initial DCC Communication & Notification Operational Reference created from KB Owner-approved source input and gap analysis. |
