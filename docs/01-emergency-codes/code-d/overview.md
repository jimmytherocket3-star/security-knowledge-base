# Code D — Deceased Person Incident Management

**Document ID:** SEC-CODE-D-001  
**Title:** ระเบียบปฏิบัติมาตรการพบผู้เสียชีวิตในโครงการ  
**Source SOP:** OB-SOP-EP-0039  
**Version:** 1.2  
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
8. After DCC approval, SOC contacts **Lumphini Police Station 02-255-5994 / 081-172-0239**, **Erawan Center 1669**, and **Institute of Forensic Medicine, Police General Hospital 02-207-6108**.
9. **TMT** facilitates traffic/access for police and forensic transport; Security Guard maintains strict cordon control.

### Phase 4 — Forensic Inspection & Code D Entry
10. **Police** formally control the incident scene and interview relevant persons.
11. **Forensic medical personnel/pathologist** inspect the body, conduct forensic examination at the scene and collect forensic evidence.
12. **Forensic Pathologist confirms death officially.**
13. After confirmation, **EOT informs SOC that the incident is Code D**.
14. **SOC opens a new Mozart case** using Event Type `Deceased Person Protocol (Code D)` and records the original case number as the **Reference Case Number**.
15. SOC checks and compiles relevant **CCTV** as evidence.

### Phase 5 — Body Relocation & Family Contact
16. **Police are responsible for contacting/notifying the deceased person's relatives.**
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

SOC's Mozart action is not medical authority to determine death.

---

## 4. Notification & Escalation Matrix
1. Initial receipt: SOC informs/directs Security Guard, EOT, Nurse/EMT, DCC, BMO and TMT.
2. No vital signs: SOC reports DCC for external coordination approval.
3. After DCC approval: SOC contacts Lumphini Police, 1669 and Institute of Forensic Medicine, Police General Hospital.
4. After death confirmation / Code D: source summary states SOC updates Mozart and informs Safety, IMT and PR/Legal.

---

## 5. Communication — Source-Supported Boundary
OB-SOP-EP-0039 **does not specify a dedicated Code D radio channel number**.

The source identifies incident communication through **SOC or Contact Centre (CC)** and direct external-agency telephone contacts:
- Lumphini Police Station: `02-255-5994` / `081-172-0239`.
- Erawan Center: `1669`.
- Institute of Forensic Medicine, Police General Hospital: `02-207-6108`.

A Code D-specific Radio Channel Plan is therefore **not established by this SOP**. Do not infer EMER1 or any other channel.

---

## 6. Scene Preservation / Evidence
- Do not touch or move the body before authorized forensic/police handling.
- Security Guard uses cordon line and a field tent/cover to preserve privacy and the scene.
- Police/forensic personnel are responsible for forensic evidence and the deceased person's belongings according to the supplied source summary.
- SOC checks, compiles and provides relevant CCTV records to authorities.

---

## 7. Mozart Workflow for Code D
The SOP confirms three principal Mozart actions:
1. **Initial Case:** Event Type = `Medical Assistance (Major - Ambulance)`.
2. **Confirmed Code D:** open a new case with Event Type = `Deceased Person Protocol (Code D)` and enter the original emergency-medical case as the **Reference Case Number**.
3. **Case Closure:** summarize the incident and perform **Close Case**.

### Mozart Knowledge Gap Boundary
The SOP does **not** show/confirm:
- UI screenshots / exact screen layout.
- Complete field schema.
- Mandatory vs optional fields.
- Exact location-coordinate fields.
- Attachment fields for images/forensic documents.
- System approval-button/workflow configuration.

Do not infer these from the three confirmed Mozart actions.

---

## 8. Police / Forensic / Family Handover
- Police formally control the scene and investigation.
- Forensic personnel conduct examination and evidence collection; Forensic Pathologist confirms death.
- Police are responsible for contacting/notifying relatives.
- Body relocation is handled by police/forensic personnel with EOT/TMT logistical support.

---

## 9. Incident Report / Closure
Source summary identifies:
- Incident Report Form: `OB-FR-LW-0101`.
- Accident Investigation Form: `OB-FR-LW-0102`.
- Referenced SOP: `OB-SOP-LW-0001`.

Closure sequence: police forensic work completed and area released → body relocated → area cleaned → BMO/Safety report/review → SOC closes Mozart case → Post-Incident Review.

---

## 10. Media / Privacy
- Security Guard / EOT / TMT use screening/cordon measures during scene and body movement to protect privacy and prevent unauthorized photography.
- Source summary references PDPA and legal context concerning deceased-person privacy/reputation; this KB does not independently verify legal interpretation/current applicability.
- **PR**, together with management and Legal, prepares/handles media information according to the supplied source summary.

---

## 11. Swimlane Graphics & Decision Symbols — Source-Supported
The approved source describes the graphical Swimlane on SOP pages 13 and 15 as follows.

### Start / End Nodes
- **Green circle:** initial Start node for First Person.
- **Red circle:** Role Start for the beginning of each department/role's action.
- **Green circle with dark border:** End / Clear node when the area-return and case-closure process is complete.

### Decision Diamonds
- **Yellow Diamond:** general decision/assessment points, including `Safe?` and `Has sign of life? / Conscious?`.
- **Red Diamond:** critical decision point for forensic confirmation of death, represented as `Declared dead by Forensic Pathologist? / Dead?`, which transitions the process into formal Code D handling.

### Process Rectangles
- **White/gray box with black border:** normal operational activity/task.
- **Orange/red-border box:** critical activity such as emergency escalation and Mozart recording.

### Swimlanes / Role Badges
The supplied source lists the lanes/roles as:
**First Person, DCC, CC, SOC, EOT, Police, TMT, BMO Estate, FMC, BMO Component, Nurse/EMT, Reception/Concierge, Retail Operation**.

This graphical description supplements the six-phase textual workflow. Preserve the source terminology rather than reconciling or replacing role labels without additional approved evidence.

---

## 12. Remaining Knowledge Gaps
- **Dedicated Code D Radio Channel:** not specified in OB-SOP-EP-0039. This is a confirmed absence from the supplied SOP, not permission to infer another emergency channel.
- **Mozart UI / Mandatory Fields / Attachment / Approval Configuration:** not shown or confirmed by the supplied SOP.
- Any graphical details of the original Swimlane beyond the source-supported nodes, colors, decision diamonds, process rectangles and listed role lanes above remain unsupported unless additional source evidence is supplied.

---

## 13. AI Guardrails
- Forensic Pathologist confirmation is required before treating the incident as officially confirmed death under this source-supported workflow.
- Do not treat SOC/EOT/Security as medical authority to confirm death.
- Preserve the initial `Medical Assistance (Major - Ambulance)` → confirmed `Deceased Person Protocol (Code D)` distinction.
- **Never invent a Code D radio channel.** The SOP does not specify one.
- Do not invent Mozart UI, mandatory fields, attachment fields or approval workflow.
- Do not instruct project staff to notify relatives directly; the approved source assigns family notification to Police.
- Preserve source Swimlane terminology and symbol descriptions without silently reconciling them with other documents.
- Missing source support = Knowledge Gap.

---

## 14. Sources
- `ระเบียบปฏิบัติมาตรการพบผู้เสียชีวิตในโครงการ.md` — approved 2026-09-13; high-level SOP overview.
- `ระเบียบปฏิบัติมาตรการพบผู้เสียชีวิตในโครงการ0.1.md` — approved 2026-09-13; detailed workflow and Gap-resolution summary.
- `ระเบียบปฏิบัติมาตรการพบผู้เสียชีวิตในโครงการ0.2.md` — approved 2026-09-13; Radio Channel absence, Mozart evidence boundary and Swimlane graphic/symbol details.

---

## 15. Change Log
- v1.0 — 2026-09-13 — Initial Approved Reference from high-level source summary.
- v1.1 — 2026-09-13 — Added six-phase Detailed Swimlane Workflow, authority/handover, notification matrix, scene/evidence control, Mozart workflow, family notification, reporting/closure and media/privacy information.
- **v1.2 — 2026-09-13** — Confirmed no dedicated Code D radio channel is specified by OB-SOP-EP-0039; refined Mozart Knowledge Gap to UI/Mandatory Fields/Attachment/Approval configuration; added source-supported Swimlane graphical nodes, decision symbols, process boxes and role lanes.