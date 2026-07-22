# Dataset Inventory

## Candidate Sources

| Source                                                      | Grain                             | Current status                     | Use                                                                         |
| ----------------------------------------------------------- | --------------------------------- | ---------------------------------- | --------------------------------------------------------------------------- |
| UN IGME stillbirth estimates                                | Country, regional, global         | Usable for burden framing          | Official cross-country burden and trend baseline                            |
| DHS Guide to Statistics: perinatal mortality                | Survey, country and sub-national  | Usable with survey limits          | Reproducible definition and denominator for DHS-7/DHS-8 rates               |
| DHS-8 pregnancy history and interviewer manual              | Household, pregnancy, survey      | Usable for instrument review       | Outcome, duration, and live-birth confirmation wording                      |
| WHO institutional stillbirth indicator metadata             | Facility, country, sub-national   | Usable for indicator specification | Timing, thresholds, denominator, and required disaggregation                |
| UNICEF HMIS stillbirth data-quality assessment              | Facility, district, national      | Usable for data-quality audit      | Vital status, gestational age, birthweight, completeness, and context       |
| WHO/UNICEF MPDSR materials                                  | Facility, community, sub-national | Usable for audit workflow          | Notification, review, modifiable-factor analysis, and non-punitive response |
| WHO CRVS quality and use assessment                         | National CRVS, system components  | Limited for stillbirth rate        | Registration completeness, legal framework, data flow, and quality checks   |
| MICS or other survey modules with pregnancy outcome content | Household, cluster, sub-national  | Limited and uneven availability    | Cross-check on self-reported pregnancy outcomes                             |
| National CRVS stillbirth or fetal death tabulations         | Country to district, variable     | Limited and definition-sensitive   | Registration completeness and legal-definition context                      |
| Facility maternity registers and perinatal death audits     | Facility to district, variable    | Limited and high-risk              | Service-contact signal, never a standalone quality ranking                  |
| EmONC or maternity service readiness assessments            | Facility, district, national      | Limited but relevant               | Context on whether burden plausibly tracks labor-and-delivery care gaps     |
| Population denominators and admin boundaries                | District, gridded, national       | Usable but version-sensitive       | Rate construction and mapping context                                       |

## Required Properties

- Definition threshold: gestational age, birthweight, or local stillbirth definition.
- Measure family: survey recall, CRVS registration, facility count, or audit workflow.
- Numerator and denominator definition.
- Time reference and whether the measurement is period-based or event-based.
- Geographic grain and whether sub-national identifiers survive public release.
- Ability or inability to distinguish intrapartum from antepartum stillbirth.
- Access conditions, reporting incentives, and known missingness.

## Rejection Rule

A source is rejected for canonical comparison if the stillbirth definition threshold, denominator, or reporting population cannot be verified. Facility stillbirth counts without clear referral and case-mix context may be used as workflow clues but not as direct quality rankings. Survey sources that cannot distinguish stillbirth from other adverse pregnancy outcomes at the documented question wording should be listed as limited or rejected rather than generalized.
