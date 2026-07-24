# Dataset Inventory

## Measure Families

These measures answer different questions and must not be collapsed:

| Measure family     | Question answered                                                         | Common failure                                                |
| ------------------ | ------------------------------------------------------------------------- | ------------------------------------------------------------- |
| Living arrangement | Who resides in the household?                                             | Living alone is treated as equivalent to lacking support.     |
| Family distance    | How long would a chosen family responder take to arrive?                  | Administrative residence is treated as actual availability.   |
| Functional need    | What activities or capacities require support?                            | Diagnosis is treated as functional dependence, or vice versa. |
| Care receipt       | Who currently provides which care and how often?                          | Any family contact is counted as adequate care.               |
| Local response     | Who can acknowledge, reach, resolve, or transfer a request?               | A phone number is counted as a functioning service.           |
| Consent preference | What monitoring, disclosure, and assistance does the older person accept? | Family authorization replaces the older person's decision.    |

## Candidate Data Sources

| Source family                                                         | Potential grain                     | Current status                                                   | Potential use                                                            | Blocking limitation                                                                                                                  |
| --------------------------------------------------------------------- | ----------------------------------- | ---------------------------------------------------------------- | ------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ |
| 2019 Population and Housing Census and ageing tables                  | Household to district/province      | Limited but usable for population frame                          | Age, household context, migration, disability proxy, living arrangement  | Public tabulations do not preserve family distance, consent, current responder availability, or linkable household detail.           |
| VHLSS 2022 results and microdata documentation                        | Household, individual, commune      | Blocked pending stable source access and microdata/module review | Household composition, health-care use, income, housing, commune context | The official publication endpoint was not reachable in the repository source check; do not use a secondary citation as a substitute. |
| Population Change and Family Planning Survey 2021 older-person module | Person/household, release-dependent | Candidate, pending questionnaire and microdata inspection        | Older-person care needs and situation, population context                | Publication description does not expose all field definitions, missingness, weights, consent, or responder variables.                |
| Vietnam Time-Use Survey 2022                                          | Individual/household, region        | Usable for caregiver-time context                                | Unpaid elder-care time and caregiver burden among ages 15–64             | It excludes older respondents and does not measure response timeliness, resolution, or clinical outcomes.                            |
| National Survey on People with Disabilities 2016                      | Person/household, release-dependent | Limited and dated                                                | Functional limitation and disability measurement                         | Disability is not the full care-need construct; the 2016 frame needs newer corroboration.                                            |
| National Internal Migration Survey 2015                               | Migrant/person, release-dependent   | Limited context source                                           | Migration and service-access context                                     | Migration does not equal family distance or unavailability; it cannot identify a care-response gap.                                  |
| UNFPA and National Statistics Office analyses                         | National synthesis                  | Context only until underlying tables are accessible              | Demographic and care-system framing                                      | Published stories do not expose all variable definitions or microdata.                                                               |
| Intergenerational self-help club administrative records               | Club, commune, participant          | Limited                                                          | Responder presence, visit records, service types                         | Coverage, data quality, consent, denominator, staff capacity, and access terms are unverified.                                       |
| Commune health-station or NCD management records                      | Facility or patient                 | Blocked pending approval                                         | Referral capacity and continuity context                                 | Sensitive health data, incomplete capture, incompatible identifiers, and no proof of home-response availability.                     |
| Social-protection and social-work case records                        | Facility, case, or locality         | Blocked pending approval                                         | Existing care pathways and vulnerability support                         | Sensitive data, selection bias, incomplete community coverage, and unclear reuse permission.                                         |
| Prospective manual pilot event log                                    | Request and visit                   | Not yet collected                                                | Acknowledgement, reach, resolution, transfer, unresolved events, cost    | Requires protocol approval, consent, data minimization, safeguarding, and exit plan.                                                 |

## Rejected Inputs

- Commercial wearable dashboards without event-level response and attrition data.
- Testimonials offered as average impact evidence.
- Family contact lists treated as proof of availability.
- Smartphone activity treated as proof of safety or functional capacity.
- Household-level health or location data obtained without documented consent and minimization.

## Required Properties

- Measure family and exact field definition.
- Source year and collection period.
- Sampling frame and weighting.
- Geographic grain and boundary version.
- Missingness and proxy-response rules.
- Consent, access, license, and linkage restrictions.
- Whether the source measures presence, contact, reach, resolution, or outcome.

## Rejection Rule

A source is rejected for denominator construction if it silently equates living alone with unmet need, family residence with response availability, contact with resolution, or monitoring with health benefit.

## Source-inventory decision

The five dated additions in `evidence.json`, together with the existing official evidence ledger, satisfy the scoped task's minimum inventory. None is sufficient alone for the care-gap denominator. The next defensible step is questionnaire and microdata inspection of the 2021 older-person module and VHLSS 2022 once a stable official endpoint is available, followed by a separate specification that leaves family travel time, consent, and responder availability unknown when unobserved.
