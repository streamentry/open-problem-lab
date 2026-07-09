# Dataset Inventory

## Candidate Sources

| Source family                                                                  | Component measured                                                                                 | Timing reference                                  | Grain                                                   | Status                                    | Use                                                                 | Why it belongs in this class                                                                                                                                                   |
| ------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------- | ------------------------------------------------- | ------------------------------------------------------- | ----------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| WHO rabies fact sheet                                                          | Burden, dog-mediated transmission share, basic PEP component definition                            | Updated June 2024                                 | Global and broad regional framing                       | Limited                                   | Burden and component framing                                        | Strong burden anchor, but it cannot identify country, district, or facility access to vaccine, RIG, monoclonal antibodies, triage, or completion.                              |
| Gavi, WHO, and UAR rabies vaccine support announcement                         | Human rabies vaccine support scope and exclusions                                                  | June 2024 programme launch                        | Gavi-eligible country programme eligibility             | Usable for allocation-moment framing      | Separates vaccine procurement support from RIG and dog-vaccine gaps | The source names the current financing window and explicitly prevents treating Gavi vaccine support as complete PEP access.                                                    |
| WHO rabies vaccine position paper                                              | PEP policy, RIG use, route and regimen strategy                                                    | April 2018                                        | Global policy guidance                                  | Limited                                   | Component taxonomy and regimen guardrail                            | Useful for defining what complete PEP means; not a source for current stock, facility readiness, or patient delay.                                                             |
| WHO rabies vaccination and immunization page                                   | Exposure category, RIG indication, intradermal route                                               | Current WHO guidance page, accessed July 2026     | Global clinical and programme guidance                  | Limited                                   | Bite-risk triage and route-capacity guardrail                       | It anchors the category I/II/III distinction and RIG requirement for category III exposure, but cannot prove that a health system applies the rules.                           |
| Rabies PEP logistics assessment, selected Asia and Africa countries, 2017-2018 | Vaccine cost, availability, distribution, intradermal use, reporting cadence                       | January 2017 to May 2018 data collection          | 23 responding countries from a convenience sample       | Limited baseline                          | Baseline taxonomy for source extraction                             | Best current pack source for the shape of PEP logistics variation, but too old and non-representative for present allocation. RIG scarcity meant the study focused on vaccine. |
| WHO GHO rabies topic                                                           | Reported human rabies deaths and WHO data-quality warning                                          | Dynamic GHO topic page, accessed July 2026        | Country indicator surface                               | Limited                                   | Reporting-cadence and burden-presence context                       | Useful as a warning that reported deaths are not a clean denominator. Low deaths can reflect low reporting, not sufficient PEP access.                                         |
| WHO African Region rabies prevention and control WER                           | Surveillance, PEP decision trees, case investigation, IBCM, One Health programme requirements      | June 2026                                         | Regional programme framing                              | Limited                                   | Current Africa-region programme and tool inventory                  | Identifies live programme tools and surveillance requirements, but does not publish country facility-tier access records.                                                      |
| WOAH WAHIS animal-health data                                                  | Animal rabies reports, domestic and wildlife disease notifications, annual animal-health reporting | Dynamic WOAH reporting system, accessed July 2026 | Country and event reporting; sub-national detail varies | Usable only as animal-context layer       | Dog-rabies and dog-vaccination context                              | Official animal-health reporting surface. It must be paired with human PEP data because animal rabies presence alone cannot prove the binding human-health bottleneck.         |
| WHO Rabies Modelling Consortium PEP investment model                           | Modelled Gavi-eligible burden and PEP investment scenarios                                         | Published 2019                                    | Gavi-eligible country model                             | Limited                                   | Tractability and replication target                                 | Supports why PEP investment can matter, but model assumptions cannot substitute for current source inventory or country readiness screening.                                   |
| CDC rabies status by country                                                   | Travel and importation risk classification, including PEP access consideration                     | Updated April 2026                                | Country classification for US public-health use cases   | Rejected for canonical allocation ranking | External comparator only                                            | The page is designed for US travelers and importation policy, not for exposing component-level endemic-country PEP gaps.                                                       |
| Media reports of bite clusters, deaths, or local alerts                        | Event anecdotes                                                                                    | Event date                                        | Local narrative                                         | Rejected for V0 ranking                   | Possible lead generation only                                       | Without linked surveillance, PEP, RIG, animal-rabies, or denominator records, these reports cannot support canonical access classification.                                    |
| Vaccine procurement totals alone                                               | Human vaccine volume                                                                               | Procurement period                                | National or procurement-unit aggregate                  | Rejected for complete PEP access          | Procurement context only                                            | Procurement does not prove timely first dose, completion, intradermal capacity, RIG or monoclonal availability, correct triage, patient cost, or rural reach.                  |

## Classification Notes

### Usable

- **Gavi, WHO, and UAR rabies vaccine support announcement**: Use for the current allocation moment and for excluding overclaiming. The programme can support human rabies vaccine procurement and associated supplies, but the source does not prove RIG access, dog vaccination, country approval, delivery, or completion.
- **WOAH WAHIS animal-health data**: Use only as the dog-rabies and animal-surveillance side of a One Health evidence chain. It is usable because it is the official reporting surface for animal-health events, but it is insufficient without human bite, PEP, and biologics records from the same geography and time.

### Limited

- **WHO rabies fact sheet**: Use for global burden, transmission source, and the complete PEP component chain. Do not use it for country readiness.
- **WHO rabies vaccine position paper and WHO rabies vaccination page**: Use for component definitions, exposure categories, RIG indication, and route/regimen guardrails. They are guidance sources, not implementation proof.
- **Sreenivasan et al. PEP logistics assessment**: Use as the baseline source taxonomy for vaccine availability, cost, distribution, intradermal use, and reporting cadence. Its age, convenience sample, and vaccine focus make it a source-discovery tool rather than a current ranking backbone.
- **WHO GHO rabies topic**: Use as a reported-deaths surface and a warning about surveillance weakness. Reported deaths can indicate presence, not full extent.
- **WHO African Region WER**: Use for current programme framing around surveillance, PEP decision trees, case investigation, and IBCM. It does not provide a country-by-country readiness table.
- **WHO Rabies Modelling Consortium model**: Use to identify assumptions a replicator must test. It does not classify present-day component gaps.

### Rejected

- **CDC rabies status by country**: Reject for canonical allocation ranking because its intended decision is US travel and animal-importation guidance. It can be checked as an external comparator after source-level country evidence exists.
- **Media reports of single bite clusters or deaths**: Reject unless they link to official surveillance, PEP utilization, RIG, animal-rabies, or denominator data.
- **Vaccine procurement totals alone**: Reject for complete PEP access. A country can procure vaccine and still fail on category-III RIG, monoclonal access, triage, cost, completion, or rural travel burden.

## Required Properties Before Country Screening

- Component measured: wound care, exposure-category triage, vaccine access, route/regimen capacity, RIG or monoclonal access, patient cost or travel burden, reporting cadence, or dog-vaccination and animal-rabies context.
- Geography and facility tier, not just national programme narrative.
- Time reference and reporting cadence.
- Numerator and denominator, including whether the denominator is bite victims, suspected exposures, category-II/III exposures, vaccine courses, completed schedules, RIG-eligible patients, dogs vaccinated, or animal rabies events.
- Access conditions and whether the source is public, archived, downloadable, or dashboard-only.
- Known mismatch against other components. A source measuring one component must not be promoted to complete PEP access.

## Rejection Rule

A source is rejected for canonical component-level PEP access analysis if it lacks a dated source, a recoverable URL, a named component, a checkable grain, or a denominator. Sources valid only for burden framing, clinical guidance, travel advice, or animal-health context should be listed as limited rather than silently generalized.

## Task Verdict

This inventory satisfies the scoped `source-inventory` task because it classifies more than six candidate sources as usable, limited, or rejected with explicit reasons covering:

- vaccine access and procurement scope
- RIG or monoclonal antibody indication and access limits
- bite-risk triage and exposure category
- reporting cadence and under-reporting
- patient cost and delivery-system baseline from the logistics assessment
- dog-vaccination and animal-rabies context through WOAH WAHIS

It does **not** satisfy country-readiness screening. The next task should fail unless it pairs human PEP records with RIG or monoclonal availability, exposure-category or bite-risk data, and animal-rabies context for the same geography and time window.
