# Dataset Inventory

## Candidate Sources

| Source                                                   | Grain and time reference                                               | Status                                                       | What it can support                                                                     | Non-equivalence or gap                                                                                    |
| -------------------------------------------------------- | ---------------------------------------------------------------------- | ------------------------------------------------------------ | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| WHO Global Database on Blood Safety (GDBS)               | Country; latest reporting cycle is mainly 2023 in the 2026 summary     | Usable for national framing                                  | Donation rate, governance, screening, processing, and blood-system comparisons          | Cannot measure a named facility's emergency stock, compatibility, or time-to-transfusion                  |
| WHO SARA blood-transfusion module                        | Facility survey or census; observation window varies by implementation | Usable with explicit survey limits                           | Observed readiness, supply source, and prior-three-month interruption indicator         | Not continuous stock data; interruption duration and emergency response are not inherently captured       |
| WHO Harmonized Health Facility Assessment (HHFA)         | Facility; cross-sectional assessment with standardized modules         | Usable for measurement design and selected implementations   | Service availability, readiness, quality and safety, management, and finance indicators | Facility readiness on survey day is not proof of reliable blood during an obstetric emergency             |
| National blood-service stock, issue, and cold-chain logs | Facility or blood-centre; potentially daily or event-level             | Potentially usable after access and de-identification review | Stock interruption, component movement, expiry, testing, and distribution timing        | Often siloed; access, retention, unit definitions, and linkage to obstetric events require verification   |
| Maternal-health and referral records                     | Facility, referral, or district; episode-level where documented        | Limited until provenance and linkage are verified            | Obstetric haemorrhage episodes, referral timing, transfusion request and outcome fields | Completeness and timestamp quality may be poor; patient-level linkage creates privacy and governance risk |
| National donation-rate dashboards                        | Country or region; annual or periodic                                  | Limited for this pack's core question                        | Trend and equity framing                                                                | Donation volume is a supply proxy and cannot be substituted for facility-level availability               |

## Required Dataset Properties

- Facility identifier and facility level.
- Blood product type, units, compatibility or cross-match status where relevant.
- Observation date, stockout or interruption start and end, and reporting lag.
- Definition of availability, readiness, request, issue, transfusion, and referral.
- Obstetric case definition and denominator, if maternal outcomes are linked.
- Missingness, non-response, private-facility coverage, and data-quality checks.
- Data-access permission, de-identification method, and retention policy.
- Referral distance, transport mode, and timing only when lawfully collected and minimized.

## Classification Rule

No source is called usable for time-to-transfusion analysis unless it records timestamps or a defensible observation window for both the blood pathway and the relevant obstetric episode. A source may still be usable for national framing or facility-readiness measurement when those boundaries are stated.
