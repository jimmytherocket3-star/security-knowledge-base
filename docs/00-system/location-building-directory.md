---
document_id: SEC-SYSTEM-LOCATION-001
title: One Bangkok Location & Building Directory
version: 0.9
status: Reference
owner: KB Owner
scope: One Bangkok
source: User-provided location/building references, approved location-name image, loading-point image, Zoning Knowledge image, KB Owner-approved ambulance/patient pickup details, and KB Owner-approved Zone color mapping
updated: 2026-09-10
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

| Zone | Approved Color / Area |
|---|---|
| **Zone 1** | สีฟ้า |
| **Zone 2** | สีเหลือง |
| **Zone 3** | สีส้ม |
| **Zone 4** | สีแดง |
| **Zone 5** | ทางด่วน |
| **Zone 6** | สีเขียว |

## Approved Building / Area → Zone Mapping

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
- For a building/area explicitly listed above, AI may answer the Zone directly.
- Preserve source labels/variants; do not silently extend mappings.
- Unlisted Building/Area → Zone mappings remain unsupported until approved.

## Zoning Map — Confirmed Spatial Labels

Embassy Road; EXAT Connection; Wireless Road; One Bangkok Boulevard; One Bangkok Park; Parade Park; Rama4 Road; MRT Connection; Wireless Park; Wireless House; Pathom House; One Power; Post 1928; Tower 2; Tower 3; Tower 4; Tower 5; Forum; Parade; The Storeys; ONE89 / The Ritz-Carlton area; Eighteen Seven; Andaz area; Frasers Suites; One Bangkok Tower / H4.

### Spatial-Relationship Guardrail
The zoning diagram is schematic. Do not infer precise distances, entrances, travel routes, emergency access routes, floor connectivity, or shortest paths unless separately confirmed by approved operational data.

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

## Ambulance / Patient Pickup References

### Parade
For ambulance coordination to receive an injured person or patient at **Parade**, use:

**Parade Loading 1, โค้ง 90 องศา, ประตูทางออกชั้น B1**

### The Storeys
For ambulance/patient pickup location reference at **The Storeys**, the KB Owner approved the following three locations on 2026-09-10:

1. **โค้ง 90° — ชั้น B1**
2. **Loading 8 — ชั้น B1**
3. **Drop-off The Storeys — ชั้น G**

### Pickup Reference Guardrails
- The three The Storeys locations are approved as patient/ambulance pickup location references.
- No Primary/Secondary priority or condition-of-use has been assigned among the three locations; do not invent one.
- Do not infer that these pickup details apply to other buildings or Loading Points.
- These location references do not change Code M workflow, medical decision authority, emergency command structure, or vehicle routing beyond the explicitly approved location facts.

## Intended KB Usage

Emergency procedures, incident reports, SOC case records, training materials, and contact references may use this document to identify approved location names, source-confirmed functional zoning, approved Zone/color and Building/Area→Zone mappings, approved Loading Point relationships, and approved patient/ambulance pickup locations where explicitly documented.

## AI Guardrails

1. Preserve approved spelling and source terminology unless the KB Owner approves normalization or correction.
2. Do not invent pronunciations where the source does not provide one.
3. Do not silently merge source variants such as `One 89`, `ONE89 wireless`, `One 89 Wiress`, `Eighteen Seven`, and `EI8HTEEN SEVEN`.
4. Zoning classification may be used only where explicitly approved.
5. For direct Building → Zone answers, use the explicit mapping table.
6. The schematic map may support broad site context but not precise navigation/emergency routing except separately approved operational data.
7. Do not invent additional buildings, check-in points, Loading Point mappings, aliases, pronunciations, Zone boundaries, or spatial relationships.
8. This directory does not change emergency SOP workflow, Declaration Authority, command structure, or response responsibilities.
9. If a Loading Point maps to multiple buildings, retain all source-shown buildings unless incident-specific evidence resolves the location.
10. New names, aliases, corrections, zoning changes, mappings, pronunciations, or spatial/loading/pickup relationships require KB Owner approval.

## Remaining Knowledge Gaps

- KG-01: Canonical alias normalization across differing source spellings remains pending.
- KG-02: Exact check-in/patient pickup mappings beyond Loading 1–8 are not supplied except the approved Parade and The Storeys pickup references above.
- KG-03: Pronunciations not explicitly supplied remain unconfirmed.
- KG-04: Exact entrances, pedestrian/vehicle routes, emergency access routes, and inter-building connectivity are not established except where separately confirmed by approved operational data.
- KG-05: Building/Area→Zone mappings not explicitly listed remain unconfirmed.
- KG-06: The Storeys pickup-point priority/selection criteria (Primary/Secondary or condition-of-use) remain unconfirmed.

## Change Log

- v0.9 — 2026-09-10 — Added KB Owner-approved The Storeys ambulance/patient pickup references: โค้ง 90° ชั้น B1; Loading 8 ชั้น B1; Drop-off The Storeys ชั้น G. No priority or condition-of-use inferred.
- v0.8 — 2026-09-08 — Added explicit Building/Area → Zone mappings from approved Zoning Knowledge.
- v0.7 — 2026-09-08 — Added approved Zone color mapping.
- v0.6 — 2026-09-08 — Corrected Parade ambulance/patient pickup wording.
- v0.5 — 2026-09-08 — Added approved Parade ambulance/patient pickup reference.
- v0.4 — 2026-09-06 — Added approved Zoning Knowledge classifications and schematic spatial labels.
- v0.3 — 2026-09-06 — Added approved Loading 1–8 mappings.
- v0.2 — 2026-09-06 — Added approved individual location names and source-provided Thai pronunciation/notes.
- v0.1 — 2026-09-06 — Created from approved location/building reference description.
