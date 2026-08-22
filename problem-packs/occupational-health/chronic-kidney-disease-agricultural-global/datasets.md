# Dataset Inventory

## Candidate Sources

| Source / evidence ID                                                         | Grain                                                     | Classification                                           | What it can support                                                                                          | Why it cannot support more                                                                             |
| ---------------------------------------------------------------------------- | --------------------------------------------------------- | -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ |
| WHO kidney disease fact sheet (`who-kidney-disease-fact-sheet-2026`)         | Global CKD framing and diagnostic criteria                | **Usable for context and persistence rules**             | Broad CKD scale, LMIC concentration, eGFR/albuminuria persistence concepts                                   | Does not measure CKDu, agricultural workers, exposure, or sub-national burden                          |
| ISN i3C report (`isn-ckdu-consortium-measurement-gaps-2026`)                 | Cross-region field synthesis                              | **Usable for measurement-gap framing**                   | Terminology, onset-versus-progression, and exposure-measurement problems                                     | Does not provide a representative prevalence denominator or causal result                              |
| ISN Global Kidney Health Atlas (`isn-global-kidney-health-atlas-2023`)       | Country and income-group kidney-care capacity             | **Limited contextual layer**                             | Diagnostic and kidney-replacement readiness context for feasibility assessment                               | Total kidney disease and capacity indicators are not CKDu-specific or agricultural-worker observations |
| Sri Lanka multilevel case definition (`sri-lanka-ckdu-case-definition-2019`) | Regional surveillance definition                          | **Usable as a template; limited for transfer**           | Candidate fields and tiered CKDu classification                                                              | Regional criteria may not transfer to other settings without validation                                |
| MANOS occupational cohort (`manos-ckdu-workers-2022`)                        | Worker, industry, country, repeated serum tests           | **Usable research template**                             | Persistent kidney-function measurement, worksite observation, industry comparison, and exposure-study design | Selected Central American industries and workers; not a global denominator or causal estimate          |
| CKDu-AGRI Tamil Nadu (`ckdu-agri-tamil-nadu-2025`)                           | Statewide agricultural-worker sample, two-phase testing   | **Usable local prevalence evidence**                     | Demonstrates repeat-testing impact and a bounded CKDu estimate                                               | Tamil Nadu protocol and sampling cannot be treated as globally comparable without a crosswalk          |
| Rural Sri Lanka CKDu study (`sri-lanka-rural-ckdu-prevalence-2022`)          | Selected rural population and biomarker/exposure measures | **Usable local signal; limited generalizability**        | Suspected CKDu signal and candidate exposure fields                                                          | Small selected sample, suspected case label, and cross-sectional associations                          |
| Global CKD burden models                                                     | Global or country modeled estimates                       | **Limited for CKD context; rejected for CKDu numerator** | Background burden and trend framing                                                                          | Modeled CKD of all causes cannot establish CKDu, occupational burden, or exposure attribution          |
| Self-reported exposure surveys without repeat kidney testing                 | Worker or household, variable                             | **Limited for hypothesis generation**                    | Candidate exposure and recall instruments                                                                    | Recall, selection, and reverse-causality risk; cannot prove exposure or persistent disease             |
| Single serum creatinine or eGFR screen                                       | Individual or community snapshot                          | **Rejected for confirmed CKD/CKDu prevalence**           | Signal detection and recruitment for repeat testing                                                          | Cannot distinguish transient AKI, dehydration, assay error, or persistent CKD                          |
| Administrative dialysis or kidney-failure records                            | Facility or patient event, variable                       | **Limited outcome context**                              | Advanced disease and service-demand context                                                                  | Misses undiagnosed disease and cannot classify CKDu cause without clinical and exposure data           |

## Required Dataset Properties

- Kidney-function assay, calibration, eGFR equation, and urine marker.
- Repeat-test interval and persistence rule; at least 90 days for a CKD confirmation unless a source explicitly justifies another design.
- CKDu/CINAC operational label, traditional-risk-factor exclusions, and proteinuria/albuminuria phenotype.
- Worker population, industry, employment status, age/sex distribution, household/community frame, and recruitment exclusions.
- Exposure domain, instrument, timing, recall window, biological/environmental sample, and missingness.
- Acute kidney injury, dehydration, infection, medication, pregnancy, and other alternative explanations considered by the source.
- Geographic grain, season, work cycle, laboratory location, and administrative-boundary changes.
- Data access, consent, privacy, license, and whether individual-level replication is possible.

## Measurement Decision Rule

Only sources that preserve persistence, phenotype, denominator, and classification method can support a cross-setting CKDu matrix. A source may be useful for hypothesis generation while remaining unusable for prevalence, causality, or allocation. The pack should prefer a negative result documenting non-comparability over a harmonized percentage that hides incompatible definitions.

## Rejection Rule

A dataset is rejected for confirmed CKDu prevalence if it uses a single kidney-function observation, cannot document the numerator and denominator, collapses traditional CKD and CKDu, lacks the case-definition or assay method, or cannot distinguish self-report from objective exposure measurement. Rejected sources may remain in the ledger as context or as evidence of a surveillance gap.
