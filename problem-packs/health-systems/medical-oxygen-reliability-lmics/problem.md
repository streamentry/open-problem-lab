# Reliable Medical Oxygen Systems In LMICs

## Problem Statement

Medical oxygen is an essential medicine, but access is a system property rather than an equipment checkbox. A facility may own a cylinder or concentrator and still be unable to deliver safe oxygen because power, storage, piping, regulators, delivery interfaces, pulse oximeters, quality assurance, or maintenance fail.

> Which facility-level oxygen-system components most often break the chain from oxygen source to patient in low- and middle-income countries, and which measurements are reliable enough to change a named financing or maintenance decision?

## Known Facts

- Verified fact: WHO estimated in 2023 that fewer than half of LMIC health facilities had uninterrupted access to medical oxygen.
- Verified fact: A 2025 cross-sectional assessment of 2,884 facilities in 39 LMICs found reliable oxygen availability at 24.5% of primary, 52.4% of secondary, and 66.8% of tertiary facilities.
- Verified fact: The same assessment found large component-level variation, including pulse-oximeter availability from 47.8% to 96.4% and piping from 7.5% to 94.6%, depending on facility level and WHO subregion.
- Verified fact: WHO technical guidance treats oxygen as a system spanning source, distribution, regulation, delivery, monitoring, power, and maintenance.

## Uncertain Areas

- Whether facility self-report of three-month reliability agrees with direct observation, logbook, oxygen-concentration, and power-uptime checks.
- Whether national facility surveys identify district-level bottlenecks well enough for procurement or maintenance prioritization.
- Which failure component has the highest marginal effect on patient-level access after accounting for staffing, case mix, referral pathways, and demand.
- Whether observed reliability gaps persist outside the assessment period and during demand surges.

## Initial Scope

This pack accepts work on:

- Evidence and dataset inventory for facility-level oxygen sources, distribution, delivery, monitoring, power, maintenance, and quality assurance.
- Harmonization of “available”, “functional”, “reliable”, “medical-grade”, and “patient-deliverable” definitions.
- Missingness and denominator audits for facility assessments.
- Reproducible comparisons of component failures across facility level, geography, and assessment period.
- Red-team review of procurement, rationing, and clinical-use interpretations.
- Field-reality review with ministries, biomedical engineers, hospital managers, and oxygen-program implementers.

This pack does not accept clinical dosing advice, facility rankings presented as investment recommendations, or causal claims that equipment installation alone improves mortality.

## Discovery Ranking Used

| Candidate                                               | Scale                                                                                                                                                                                                                                                                                                                      | Tractability                                                                                                                                  | Neglectedness                                                                                                                                            | Evidence gap                                                                                                                                      | Why not selected                                                                              |
| ------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| Reliable medical oxygen systems in LMIC facilities      | WHO estimates fewer than half of LMIC facilities have uninterrupted oxygen; a 2025 study assessed 2,884 facilities in 39 LMICs ([WHO](https://www.who.int/publications/m/item/statement-on-access-to-quality-and-safe-medical-oxygen), [Ijaz et al.](https://www.sciencedirect.com/science/article/pii/S2214109X24005618)) | Existing facility assessments and WHO component definitions permit a reproducible reliability inventory and failure-mode classification       | Evidence is strong enough to show a gap but weak enough that donors cannot reliably distinguish source, power, distribution, and maintenance bottlenecks | Whether reported reliability and component availability can be harmonized into a decision-grade measure without implying causal mortality effects | Selected: largest uncovered health-system wedge with a concrete measurement-to-financing path |
| Safe blood availability for obstetric and trauma care   | WHO Africa reports roughly 5 million blood units collected annually, about half the estimated need in the region ([WHO AFRO](https://www.afro.who.int/news/drop-blood-donations-add-maternal-health-threats-africa))                                                                                                       | Blood-service inventories and facility assessments exist, but cross-country comparability is constrained by screening and product definitions | Important but already overlaps strongly with maternal mortality and emergency obstetric packs in this portfolio                                          | Whether stock-out duration and timely cross-facility availability are measured consistently                                                       | Not selected: narrower but more institutionally covered by existing maternal packs            |
| Newborn serious-bacterial-infection treatment access    | Bacterial infections account for nearly a quarter of neonatal deaths in LMIC-focused evidence, but access varies by facility and referral context ([Herlihy et al.](https://pmc.ncbi.nlm.nih.gov/articles/PMC4196753/))                                                                                                    | Facility and household surveys can measure recognition, referral, and antibiotic stock, but causal interpretation is difficult                | High need, but the portfolio already contains neonatal mortality, pneumonia, AMR, and child-treatment packs                                              | Whether low antibiotic stock, delayed referral, and resistance explain the same outcome at facility level                                         | Not selected: higher overlap and more confounded treatment pathways                           |
| Functional cold chain for vaccines in remote facilities | WHO/UNICEF coverage systems document immunization service delivery, but facility uptime and temperature excursions are not consistently comparable across countries                                                                                                                                                        | Temperature-log and power data can be audited                                                                                                 | High value, but vaccine-coverage equity is already represented in the portfolio                                                                          | Whether cold-chain uptime predicts missed opportunities independent of staffing and outreach                                                      | Not selected: important but less distinct from existing vaccination-coverage work             |

## Done Condition For V0

The pack is useful when one reviewed and independently reproducible source inventory distinguishes at least five oxygen-system data sources and explicitly states which can measure facility reliability, component function, power continuity, quality assurance, or patient-level delivery.
