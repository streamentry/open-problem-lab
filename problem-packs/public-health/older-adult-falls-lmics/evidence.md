# Evidence Ledger

## Interpretation Rule

This ledger records what each dated source can support at its own grain. It does not turn a global burden estimate into local incidence, a risk-factor association into causation, a facility registry into population coverage, or a fall-prevention trial into a universal programme recommendation.

## Current Records

| Evidence ID                               | Source layer                                   | What it supports                                                                                  | Confidence | Boundary                                                                                |
| ----------------------------------------- | ---------------------------------------------- | ------------------------------------------------------------------------------------------------- | ---------- | --------------------------------------------------------------------------------------- |
| `who-falls-global-burden-2021`            | WHO fact sheet                                 | Global fatal and medically attended fall burden and LMIC/older-adult concentration                | high       | No current local denominator or intervention effect                                     |
| `who-step-safely-2021`                    | WHO technical package                          | Prevention and management evidence questions across life-course groups                            | high       | Synthesis is not local implementation or effect evidence                                |
| `who-older-adult-falls-report-2008`       | WHO global report                              | Historical older-adult fall ranges and resource-targeting rationale                               | high       | Historical ranges are not current LMIC estimates                                        |
| `sage-fall-injury-lmic-2015`              | Nationally representative six-country analysis | Self-reported fall-related injury and disability association in adults aged 50+                   | high       | 2007–2010-era, cross-sectional, self-reported, and not 60+ only                         |
| `sawe-fall-registry-malawi-tanzania-2023` | Prospective multi-facility registry analysis   | Fall complaints, injury severity, arrival interval, and disposition fields in two African systems | high       | Selected facilities and highway/emergency corridors are not population incidence        |
| `family-fall-prevention-rct-china-2025`   | Cluster randomized trial                       | A tested primary-care-integrated intervention and its fall/function outcomes                      | high       | One rural Chinese system, bundled effect, self-reported falls, limited generalizability |
| `who-injury-dataset-2020`                 | WHO facility data standard                     | Candidate core and extended variables for injury-care documentation and aggregation               | high       | Standard variables do not ensure community coverage or follow-up                        |
| `who-clinical-registry-trauma-2025`       | WHO clinical registry platform                 | Practical structured injury/emergency capture, including prehospital timing                       | high       | Platform availability is not implementation, completeness, or patient outcome           |

## Persistent Claim

`fall-injury-data-sufficiency-lmics` is an **unverified** data-sufficiency claim. It states that the current public source set can frame burden and a prevention pathway, but does not yet provide one allocation-ready, cross-LMIC linkage from population falls through care delay to functional recovery. Its failure modes, kill condition, reviewer roles, and limitations are recorded in `claims.json`; the claim must not advance to acceptance without domain, replication, and red-team review.

## Evidence Gaps That Matter

The evidence base is sufficient to justify a bounded measurement problem and a plausible prevention path, but not a global intervention ranking. The critical missing joins are:

- a current older-adult fall denominator that captures people who do not reach a facility
- a reproducible link between fall event, injury severity, care-seeking, transport, arrival, treatment, transfer, and rehabilitation
- a shared functional-outcome definition that distinguishes discharge status, recurrent falls, disability, participation, and patient-defined goals
- prevention exposure and fidelity fields that identify which components were actually delivered
- equity and missingness fields that reveal whether the oldest, poorest, rural, disabled, isolated, or non-English-speaking people disappear from follow-up

The next task should attempt one country-bounded linkage and may conclude that the sources cannot be combined. That negative result is preferable to a spurious prevalence or effect estimate.

## Source Decay

The WHO global burden and older-adult report are dated context, while the SAGE and African registry results describe historical study periods. The FAMILY trial is newer but still setting-specific. Before an allocation-facing output, refresh mortality, household, facility, transport, rehabilitation, and intervention evidence and preserve the source-year boundary.
