---
document_id: SEC-CODE-M-001
title: Code M — Medical Emergency Operational Reference
version: 1.0
status: Approved Reference
owner: KB Owner
scope: Medical Emergency / Operational Procedure Reference
effective_date: 2026-09-17
updated: 2026-09-17
---

# Code M — Medical Emergency Operational Reference

## 1. Purpose and Source Boundary

This document records the Code M operational knowledge explicitly supplied and approved by the KB Owner during the Skills Hunter 2.0 Knowledge Gap closure on 2026-09-17.

It is an **Approved Reference**, not authority to invent missing medical, command, system, or routing rules. Where this document states a Knowledge Gap, AI must preserve that gap and must not fill it from incident examples, another emergency code, external knowledge, or assumptions.

Hospital transport conditions and ambulance/patient pickup locations remain governed by their routed source documents. This document cross-references those sources rather than replacing them.

## 2. Code M Definition and Trigger Boundary

Code M = **Medical Emergency**.

The available flowchart begins at **“พบเหตุ / รับแจ้ง”** (incident found / notification received).

The KB does **not** currently establish:
- a minimum severity or triage threshold for entering Code M;
- whether every first-aid case is Code M; or
- which role or unit has authority to declare/confirm Code M.

UCEP criteria described in patient-transfer material relate to hospital transfer and must **not** be treated as the Code M trigger unless separately approved.

## 3. Initial Response

When a medical incident is found or reported:

- **SS (Security Staff)** provides initial assistance and notifies FCC.
- **SOC** notifies the SOC Supervisor and opens a case in the system.
- SS / field security, Building Management, EOT, and SOC use **Emergency / EMER 1** so relevant units can receive incident information in real time and reduce multi-step message distortion.

The source does not identify the specific authority that orders the switch to EMER 1 or the authority/process for returning to the normal radio channel after the incident.

## 4. Roles and Responsibilities

### SS / Security Staff

- Find or receive the incident report.
- Provide initial assistance.
- Notify FCC.
- For a patient who can move, escort the patient according to the patient-movement process.
- For a patient who cannot move, remain with the patient and help control the area until EOT arrives.
- Support EOT during patient movement.
- Report the outcome to FCC and withdraw when the applicable flow is complete.

### FCC

The Code M source supplied during gap closure attributes these functions to **FCC**:

- Receive notification from SS.
- Coordinate notification to Building Management and SOC.
- Call EOT for support when the patient cannot move.
- Notify the nurse assigned to the medical room.
- Monitor the situation and receive operational reports from SS.
- Participate in EMER 1 incident communications.

**Terminology conflict guardrail:** the Code M source labels FCC as `Facility Control Center`, while the current canonical terminology source defines FCC as `Fire Command Center`. This disagreement is registered in `docs/00-system/source-conflict-register.md`. Do not select a winner or silently change the canonical expansion. The operational actions above are preserved as source-attributed Code M actions pending reconciliation.

### EOT — Emergency Operation Team

- Receive emergency notification from FCC or SOC.
- Support the incident area and patient care / area control together with SS.
- Support patient movement to the medical room.
- Support First Aid when Building Management cannot provide initial First Aid.
- Jointly confirm hospital-transfer information with the registered nurse.

### Registered Nurse

- Receive notification from FCC.
- Receive the patient after delivery to the medical room.
- Jointly confirm external-hospital transfer information with EOT.

For the registered nurse assigned to the Retail medical room, the supplied source additionally states that the nurse:
- checks the patient's treatment entitlement through the website;
- considers and confirms the destination hospital with Kluaynamthai Hospital personnel;
- accompanies the patient to the destination hospital to clarify information;
- may consider Kluaynamthai Hospital first if entitlement checking is delayed; and
- coordinates with the destination government hospital when the patient requests that service.

### EMT — Kluaynamthai Hospital

In the supplied UCEP transfer context, the EMT from Kluaynamthai Hospital coordinates through the Bangkok Emergency Medical Service Center (Erawan Center).

### DCC

**Knowledge Gap:** the supplied Code M procedure does not establish DCC's role or responsibility.

## 5. Patient Movement

### 5.1 Patient can move independently

1. SS provides initial assistance.
2. SS notifies FCC.
3. SS escorts the patient to the medical room.
4. On arrival, the patient is handed over to the registered nurse.
5. SS reports to FCC and withdraws.
6. SOC summarizes and closes the case according to the applicable closure flow.

For Office Tenant cases, the supplied source states:
- **Tower 4:** medical room, Ground Floor (G).
- **Tower 3:** Floor 5.
- Building Management leads/coordinates and cares for the patient within the office-building scope.

The supplied source states: **Do not send the patient to a Retail shop area in any case.**

### 5.2 Patient cannot move independently

1. SS or SOC coordinates notification through FCC/SOC so EOT can support the incident.
2. SS cares for the patient and controls the incident area until EOT arrives.
3. EOT supports the patient and movement.
4. SS supports EOT in moving the patient to the medical room.

For internal staff requiring hospital transfer, the supplied material identifies B1 as the principal ambulance area and gives examples including C3A / Loading 6 and C3B / Loading 5. Treat these as source-stated examples only. For current approved pickup/drop-off locations, route to the dedicated location/pickup references.

### 5.3 Severe patient / direct medical access

**Knowledge Gap:** no approved Code M rule currently establishes when an external ambulance or medical team should access the patient directly at the incident location rather than moving the patient to the medical room.

**Knowledge Gap:** no approved criterion currently establishes when a patient may bypass the internal medical room and be transferred directly from the incident location to an external hospital.

## 6. External Hospital Transfer

External-hospital transfer information must be confirmed by **both the registered nurse and EOT** according to the supplied Code M material.

For UCEP, the supplied material identifies an emergency-transfer context involving the project emergency vehicle, Kluaynamthai Hospital or a nearby hospital, and coordination by the Kluaynamthai Hospital EMT through the Erawan Center.

Do not use UCEP criteria as Code M declaration criteria.

For current hospital groups, distance bands, transport-charge conditions, and approved hospital transport information, route to:

`docs/00-system/hospital-transport-reference.md`

For current approved ambulance/patient pickup locations, route to:

- `docs/00-system/location-building-directory.md`
- `docs/08-reference/one-bangkok-ambulance-pickup-dropoff-points.md` where required by `KB-INDEX.md`

Do not infer a preferred pickup point, access route, or hospital from this Code M document.

## 7. Communication and Escalation

### EMER 1

The supplied Code M material requires the following groups to use Emergency / EMER 1 during the incident:
- SS / field security;
- Building Management;
- EOT; and
- SOC.

Purpose: common real-time incident awareness and reduction of message distortion / “Chinese Whisper.”

**Knowledge Gap:** authority to order the switch to EMER 1 is not identified.

**Knowledge Gap:** authority/process to return to the normal radio channel is not identified.

### Notifications established by the supplied source

- **SOC Supervisor:** SOC notifies immediately when SOC finds or receives notification of the medical emergency.
- **Building Management:** FCC notifies Building Management at the initial stage after receiving SS notification. For Office Tenant cases, SS coordinates Building Management so Building Management can lead/coordinate patient care within the office-building scope.

### Notifications not established by the supplied Code M procedure

The supplied Code M procedure does not establish a general incident notification rule for:
- DCC;
- EMT as a field radio notification recipient;
- Traffic; or
- Forward Standby.

Do not infer those notification requirements from incident logs alone.

## 8. Termination and Case Closure

### Patient declines assistance

1. SS withdraws from the area.
2. SS reports to FCC.
3. SOC summarizes and closes the case.

### Patient chooses / requires movement to the medical room

1. Patient is delivered to the medical room.
2. Patient is handed over to the registered nurse.
3. SS reports to FCC and withdraws.
4. SOC summarizes and closes the case.

The flowchart establishes SOC as the role performing **“สรุปเคส”** and **“ปิดเคส”**. It does not establish a separate approval authority for closure.

## 9. Remaining Knowledge Gaps

The following items remain explicitly unresolved:

1. Code M trigger / severity / triage criteria.
2. Code M declaration or confirmation authority.
3. DCC role in the Code M procedure.
4. Severe-patient direct medical/ambulance access criteria and process.
5. Criteria for direct transfer from incident location to external hospital without first using the medical room.
6. Formal Case Closure Authority, if separate approval is required beyond SOC performing the closure step.
7. Termination/closure workflow after successful external-hospital transfer or when the patient's condition improves without transfer.
8. Mandatory Mozart fields, attachments, evidence, approvals, and Code M closure requirements.
9. Authority to order units to switch to EMER 1.
10. Authority/process to return units to the normal radio channel after the incident.

## 10. AI Guardrails

- Do not infer a Code M trigger from UCEP criteria.
- Do not infer declaration authority from the fact that a nurse and EOT confirm hospital-transfer information.
- Do not infer DCC, Traffic, Forward Standby, or EMT notification requirements from example incident logs.
- Do not infer direct-to-hospital criteria or direct ambulance access to an incident location.
- Do not invent Mozart mandatory fields or closure evidence.
- Do not infer radio switching or return-to-normal authority.
- Do not resolve the FCC expansion disagreement; follow the registered conflict rule.
- Route hospital transport and ambulance/pickup-location questions to their dedicated sources.

## 11. Change Log

| Version | Date | Change | Approved By |
|---|---|---|---|
| 1.0 | 2026-09-17 | Created Code M operational reference from KB Owner-approved Knowledge Gap closure; preserved unresolved operational gaps and source boundaries. | KB Owner |
