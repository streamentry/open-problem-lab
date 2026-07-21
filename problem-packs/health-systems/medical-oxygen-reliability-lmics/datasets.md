# Dataset Inventory

## Candidate Sources

| Source                                                        | Grain                                   | Classification                      | What it can support                                              | Main limitation                                                      |
| ------------------------------------------------------------- | --------------------------------------- | ----------------------------------- | ---------------------------------------------------------------- | -------------------------------------------------------------------- |
| Ijaz et al. 2025 facility assessment                          | Facility, 39 LMICs, primary to tertiary | Usable with caveats                 | Reliability over prior three months and component availability   | Purposive/stratified sample and facility self-report                 |
| WHO Service Availability and Readiness Assessment instruments | Facility                                | Usable as instrument reference      | Standardized readiness fields and facility sampling structure    | Oxygen fields and survey implementations vary by country and round   |
| WHO-UNICEF oxygen device guidance                             | Device/system component                 | Usable as definition reference      | Equipment specifications, selection, use, and maintenance fields | Not a facility-status dataset                                        |
| WHO national oxygen scale-up tools                            | Country planning                        | Limited for facility comparison     | Demand and system-planning categories                            | Planning tool outputs are not observed uptime or patient delivery    |
| PATH Oxygen Needs Tracker                                     | Country/model                           | Limited for facility prioritization | Modeled oxygen need and advocacy context                         | COVID-era assumptions and modeled need are not measured reliability  |
| WHO oxygen technical page                                     | Global technical reference              | Limited for measurement             | Component taxonomy and quality concepts                          | Living page, no harmonized facility-level data or stable update date |
| National hospital equipment inventories                       | Facility or district, country-specific  | Limited pending audit               | Installed equipment and procurement history                      | Presence does not prove function, quality, power, or maintenance     |

## Required Dataset Properties

Any source used for a reliability analysis must document:

- Facility identifier, level, location, and sampling frame.
- Observation window and whether reliability is direct observation, logbook, sensor, or self-report.
- Oxygen source, distribution, delivery, monitoring, power, quality assurance, and maintenance fields.
- Denominator and missingness for every reported percentage.
- Medical-grade concentration or quality checks where available.
- Access conditions, reuse permission, version, and source date.

## Rejection Rule

A source is rejected for canonical reliability classification if it only reports equipment procurement or ownership without a function test, observation window, facility denominator, or limitation statement. Modeled oxygen need is not substituted for measured oxygen reliability.
