# Code D — Deceased Person Incident Management

**Document ID:** SEC-CODE-D-001  
**Title:** ระเบียบปฏิบัติมาตรการพบผู้เสียชีวิตในโครงการ  
**Source SOP:** OB-SOP-EP-0039  
**Version:** 1.1  
**Status:** Approved Reference  
**Owner:** KB Owner  
**Effective Date:** 2026-09-13  

---

## 1. Definition / Scope
**Code D = Deceased Person / พบผู้เสียชีวิต**.

Approved One Bangkok reference for management when a deceased person is found within the project area.

---

## 2. Source-Supported Detailed Swimlane Workflow

### Phase 1 — Initial Detection & Mozart Handling
1. **First Person / Security Guard** checks immediate safety and reports the incident to SOC or area Security Guard, including incident characteristics, location and condition/description of the person. Avoid touching or moving the body/person.
2. **SOC** opens the initial Mozart case as `Medical Assistance (Major - Ambulance)` because death has not yet been medically confirmed.
3. SOC directs Security Guard to cordon the area and use a field tent/cover for privacy; dispatches **EOT and Nurse/EMT** with equipment; informs **DCC, BMO and TMT** for support.

### Phase 2 — Safety & Condition Triage
4. **EOT / Nurse / EMT** assess scene safety before approaching, using appropriate emergency equipment/PPE.
5. If vital signs are present: provide immediate assistance under **Code M : Serious Case (OB-SOP-EP-0007)** and transport to hospital.
6. If no vital signs / person cannot be moved: preserve the scene, do not touch or move the body, maintain preliminary status as **Code M : Serious Case**, and report SOC immediately.

### Phase 3 — Escalation & External Coordination
7. SOC reports to **DCC** to request approval to coordinate external agencies.
8. After DCC approval, SOC contacts:
   - **Lumphini Police Station:** 02-255-5994 / 081-172-0239.
   - **Erawan Center / 1669**.
   - **Institute of Forensic Medicine, Police General Hospital:** 02-207-6108.
9. **TMT** facilitates traffic/access for police and forensic transport; Security Guard maintains strict cordon control.

### Phase 4 — Forensic Inspection & Code D Entry
10. **Police** formally control the incident scene and interview relevant persons.
11. **Forensic medical personnel/pathologist** inspect the body, conduct forensic examination at the scene and collect forensic evidence.
12. **Forensic Pathologist confirms death officially.**
13. After confirmation, **EOT informs SOC that the incident is Code D**.
14. **SOC opens a new Mozart case** using Event Type `Deceased Person Protocol (Code D)` and records the original case number as the **Reference Case Number**.
15. SOC checks and compiles relevant **CCTV** as evidence.

### Phase 5 — Body Relocation & Family Contact
16. **Police are responsible for contacting/notifying the deceased person's relatives.** Project staff do not directly notify relatives under this procedure.
17. Police and forensic personnel handle body relocation. **EOT and TMT** facilitate the route, service lift and discreet handover area to protect privacy and reduce unauthorized photography.

### Phase 6 — Cleanup, Reporting & Mozart Closure
18. **BMO / Cleaning Team** clean and disinfect the area only after police authorize release of the scene.
19. **BMO** prepares the incident report; **Safety** reviews the report and prevention recommendations.
20. **SOC** records the complete incident summary and closes the Mozart case (`Close Case`).
21. **DCC & PR** manage appropriate internal communication and prepare media information with management/legal coordination.
22. **IMT** conducts a **Post-Incident Review**. Source summary also states BMO communicates Mental Health Hotline **1323**.

---

## 3. Code D Authority / Handover
- **Official death confirmation:** Forensic Pathologist at the scene.
- **Code D system action:** EOT informs SOC after forensic confirmation; SOC opens/records the Code D case in Mozart.
- **Scene release / return of area:** Police authorize release of the scene.
- **Case closure:** SOC closes the Mozart case after the documented recovery/reporting sequence.

Do not reinterpret SOC's Mozart action as medical authority to determine death.

---

## 4. Notification & Escalation Matrix
1. Initial receipt: SOC informs/directs Security Guard, EOT, Nurse/EMT, DCC, BMO and TMT.
2. No vital signs: SOC reports DCC for external coordination approval.
3. After DCC approval: SOC contacts Lumphini Police, 1669 and Institute of Forensic Medicine, Police General Hospital.
4. After death confirmation / Code D: source summary states SOC updates Mozart and informs Safety, IMT and PR/Legal.

---

## 5. Scene Preservation / Evidence
- Do not touch or move the body before authorized forensic/police handling.
- Security Guard uses cordon line and a field tent/cover to preserve privacy and the scene.
- Police/forensic personnel are responsible for forensic evidence and the deceased person's belongings according to the supplied source summary.
- SOC checks, compiles and provides relevant CCTV records to authorities.

---

## 6. Mozart Workflow for Code D
- **Initial case:** `Medical Assistance (Major - Ambulance)` while condition/death is not yet officially confirmed.
- **After forensic confirmation:** new Event Type `Deceased Person Protocol (Code D)`.
- **Reference:** Code D case records the original case number as `Reference Case Number`.
- **Closure:** SOC records incident summary and performs `Close Case` after the documented closure conditions/process.

These Event Type names/actions are source-supported from the approved OB-SOP-EP-0039 summary. Do not infer additional Mozart fields or UI configuration.

---

## 7. Police / Forensic / Family Handover
- Police formally control the scene and investigation.
- Forensic personnel conduct examination and evidence collection; Forensic Pathologist confirms death.
- Police are responsible for contacting/notifying relatives.
- Body relocation is handled by police/forensic personnel with EOT/TMT logistical support.

---

## 8. Incident Report / Closure
Source summary identifies:
- Incident Report Form: `OB-FR-LW-0101`.
- Accident Investigation Form: `OB-FR-LW-0102`.
- Referenced SOP: `OB-SOP-LW-0001`.

Closure sequence described by the source: police forensic work completed and area released → body relocated → area cleaned → BMO/Safety report/review → SOC closes Mozart case → Post-Incident Review.

---

## 9. Media / Privacy
- Security Guard / EOT / TMT use screening/cordon measures during scene and body movement to protect privacy and prevent unauthorized photography.
- Source summary references PDPA and Criminal Procedure/penal-law context concerning deceased-person privacy/reputation; this KB does not independently verify legal interpretation/current applicability.
- **PR**, together with management and Legal, prepares/handles media information according to the supplied source summary.

---

## 10. Swimlane Structure
The source summary states that OB-SOP-EP-0039 pages 13 and 15 contain a detailed Swimlane with 11 lanes:
**First Person on Scene, SOC, CC, DCC, BMO, Safety, EOT, Security Guard, TMT, Police/Forensic, PR/Legal/IMT**.

The six-phase workflow above is the approved textual representation supplied from that source.

---

## 11. Remaining Knowledge Gaps
- **Specific radio channel number for Code D:** OB-SOP-EP-0039 source summary does not specify a dedicated radio channel; it emphasizes communication through SOC/DCC/control-center coordination and direct external-agency telephone contact.
- Exact original graphical Swimlane geometry/decision symbols are not reproduced in the supplied Markdown summary; the textual workflow and lane names are available.
- Any Mozart fields/UI configuration beyond the explicitly source-supported Event Types, Reference Case Number and Close Case actions remain unconfirmed.

---

## 12. AI Guardrails
- Forensic Pathologist confirmation is required before treating the incident as officially confirmed death under this source-supported workflow.
- Do not treat SOC/EOT/Security as medical authority to confirm death.
- Preserve the initial `Medical Assistance (Major - Ambulance)` → confirmed `Deceased Person Protocol (Code D)` distinction.
- Do not invent a Code D radio channel.
- Do not invent additional Mozart fields/UI configuration.
- Do not instruct project staff to notify relatives directly; the approved source assigns family notification to Police.
- Scene/body/evidence handling must remain aligned with Police/Forensic control described by the source.
- Legal references in the supplied summary are recorded as source-derived and are not independent legal verification.
- Missing source support = Knowledge Gap.

---

## 13. Sources
- `ระเบียบปฏิบัติมาตรการพบผู้เสียชีวิตในโครงการ.md` — approved 2026-09-13; high-level SOP overview.
- `ระเบียบปฏิบัติมาตรการพบผู้เสียชีวิตในโครงการ0.1.md` — approved 2026-09-13; detailed OB-SOP-EP-0039 workflow and Gap-resolution summary.

---

## 14. Change Log
- v1.0 — 2026-09-13 — Initial Approved Reference from high-level source summary.
- **v1.1 — 2026-09-13** — Added approved six-phase Detailed Swimlane Workflow, authority/handover, notification matrix, scene/evidence control, Mozart Code D workflow, family notification, reporting/closure and media/privacy information; retained dedicated radio channel and unsupported Mozart UI details as Knowledge Gaps.