---
document_id: SEC-SYSTEM-LOCATION-001
title: One Bangkok Location & Building Directory
version: 0.3
status: Reference
owner: KB Owner
scope: One Bangkok
source: User-provided location/building reference document, approved location-name image, and approved loading-point image
updated: 2026-09-06
---

# One Bangkok Location & Building Directory

## Purpose

Approved Knowledge Base reference for consistent location and building naming within One Bangkok. Use for incident communication, SOC case records, reports, emergency procedures, and location/check-in references.

## Approved Location Names

| Official / Source Name | Thai pronunciation / source note |
|---|---|
| Parade | — |
| The Storeys | เดอะสโตร์รี่ส์ |
| One Bangkok Forum | — |
| Tower 2 | ทาวเวอร์ ทู |
| Tower 3 | ทาวเวอร์ ทรี |
| Tower 4 | ทาวเวอร์ โฟร์ |
| Tower 5 | ทาวเวอร์ ไฟว์ |
| ONE89 wireless | — |
| EI8HTEEN SEVEN | — |
| The Ritz-Carlton Bangkok | — |
| Andaz One Bangkok | — |
| Pathom House | — |
| One Power (CUP) | — |
| Wireless House | พิพิธภัณฑ์บ้านวิทยุ |
| West Portal | เดิม เป็นอีสรรค์ |
| Boulevard | ถนนบูเลอวาร์ด |
| Park Lane | — |
| Arun McKinnon | อรุณแม็กคินนอน |
| EXAT | ทางด่วนพิเศษ |

## Loading Point Mapping

The following mappings are recorded exactly from the approved loading-point source image. Source labels are preserved even where naming differs from the Approved Location Names table.

| Loading Point | Building / Source Label |
|---|---|
| Loading 1 | Parade |
| Loading 2 | Signature |
| Loading 3 | Forum |
| Loading 4 | Tower 5 |
| Loading 5 | EI8HTEENSEVEN / Ritz-Carlton |
| Loading 6 | One 89 Wiress / Ritz-Carlton |
| Loading 7 | Andaz |
| Loading 8 | Tower 4 / Storeys |

### Loading Mapping Usage

When an incident or operational report identifies only a Loading Point, the AI may use the approved mapping above to identify the associated source-labeled building(s). For example, `Loading 4` maps to `Tower 5`.

Do not infer that a multi-building loading point belongs exclusively to one building. Loading 5, Loading 6, and Loading 8 explicitly contain multiple source labels and must remain multi-building mappings unless later approved information clarifies otherwise.

## Intended KB Usage

Emergency procedures, incident reports, SOC case records, training materials, and contact references should use the approved source spelling above where applicable. Preserve incident-specific floor, zone, common-area, Loading Point, or other location detail supplied with the event.

## AI Guardrails

1. Preserve the approved spelling and pronunciation/source note exactly as recorded from each supplied source unless the KB Owner approves a correction.
2. A blank pronunciation field means no pronunciation was confirmed in the approved source; do not invent one.
3. Do not silently normalize unusual source spelling or differences between sources. In particular, the loading-point image uses source labels such as `EI8HTEENSEVEN`, `One 89 Wiress`, `Forum`, `Andaz`, and `Storeys`; these are preserved as source-specific labels and are not automatically declared canonical aliases.
4. Do not invent additional buildings, check-in points, Loading Point mappings, aliases, pronunciation mappings, or location relationships.
5. This directory standardizes location references only; it does not change emergency SOP workflow, Declaration Authority, command structure, or response responsibilities.
6. When a location is used in an emergency case, preserve the exact incident-specific floor/zone/area/Loading Point details in addition to the approved building/location name.
7. If a Loading Point maps to more than one building, retain all buildings shown in the approved source and do not choose one without incident-specific evidence.
8. Additional names, aliases, corrections, pronunciation mappings, or Loading Point mappings require KB Owner review and approval.

## Remaining Knowledge Gaps

- KG-01: Exact location category/classification for each listed name is not fully confirmed.
- KG-02: Exact check-in point mappings beyond the approved Loading Point table are not yet supplied.
- KG-03: Pronunciations for entries marked `—` are not yet confirmed.
- KG-04: Relationship between source-specific loading labels (`Signature`, `Forum`, `Andaz`, `Storeys`, `One 89 Wiress`, `EI8HTEENSEVEN`) and canonical location names requires explicit confirmation before alias normalization.

## Change Log

- v0.1 — 2026-09-06 — Created from the approved user-provided location/building reference description.
- v0.2 — 2026-09-06 — Added approved individual One Bangkok location names and source-provided Thai pronunciation/notes.
- v0.3 — 2026-09-06 — Added approved Loading 1–8 to building/source-label mappings; preserved source spelling and multi-building relationships with AI guardrails.
