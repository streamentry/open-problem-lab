# Dataset Inventory

## Candidate Sources

| Source                                                                  | Grain                                                   | Status                                                | Use and boundary                                                                                         |
| ----------------------------------------------------------------------- | ------------------------------------------------------- | ----------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| Global E-waste Monitor 2024                                             | Country and regional material-flow accounting           | Usable for burden and formal-collection framing       | Denominator and policy context; not a cluster or exposure dataset                                        |
| WHO Children and Digital Dumpsites                                      | Global evidence synthesis and risk-population estimates | Usable for pathway framing                            | Burden and vulnerable-group context; not local prevalence                                                |
| ILO E-waste and employment around the world                             | Global value-chain and employment framing               | Usable with local validation                          | Work-structure hypotheses; not a local worker census                                                     |
| National customs, permits, and extended-producer-responsibility records | Country, facility, shipment, or product category        | Potentially usable after provenance review            | Candidate flow and formal-facility denominator; likely misses informal activity                          |
| Environmental sampling from soil, dust, air, water, food, or blood      | Site, household, worker, or school sample               | Usable only with method and ethics review             | Exposure measurement; requires sampling frame, analyte, detection limits, and chain of custody           |
| OpenStreetMap, satellite imagery, and land-use layers                   | Variable spatial and temporal grain                     | Limited for candidate discovery                       | May identify access, land use, smoke, or settlement context; cannot prove e-waste processing or exposure |
| News, NGO, and crowdsourced site lists                                  | Place or narrative report                               | Limited or rejected unless independently corroborated | Discovery leads only; not a prevalence or enforcement list                                               |

## Required Dataset Properties

- Processing activity and date, not merely a waste or facility label.
- Geographic grain, coordinate uncertainty, and whether the site is active during the observation period.
- Material category and processing method, including dismantling, burning, acid leaching, repair, resale, or mixed activity.
- Sampling frame, analytes, detection limits, quality controls, chain of custody, and ethical approvals for human data.
- Worker, resident, child, and pregnancy status only when lawfully collected, minimized, and necessary.
- Missingness, under-reporting, seasonal activity, transboundary flows, and displacement after enforcement.
- License, reuse conditions, and version or access date.

## Rejection Rule

Reject a source for canonical exposure or allocation analysis when it cannot distinguish e-waste processing from general waste, lacks a verifiable method or date, has unknown geographic grain, or turns proximity into exposure without measurements. A rejected source may remain listed as a discovery lead.
