# Validation

## Validation Layers

| Layer               | Gate                                                                                                                                                                   |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Structure           | `pnpm validate` passes schemas, links, and canonical-file completeness checks.                                                                                         |
| Evidence            | Every factual claim maps to a dated record in `evidence.json` with a stable URL, method, confidence, and specific limitations.                                         |
| Denominator         | Fall events, injuries, mortality, facility presentations, time-to-care, rehabilitation, and functional recovery remain separate.                                       |
| Reproducibility     | Any estimate or effect can be regenerated from locked inputs, field definitions, checksums, and documented code or tabulations.                                        |
| Domain review       | An injury-prevention, gerontology, rehabilitation, or health-systems reviewer checks definitions, clinical boundaries, and transportability.                           |
| Intervention review | Trial allocation, eligibility, fidelity, co-interventions, outcome instruments, attrition, and follow-up are checked against the primary source.                       |
| Red-team            | Age or disability discrimination, unsafe home entry, medication changes, automated targeting, victim blame, privacy, false reassurance, and denial of care are tested. |
| Field reality       | Older adults, caregivers, community workers, emergency providers, rehabilitation services, and the named decision-maker check feasibility and burden.                  |
| Replication         | Quantitative, comparative, causal, and field-facing outputs receive independent replication before acceptance.                                                         |

## Fall-Event Requirements

Any fall estimate must record:

- the fall definition and whether the event was witnessed, self-reported, caregiver-reported, clinically assessed, or registry-abstracted
- age boundary, sex/gender where appropriate, residence, setting, activity, mechanism, intent, and recurrence window
- the numerator, denominator, population or facility frame, sampling design, weights, reference period, and uncertainty
- whether the estimate counts all falls, injurious falls, medically attended falls, admitted cases, fractures, or deaths
- whether people who did not seek formal care are observable and how under-reporting or non-response is handled
- missingness, failed linkage, recall, survivor, selection, and loss-to-follow-up bias

WHO global fall estimates and facility registries are context or care-pathway measures unless their source explicitly defines a compatible population denominator. A facility count must not be relabelled as incidence.

## Injury And Time-to-Care Requirements

Every care-pathway extract must distinguish:

1. event time and place
2. decision to seek care
3. departure and transport mode
4. arrival at first facility
5. clinical assessment and injury severity
6. admission, treatment, surgery or fracture care
7. transfer, rehabilitation referral, attendance, and functional follow-up
8. death, unresolved care, refusal, and loss to follow-up

An arrival interval that includes care-seeking delay is not transport time. A discharge record is not functional recovery. A rehabilitation referral is not rehabilitation receipt.

## Intervention And Causal Requirements

Any intervention analysis must preserve:

- trial or quasi-experimental design, cluster and participant allocation, eligibility, comparator, and contamination
- intervention components, delivery owner, dose, attendance or exposure, fidelity, co-interventions, and adverse events
- outcome definition, observation window, instrument/version, missingness, attrition, and analysis population
- effect measure, uncertainty interval, prespecified analysis, and limitations on transportability

The FAMILY trial is evidence that one bundled primary-care intervention was evaluated in rural China. It is not evidence that the same effect holds in every LMIC or for excluded high-risk groups.

## Patient, Caregiver, And Data-Governance Requirements

Any person-level or household data collection requires:

- informed, voluntary, revocable consent appropriate to capacity and context
- a minimum necessary data plan, retention period, access control, complaint route, and secure linkage
- participant choice about home entry, caregiver contact, environmental assessment, and disclosure
- separate refusal, unable-to-contact, and missing states; refusal is not non-need or non-compliance
- safeguarding and referral procedures owned by an appropriate service, not an automated model or unlicensed collector

## Claims That Remain Prohibited

Without an appropriately powered and reviewed study, this pack cannot claim:

- that a specific person will fall or that a risk score is clinically valid
- reduced mortality, fractures, admissions, disability, or caregiver burden from a cross-sectional, registry, or self-reported result
- that a risk factor is causal or that a household, provider, older person, or community is responsible for falls
- universal effectiveness of exercise, home modification, medication review, vitamin supplementation, education, or digital monitoring
- that fewer reported falls proves fewer serious injuries or better functional recovery
- that a prevention, transport, fracture-care, rehabilitation, housing, or budget programme should be scaled without the named decision, field review, and independent replication

The first publishable artifact is a bounded source/case-definition crosswalk or a negative result showing that an incidence, care-delay, or intervention comparison is not yet auditable.
