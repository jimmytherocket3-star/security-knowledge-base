---
document_id: SEC-SYSTEM-LOCATION-001
title: One Bangkok Location & Building Directory
version: 0.4
status: Reference
owner: KB Owner
scope: One Bangkok
source: User-provided location/building references, approved location-name image, loading-point image, and Zoning Knowledge image
updated: 2026-09-06
---

# One Bangkok Location & Building Directory

## Purpose

Approved Knowledge Base reference for consistent location, building, loading-point, and zoning references within One Bangkok. Use for incident communication, SOC case records, reports, emergency procedures, and location/check-in references.

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

## Zoning Knowledge

The approved Zoning Knowledge source explicitly groups the following names by functional type. Source terminology is preserved.

### Retail

- Parade — พาเหรด
- The Storeys — เดอะ สตอรี่ส์
- Post1928 — โพสต์ ในพื้นที่เวนดิ้ง
- Forum

### Office

- One Bangkok Tower
- One Bangkok Tower 2
- One Bangkok Tower 3
- One Bangkok Tower 4
- One Bangkok Tower 5

### Hotel

- Frasers Suites
- The Ritz-Carlton Bangkok
- Andaz One Bangkok
- H2B Hotel

### Residence

- One 89
- Eighteen Seven

## Zoning Map — Confirmed Spatial Labels

The source map additionally shows the following labeled places or connections within the One Bangkok site context:

- Embassy Road
- EXAT Connection
- Wireless Road
- One Bangkok Boulevard
- One Bangkok Park
- Parade Park
- Rama4 Road
- MRT Connection
- Wireless Park
- Wireless House
- Pathom House
- One Power
- Post 1928
- Tower 2, Tower 3, Tower 4, Tower 5
- Forum
- Parade
- The Storeys
- ONE89 / The Ritz-Carlton area
- Eighteen Seven
- Andaz area
- Frasers Suites
- One Bangkok Tower / H4

### Spatial-Relationship Guardrail

The zoning diagram is a schematic reference. AI may use it to understand source-shown zoning and broad adjacency/context, but must not infer precise distances, entrances, travel routes, emergency access routes, floor connectivity, or shortest paths unless separately confirmed by approved operational data.

## Loading Point Mapping

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

When an incident or operational report identifies only a Loading Point, AI may use the approved mapping to identify the associated source-labeled building(s). Multi-building mappings must remain multi-building unless incident-specific evidence identifies the relevant building.

## Intended KB Usage

Emergency procedures, incident reports, SOC case records, training materials, and contact references may use this document to identify an approved location name, its source-confirmed functional zoning, and an approved Loading Point relationship. Preserve incident-specific floor, zone, common-area, Loading Point, or other location detail supplied with the event.

## AI Guardrails

1. Preserve approved spelling and source terminology unless the KB Owner approves normalization or correction.
2. Do not invent pronunciations where the source does not provide one.
3. Do not silently merge source variants such as `One 89`, `ONE89 wireless`, `One 89 Wiress`, `Eighteen Seven`, and `EI8HTEEN SEVEN`; treat them as source variants pending explicit alias normalization.
4. Zoning classification may be used only where explicitly shown by the approved Zoning Knowledge source.
5. The schematic map may support broad site context, but not precise navigation or emergency routing.
6. Do not invent additional buildings, check-in points, Loading Point mappings, aliases, pronunciation mappings, or spatial relationships.
7. This directory does not change emergency SOP workflow, Declaration Authority, command structure, or response responsibilities.
8. If a Loading Point maps to multiple buildings, retain all source-shown buildings unless incident-specific evidence resolves the location.
9. New names, aliases, corrections, zoning changes, pronunciation mappings, or spatial/loading relationships require KB Owner approval.

## Remaining Knowledge Gaps

- KG-01: Canonical alias normalization across differing source spellings remains pending.
- KG-02: Exact check-in point mappings beyond Loading 1–8 are not yet supplied.
- KG-03: Pronunciations not explicitly supplied remain unconfirmed.
- KG-04: Exact entrances, pedestrian/vehicle routes, emergency access routes, and inter-building connectivity are not established by this schematic.
- KG-05: Zoning/classification of map labels not included in the source's Retail/Office/Hotel/Residence lists remains unconfirmed.

## Change Log

- v0.1 — 2026-09-06 — Created from approved location/building reference description.
- v0.2 — 2026-09-06 — Added approved individual location names and source-provided Thai pronunciation/notes.
- v0.3 — 2026-09-06 — Added approved Loading 1–8 mappings and multi-building guardrails.
- v0.4 — 2026-09-06 — Added approved Zoning Knowledge classifications and schematic spatial labels; added guardrails against inferring precise routes or distances.
