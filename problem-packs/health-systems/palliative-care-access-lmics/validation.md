# Validation

## Validation Layers

| Layer            | Gate                                                                                                                                                                |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Structure        | `pnpm validate` passes schemas, links, and canonical-file completeness checks.                                                                                      |
| Evidence         | Every factual claim maps to a dated record in `evidence.json` with a stable URL, method, confidence, and specific limitations.                                      |
| Denominator      | Need, service supply, facility readiness, referral, first contact, continuity, medicine access, patient/caregiver outcome, equity, and missingness remain separate. |
| Reproducibility  | Any country or district metric can be regenerated from locked inputs, field definitions, checksums, and documented code or tabulations.                             |
| Domain review    | A palliative-care and health-systems reviewer checks definitions, service boundaries, patient-centredness, and clinical non-use cases.                              |
| Medicines safety | A qualified medicines-access reviewer checks controlled-medicine, diversion, procurement, affordability, formulation, and prescribing boundaries.                   |
| Red-team         | Clinical overreach, stigma, provider blame, privacy, coercion, false reassurance, undertreatment, and unsafe medicine incentives are tested.                        |
| Field reality    | Patients, caregivers, providers, community services, and the named decision-maker or budget owner check feasibility and burden.                                     |
| Replication      | Quantitative, comparative, and field-facing outputs receive an independent replication before acceptance.                                                           |

## Need-Denominator Requirements

Any estimate of palliative-care need must record:

- the operational definition of palliative-care need or serious health-related suffering
- whether the estimate covers adults, children, all ages, specific diagnoses, or people in the last year of life
- the numerator, denominator, population frame, geography, reference date, sampling design, weights, and uncertainty
- how people outside formal facilities, people in home/community care, people in conflict or humanitarian settings, and people with non-cancer conditions are handled
- age, sex/gender where appropriate, disability, socioeconomic, rural/urban, migration, language, and other equity strata relevant to the decision
- missingness, non-response, linkage error, double counting, and temporal drift

Deaths, disease prevalence, cancer incidence, hospice enrolment, opioid consumption, and facility encounters are context or proxy measures unless the source explicitly defines them as the need denominator. A proxy must remain labelled as a proxy.

## Service And Continuity Requirements

Every service map must distinguish:

1. policy or legal recognition
2. financing or benefit-package inclusion
3. provider or programme existence
4. operating status, opening hours, catchment, and geographic reach
5. trained staff, guidance, supervision, privacy, essential medicines, and referral readiness
6. referral offered, referral accepted, first contact, assessment, care plan, follow-up, transfer, closure, and loss to follow-up
7. patient-defined goals, symptom or function measure, caregiver support, complaint, safeguarding, and consent

A directory entry, policy statement, referral, appointment, phone contact, or one recorded encounter is not evidence of continuing care. Unknown service status or missing follow-up remains unknown.

## Medicine-Access Requirements

Any medicine analysis must keep these fields separate:

- legal authorization and prescriber or facility scope
- product, formulation, strength, and procurement channel
- facility availability on a specified observation date
- stockout duration, order fulfilment, distribution, and storage
- price, affordability, insurance coverage, and patient out-of-pocket payment
- dispensing, dose or indication where lawfully and safely observable
- consumption statistics and their population coverage
- diversion-prevention, recordkeeping, training, and complaints safeguards

Morphine consumption is a distributional context indicator, not a measure of palliative-care coverage, quality, symptom relief, or appropriate use. No output may recommend relaxing controlled-medicine safeguards from this pack alone.

## Patient, Caregiver, And Data-Governance Requirements

Any person-level or household data collection requires:

- informed, voluntary, revocable consent appropriate to the participant's capacity and context
- a stated purpose, minimum necessary fields, retention period, access control, and complaint route
- separation of patient preference from family, provider, payer, or donor preference
- safe handling of sensitive diagnoses, disability, prognosis, medicine use, poverty, and caregiver information
- an explicit missingness and refusal state; refusal is not non-need or non-compliance
- safeguarding and referral procedures that are owned by an appropriate service, not by an unlicensed data collector

## Claims That Remain Prohibited

Without an appropriately powered and reviewed study, this pack cannot claim:

- reduced mortality, hospital admission, emergency use, symptom burden, or caregiver burden
- clinical equivalence of community, home, primary-care, specialist, volunteer, or digital services
- that a medicine is clinically indicated or that a shortage caused a specific patient outcome
- that opioid availability or consumption proves quality palliative care or causes better outcomes
- that a country, district, provider, clinician, patient, or caregiver is responsible for an observed gap
- that a service should be scaled, a budget reallocated, or a controlled-medicine rule changed

The first publishable artifact is a bounded, replicated measurement crosswalk or a negative result showing that the proposed allocation comparison is not yet auditable.
