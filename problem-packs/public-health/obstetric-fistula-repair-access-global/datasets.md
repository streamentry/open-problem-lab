# Dataset Inventory

## Candidate Sources

| Source                                                                 | Grain                                     | Current status                                 | Use                                                                                                             |
| ---------------------------------------------------------------------- | ----------------------------------------- | ---------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| UNFPA Campaign to End Fistula records                                  | Country, program, variable                | Limited but central                            | Campaign footprint, supported repairs, program priorities, and policy framing                                   |
| BMJ Global Health 2025 prevalence estimates                            | Country, regional, global                 | Usable for burden framing                      | Current modelled prevalence baseline for 55 low- and middle-income countries                                    |
| DHS fistula module and women's questionnaire data                      | Individual, cluster, national             | Limited and survey-dependent                   | Awareness and self-reported symptom measures where the module was fielded                                       |
| National fistula program or repair-center registries                   | Facility, program, country                | Limited and fragmented                         | Repair volume, follow-up, and case-finding clues when provenance is documented                                  |
| Surgical outcome studies and repair cohorts                            | Facility, study cohort                    | Limited for access                             | Repair success, continence, recurrence, and follow-up definitions                                               |
| EmONC needs assessments and facility readiness data                    | Facility, district, national              | Limited but relevant                           | Prevention context for obstructed labour management and emergency obstetric capacity                            |
| Referral-delay, transport, and caesarean-access data                   | District to facility, variable            | Limited                                        | Mechanism evidence for incident fistula prevention failures                                                     |
| Population denominators and admin boundaries                           | District, gridded, national               | Usable but version-sensitive                   | Rate construction, catchment comparison, and uncertainty documentation                                          |
| DHS Analytical Studies No. 17 and standardized fistula module guidance | Individual, survey, country               | Limited; instrument-dependent                  | Self-reported leakage and treatment-seeking proxy; usable only after questionnaire and denominator audit        |
| WHO EmOC monitoring handbook and signal-function tools                 | Facility, district, national              | Limited; indicator framework                   | Prevention-capacity context for actual emergency-care availability and use; not fistula incidence               |
| Bangladesh national fistula annual report                              | Country, division, facility network, year | Usable for one-country program-output analysis | Identified cases, admissions, surgeries, successful repairs, diagnostic mix, and reintegration program activity |

## Required Properties

- Measurement family: prevalent untreated fistula, incident fistula, repair output, repair outcome, symptom self-report, or prevention-capacity proxy.
- Numerator definition: confirmed diagnosis, self-report, repair event, successful closure, continence outcome, recurrence, or inoperable case.
- Denominator definition: women of reproductive age, all women ages 15-64, births, deliveries, facility deliveries, treated patients, or catchment population.
- Time reference and whether measurement is lifetime, point prevalence, annual incidence, program year, or follow-up interval.
- Geographic grain and whether sub-national identifiers survive public release.
- Case-finding method and likely missingness from stigma, isolation, affordability, and distance.
- Repair outcome definition, follow-up window, and loss-to-follow-up handling.
- Whether the source can distinguish accumulated backlog from continuing incident prevention failure.

## Rejection Rule

A source is rejected for allocation ranking if it cannot identify the measurement family, denominator, time reference, and case-finding method. Self-reported symptoms may be used as a measurement clue, not as confirmed obstetric fistula prevalence. Repair counts without recurrence, referral, and follow-up context may be used as capacity clues, not as proof that need is falling.

## Classification Notes For This Task

- **Usable for bounded use:** the BMJ modelled estimate for global or specified-country burden framing; population denominators and boundary files for rate construction; the Bangladesh annual report for a Bangladesh-only program-output and case-mix review when its reporting completeness is stated.
- **Limited and conditionally usable:** UNFPA campaign records, DHS fistula modules and microdata, national repair-centre registries, surgical cohorts, WHO EmOC indicators, and referral-delay data. Each can answer a defined sub-question, but none alone identifies the untreated backlog and none should be ranked across countries without denominator, time, instrument, and coverage checks.
- **Rejected for direct allocation ranking:** any self-reported symptom estimate without the exact instrument and eligibility filter; any repair count without case definition and follow-up window; any EmOC readiness score treated as proof of fistula incidence; and any global campaign total treated as a country-comparable service denominator.

The minimum replicable classification record for a candidate source is: measurement family, numerator, denominator, time reference, geographic grain, case-finding method, missingness, and whether it can separate accumulated backlog from continuing prevention failure. If one of those fields is absent, the source remains limited or rejected rather than being silently promoted.
