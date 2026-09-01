# Evidence Ledger

## Interpretation Rule

The evidence ledger records what a dated source can support, at its own grain. It does not turn global need estimates into local coverage, service guidance into implementation evidence, or medicine consumption into palliative-care access. Every quantitative or operational claim in this pack must point to an evidence ID in `evidence.json`.

## Current Records

| Evidence ID                                      | Source layer                      | What it supports                                                                                    | Confidence | Boundary                                                                                 |
| ------------------------------------------------ | --------------------------------- | --------------------------------------------------------------------------------------------------- | ---------- | ---------------------------------------------------------------------------------------- |
| `who-palliative-care-burden-access-2020`         | WHO fact sheet                    | Global need and reported access context; 194-Member-State funding/reach survey context              | high       | No current country denominator or patient-level coverage                                 |
| `who-palliative-care-actionable-indicators-2021` | WHO technical indicator framework | Candidate policy, service, medicine, training, community, and research fields                       | high       | Framework is not implementation or impact evidence                                       |
| `who-primary-care-palliative-guide-2018`         | WHO primary-care guide            | Service-layer, referral, continuity, equity, patient-values, and family-support design requirements | high       | General guidance is not local workforce or clinical-effect evidence                      |
| `who-quality-palliative-care-2021`               | WHO quality resource              | Quality domains and measurement/planning frame                                                      | high       | No universal thresholds or outcome dataset                                               |
| `who-morphine-access-2023`                       | WHO medicine-access report        | Morphine's medical role and barriers to safe access                                                 | high       | Morphine is used across several clinical contexts and is not coverage                    |
| `incb-narcotic-drugs-2019`                       | INCB technical statistics         | Dated global distribution of morphine consumption                                                   | high       | Aggregate 2018 consumption does not identify indication, appropriateness, or local stock |
| `who-hhfa-comprehensive-guide-2023`              | WHO facility-assessment framework | Facility availability, readiness, quality, management, and finance methods                          | high       | Facility assessment does not show population need, receipt, continuity, or benefit       |
| `who-palliative-care-planning-2016`              | WHO programme-management guide    | Candidate policy, service, medicine, education, and evaluation indicators                           | high       | Design guidance is not current country data or programme performance                     |
| `who-palliative-care-paediatrics-2018`           | WHO paediatric guide              | Child-specific need and service-planning boundary                                                   | high       | Historical guidance and estimates are not current paediatric coverage                    |
| `whpca-global-atlas-2020`                        | WHPCA global synthesis            | 2017 need proxy, country development categories, provider/patient baseline tables                   | high       | Mixed-source 2020 synthesis is not current operating capacity or continuity              |
| `who-hhfa-indicator-reference-2024`              | WHO facility questionnaire        | Concrete facility fields for palliative service type, home linkage, guideline observation, training | high       | Reference instrument is not a completed national or facility dataset                     |
| `who-global-health-estimates-methods-2024`       | WHO mortality methods             | Reproducible mortality-context inputs and temporal boundary                                         | high       | Mortality context is not palliative-care need, receipt, or outcome                       |

## Source-Inventory Completion Note

The completed inventory now covers the seven task requirements at different evidence levels:

| Requirement                    | Accepted source records                                                                      | Inventory result                                                                                                                        |
| ------------------------------ | -------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| Population need                | `who-palliative-care-burden-access-2020`, `whpca-global-atlas-2020`                          | Usable for dated global context and a serious-health-related-suffering proxy; local denominator remains open.                           |
| Service supply and planning    | `who-palliative-care-actionable-indicators-2021`, `who-palliative-care-planning-2016`        | Usable for field design and candidate service indicators; a directory or policy is not operating capacity.                              |
| Facility readiness             | `who-hhfa-comprehensive-guide-2023`, `who-hhfa-indicator-reference-2024`                     | Usable for facility assessment design, including palliative-specific service and training fields; no patient access claim.              |
| Referral and continuity        | `who-primary-care-palliative-guide-2018`, `who-quality-palliative-care-2021`                 | Usable for pathway and quality-field design; no linked referral-to-closure dataset is currently identified.                             |
| Medicine access                | `who-morphine-access-2023`, `incb-narcotic-drugs-2019`                                       | Usable for separate access and distribution context; no coverage or appropriate-use inference.                                          |
| Patient and caregiver outcomes | `who-quality-palliative-care-2021`, `who-palliative-care-actionable-indicators-2021`         | Frameworks identify the need for person-centred and caregiver measures; a validated, open, cross-country episode dataset remains a gap. |
| Equity and missingness         | `who-palliative-care-actionable-indicators-2021`, `who-global-health-estimates-methods-2024` | Usable for required strata and mortality-context scaffolding; incomplete reporting must remain visible rather than imputed.             |

This is sufficient for the task's source classification condition, but not for a country-level coverage estimate. The next task must test the missing joins in one named setting and may return a negative result.

## Evidence Gaps That Matter

The portfolio now has authoritative definitions and candidate measurement tools, but it does not yet have a verified country-level cascade. The critical missing joins are:

- a need denominator that does not silently substitute mortality, cancer, or last-year-of-life counts for all relevant suffering
- a service frame that verifies whether listed services are operating, reachable, staffed, and able to accept referrals
- an episode link from referral to first contact, continuing support, transfer, closure, or loss to follow-up
- a medicine link that separates legal access, procurement, availability, affordability, dispensing, and appropriate use
- patient- and caregiver-reported goals and outcomes that are not replaced by provider activity or opioid volume

The next task must test whether these joins can be made in one named LMIC setting. A negative result is useful: it would show that a proposed allocation comparison is not yet auditable.

## Source Decay

The WHO fact sheet and INCB statistics are dated context, not live dashboards. Before an allocation-facing output, refresh the need estimate, medicine statistics, national policy, facility frame, and local service records. If an indicator page has moved or an API has retired, preserve the historical record and revalidate the replacement rather than silently changing the series.
