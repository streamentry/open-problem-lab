# Dataset Inventory

## Candidate Sources

| Source / evidence ID                                                                  | Grain                                                        | Classification                                                     | Currency / access                                                                      | What it can support                                                                                                                         | Why it cannot support more                                                                                          |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------------ | -------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| National training-provider registries                                                 | Institution or district, country-dependent                   | **Candidate; audit required**                                      | Fragmented across government, NGO, private, and informal providers; access varies      | Provider availability and programme inventory where coverage is documented                                                                  | Cannot establish national completeness or graduate employment without provider-type and missingness audit           |
| ILO SWTS microdata (`ilo-swts-microdata-2014`)                                        | Youth individual, country survey                             | **Usable with access and vintage limits**                          | More than 30 countries, 2012-2016; microdata by request                                | Youth training participation, labour-market transition, employment and unemployment pathways; LDES employer-demand layer in seven countries | Historical, country-specific, not a provider registry, and not automatically sub-national or current                |
| ILO YouthSTATS (`ilo-youthstats-methodology-2022`)                                    | Country or survey indicator, youth ages 15-29                | **Usable for definitions and context**                             | ILOSTAT gateway; exact update date not exposed                                         | Harmonized youth employment, unemployment, transition, working-time, and earnings concepts                                                  | No provider enumeration, participant-level training attribution, or guaranteed sub-national grain                   |
| ILOSTAT LFS and informality methods (`ilostat-informal-employment-methods-2023`)      | Household microdata and country indicators, mainly main job  | **Usable for informal-outcome definitions**                        | National-source microdata processed by ILO; country availability varies                | Formal/informal employment classification and outcome-context design                                                                        | Does not identify training graduates, provider participation, second-job outcomes, or causal impact                 |
| World Bank STEP (`worldbank-step-skills-measurement-2017`)                            | Urban adults ages 15-64, household and employer survey       | **Usable skills-demand layer; limited for youth/provider mapping** | Data collected 2012-2017 in listed economies; documentation available with dataset     | Cognitive, socio-emotional, job-relevant skills, employer training, skills demand, and satisfaction with training                           | Urban target population, historical coverage, no provider census, and separate household/employer instruments       |
| UNESCO-UNEVOC TVET country profiles (`unesco-unevoc-tvet-country-profiles-2026`)      | National TVET system and comparative indicators              | **Limited but useful system context**                              | Dynamic partner database; current profile currency and underlying sources vary         | National TVET governance, pathways, system diagrams, and statistical context                                                                | Not a complete provider registry, sub-national availability map, or graduate tracer                                 |
| World Bank Enterprise Surveys (`worldbank-enterprise-surveys-2024`)                   | National formal-firm survey; some indicator views by economy | **Usable employer-demand context**                                 | 2006-2023 catalog coverage; public CC BY 4.0 aggregated data; microdata registered     | Employer-side constraints, formal-firm training indicators, firm characteristics, and demand context                                        | Formal firms dominate the core frame; no youth graduate linkage, provider inventory, or informal-sector equivalence |
| Benin Youth Employment Project metadata (`worldbank-benin-youth-employment-rct-2026`) | Project and randomized treatment arm                         | **Usable evaluation-design source; outcome access pending**        | 2017 Benin study; public classification but no resources listed; Research Data License | Defines treatment arms, outcome fields, gender and skills heterogeneity, and a reproducible evaluation design                               | Country/program-specific, baseline metadata, no provider census, and no result can be cited without follow-up data  |
| TVET management information systems                                                   | Institution or programme, variable                           | **Limited**                                                        | Often restricted to ministries or providers; release and access must be checked        | Enrollment, completion, attendance, and sometimes placement fields                                                                          | Provider coverage and outcome definitions vary; private, NGO, and informal providers may be absent                  |
| NGO and private training documentation                                                | Programme, cohort, variable                                  | **Limited**                                                        | Often available only through programme reports or direct requests                      | Identify non-government provision and cohort-specific outcomes                                                                              | No common denominator, inconsistent follow-up, selective reporting, and no national completeness                    |
| Skills-mismatch assessments                                                           | Sector or occupation, variable                               | **Limited**                                                        | Methods and dates vary; employer and worker instruments are not interchangeable        | Demand-supply context and occupation-level mismatch hypotheses                                                                              | Does not identify provider capacity or prove training causes employment                                             |
| Single follow-up or graduate self-report without baseline                             | Graduate or programme, variable                              | **Rejected for effectiveness claims**                              | Access and follow-up completeness often unclear                                        | Hypothesis generation about outcomes and measurement feasibility                                                                            | Cannot separate selection, attrition, labour-market change, informal work, or programme effect                      |

## Required Dataset Properties

- Date range and temporal resolution.
- Geographic grain and spatial resolution.
- Training-provider data completeness — explicitly document fragmentation across government, NGO, and private operators.
- Employment-outcome tracking rate — document what share of training programs track graduate employment.
- Informal-sector measurement methodology.
- Access conditions and license.

## Inventory Decision Rule

The current evidence supports a layered analysis, not one merged dataset:

1. Use UNEVOC and country administrative sources for TVET system context.
2. Use provider registries and programme records only after enumerating which provider types are absent.
3. Use SWTS, YouthSTATS, labour-force surveys, and STEP for participant or labour-market context with survey-specific denominators.
4. Use Enterprise Surveys for formal-employer demand and formal-training indicators, keeping informal-enterprise sources separate.
5. Use named evaluation datasets such as Benin only for their documented treatment arms and outcomes.

No source currently verifies the pack's earlier “fewer than 10 percent of programs track outcomes” statement across LMICs. That figure is removed from the canonical framing until a country-specific programme census and tracking denominator are found.

## Cross-Validation Requirements

Before a sub-national analysis is called actionable, it must report:

- provider types and geographic coverage captured by each registry;
- training type, cohort, enrollment, completion, and outcome-tracking fields;
- labor-force survey youth definition and informal/self-employment capture;
- employer-sector and firm-size coverage;
- observation year and update lag; and
- unmatched providers, unmatched graduates, missing outcomes, and any linkage assumptions.

## Rejection Rule

A dataset is rejected for canonical analysis if grain, date range, license, or method cannot be verified. Datasets with known limitations may be listed as limited with explicit documentation. Rejected datasets may still be listed as context or as evidence of a measurement gap.
