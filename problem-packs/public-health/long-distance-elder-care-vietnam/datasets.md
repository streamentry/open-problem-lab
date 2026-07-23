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

| Source family                                           | Potential grain                            | Current status                                      | Potential use                                                         | Blocking limitation                                                                                              |
| ------------------------------------------------------- | ------------------------------------------ | --------------------------------------------------- | --------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| National population census and ageing tables            | Household to province, depending on access | Limited pending documentation                       | Living arrangement, age, migration context, disability proxies        | Public tables may not preserve family distance, current responder availability, or linkable household detail.    |
| Household living-standards or ageing surveys            | Household or survey cluster                | Limited pending module review                       | Care receipt, income, health access, living arrangement               | Module content, recency, sampling error, restricted geography, and linkage permission require verification.      |
| UNFPA and National Statistics Office analyses           | National synthesis                         | Context only until underlying tables are accessible | Demographic and care-system framing                                   | Published stories do not expose all variable definitions or microdata.                                           |
| Intergenerational self-help club administrative records | Club, commune, participant                 | Limited                                             | Responder presence, visit records, service types                      | Coverage, data quality, consent, denominator, staff capacity, and access terms are unverified.                   |
| Commune health-station or NCD management records        | Facility or patient                        | Blocked pending approval                            | Referral capacity and continuity context                              | Sensitive health data, incomplete capture, incompatible identifiers, and no proof of home-response availability. |
| Social-protection and social-work case records          | Facility, case, or locality                | Blocked pending approval                            | Existing care pathways and vulnerability support                      | Sensitive data, selection bias, incomplete community coverage, and unclear reuse permission.                     |
| Prospective manual pilot event log                      | Request and visit                          | Not yet collected                                   | Acknowledgement, reach, resolution, transfer, unresolved events, cost | Requires protocol approval, consent, data minimization, safeguarding, and exit plan.                             |

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
