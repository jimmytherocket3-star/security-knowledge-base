---
document_id: SEC-SYSTEM-LOCATION-001
title: One Bangkok Location & Building Directory
version: 0.8
status: Reference
owner: KB Owner
scope: One Bangkok
source: User-provided location/building references, approved location-name image, loading-point image, Zoning Knowledge image, KB Owner-approved Parade ambulance pickup detail, and KB Owner-approved Zone color mapping
updated: 2026-09-08
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

## Approved Zone Color Mapping

KB Owner approved the following Zone ↔ color mapping on 2026-09-08:

| Zone | Approved Color / Area |
|---|---|
| **Zone 1** | สีฟ้า |
| **Zone 2** | สีเหลือง |
| **Zone 3** | สีส้ม |
| **Zone 4** | สีแดง |
| **Zone 5** | ทางด่วน |
| **Zone 6** | สีเขียว |

## Approved Building / Area → Zone Mapping

The following mappings are transcribed from the KB Owner-approved Zoning Knowledge schematic together with the approved Zone ↔ color mapping. These are stored explicitly so AI retrieval does not need access to the original image to answer building-to-Zone questions.

| Building / Area shown on source | Source color/area | Zone |
|---|---|---|
| **Tower 3** | สีฟ้า | **Zone 1** |
| **Tower 2** | สีฟ้า | **Zone 1** |
| **Parade** | สีฟ้า | **Zone 1** |
| **Frasers Suites** | สีฟ้า | **Zone 1** |
| **Parade Park** | สีฟ้า | **Zone 1** |
| **The Storeys** | สีเหลือง | **Zone 2** |
| **Tower 4** | สีเหลือง | **Zone 2** |
| **Pathom House** | สีเหลือง | **Zone 2** |
| **Andaz area** | สีเหลือง | **Zone 2** |
| **Wireless Park** | สีเหลือง | **Zone 2** |
| **Post 1928** | สีส้ม | **Zone 3** |
| **Tower 5** | สีส้ม | **Zone 3** |
| **ONE89 / The Ritz-Carlton area** | สีส้ม | **Zone 3** |
| **Eighteen Seven** | สีส้ม | **Zone 3** |
| **Forum** | สีแดง | **Zone 4** |
| **One Bangkok Tower / H4** | สีแดง | **Zone 4** |
| **One Bangkok Park** | สีเขียว | **Zone 6** |
| **EXAT / ทางด่วน** | ทางด่วน | **Zone 5** |

### Building-to-Zone Usage Rule

- For a building/area explicitly listed in the table above, AI may answer the Zone directly without re-interpreting the image.
- Preserve source labels and variants as shown; do not silently extend a mapping to a different building or alias unless separately approved.
- Zone 5 is recorded from the KB Owner's approved statement `ทางด่วน = Zone 5`; the schematic's EXAT / expressway context is the supported area reference.
- Areas or buildings not explicitly listed remain unsupported for direct Building → Zone mapping until approved.

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

## Parade Ambulance / Patient Pickup Reference

สำหรับการประสานรถพยาบาลเพื่อรับผู้บาดเจ็บหรือผู้ป่วยที่อาคาร **Parade** ให้ใช้อ้างอิงตำแหน่งตามข้อความที่ KB Owner อนุมัติดังนี้:

**Parade Loading 1, โค้ง 90 องศา, ประตูทางออกชั้น B1**

ข้อมูล `โค้ง 90 องศา` และ `ประตูทางออกชั้น B1` เป็นรายละเอียดตำแหน่งที่ KB Owner ให้และอนุมัติเมื่อ 2026-09-08

### Usage Guardrail

- ใช้ข้อมูลนี้สำหรับการอ้างอิงตำแหน่งรถพยาบาล/การรับผู้บาดเจ็บหรือผู้ป่วยที่ Parade
- ห้ามอนุมานว่ารายละเอียดเดียวกันใช้กับ Loading Point หรืออาคารอื่น
- ข้อมูลนี้ไม่ได้เปลี่ยน Code M workflow, medical decision authority, หรือ emergency command structure

## Intended KB Usage

Emergency procedures, incident reports, SOC case records, training materials, and contact references may use this document to identify an approved location name, its source-confirmed functional zoning, approved Zone/color and Building/Area→Zone mappings, an approved Loading Point relationship, and approved incident-specific location details where explicitly documented. Preserve incident-specific floor, zone, common-area, Loading Point, or other location detail supplied with the event.

## AI Guardrails

1. Preserve approved spelling and source terminology unless the KB Owner approves normalization or correction.
2. Do not invent pronunciations where the source does not provide one.
3. Do not silently merge source variants such as `One 89`, `ONE89 wireless`, `One 89 Wiress`, `Eighteen Seven`, and `EI8HTEEN SEVEN`; treat them as source variants pending explicit alias normalization.
4. Zoning classification may be used only where explicitly shown by the approved Zoning Knowledge source or approved mapping tables in this document.
5. For direct Building → Zone answers, use the explicit Approved Building / Area → Zone Mapping table above; do not require re-analysis of the source image.
6. The schematic map may support broad site context but not precise navigation or emergency routing except where separately confirmed by approved operational data such as the Parade ambulance/patient pickup reference.
7. Do not invent additional buildings, check-in points, Loading Point mappings, aliases, pronunciation mappings, Zone boundaries, or spatial relationships.
8. This directory does not change emergency SOP workflow, Declaration Authority, command structure, or response responsibilities.
9. If a Loading Point maps to multiple buildings, retain all source-shown buildings unless incident-specific evidence resolves the location.
10. New names, aliases, corrections, zoning changes, Zone/color mappings, Building/Area→Zone mappings, pronunciation mappings, or spatial/loading relationships require KB Owner approval.

## Remaining Knowledge Gaps

- KG-01: Canonical alias normalization across differing source spellings remains pending.
- KG-02: Exact check-in point mappings beyond Loading 1–8 are not yet supplied, except the approved Parade ambulance/patient pickup detail recorded above.
- KG-03: Pronunciations not explicitly supplied remain unconfirmed.
- KG-04: Exact entrances, pedestrian/vehicle routes, emergency access routes, and inter-building connectivity are not established by the schematic except where separately confirmed by approved operational data.
- KG-05: Building/Area→Zone mappings not explicitly listed in the approved mapping table remain unconfirmed.

## Change Log

- v0.8 — 2026-09-08 — Added explicit Building/Area → Zone mappings transcribed from the KB Owner-approved Zoning Knowledge schematic and approved Zone color mapping, including Tower 3 → Zone 1, so future retrieval does not require access to the original image.
- v0.7 — 2026-09-08 — Added KB Owner-approved Zone color mapping: Zone 1 = สีฟ้า, Zone 2 = สีเหลือง, Zone 3 = สีส้ม, Zone 4 = สีแดง, Zone 5 = ทางด่วน, Zone 6 = สีเขียว.
- v0.6 — 2026-09-08 — Corrected approved Parade ambulance/patient pickup wording to: `Parade Loading 1, โค้ง 90 องศา, ประตูทางออกชั้น B1`.
- v0.5 — 2026-09-08 — Added KB Owner-approved Parade ambulance/patient pickup reference.
- v0.4 — 2026-09-06 — Added approved Zoning Knowledge classifications and schematic spatial labels; added guardrails against inferring precise routes or distances.
- v0.3 — 2026-09-06 — Added approved Loading 1–8 mappings and multi-building guardrails.
- v0.2 — 2026-09-06 — Added approved individual location names and source-provided Thai pronunciation/notes.
- v0.1 — 2026-09-06 — Created from approved location/building reference description.
