# Dataset Inventory

## Candidate Sources

| Source                                               | Grain                          | Current status               | Use                                                                                  |
| ---------------------------------------------------- | ------------------------------ | ---------------------------- | ------------------------------------------------------------------------------------ |
| UNFPA Campaign to End Fistula records                | Country, program, variable     | Limited but central          | Campaign footprint, supported repairs, program priorities, and policy framing        |
| BMJ Global Health 2025 prevalence estimates          | Country, regional, global      | Usable for burden framing    | Current modelled prevalence baseline for 55 low- and middle-income countries         |
| DHS fistula module and women's questionnaire data    | Individual, cluster, national  | Limited and survey-dependent | Awareness and self-reported symptom measures where the module was fielded            |
| National fistula program or repair-center registries | Facility, program, country     | Limited and fragmented       | Repair volume, follow-up, and case-finding clues when provenance is documented       |
| Surgical outcome studies and repair cohorts          | Facility, study cohort         | Limited for access           | Repair success, continence, recurrence, and follow-up definitions                    |
| EmONC needs assessments and facility readiness data  | Facility, district, national   | Limited but relevant         | Prevention context for obstructed labour management and emergency obstetric capacity |
| Referral-delay, transport, and caesarean-access data | District to facility, variable | Limited                      | Mechanism evidence for incident fistula prevention failures                          |
| Population denominators and admin boundaries         | District, gridded, national    | Usable but version-sensitive | Rate construction, catchment comparison, and uncertainty documentation               |

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
