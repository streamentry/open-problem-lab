# Playbooks

## Measurement-First Sequence

1. Name the decision-maker and decision before collecting data.
2. Lock the need definition, population frame, geography, time window, and equity strata.
3. Inventory service, facility, routine, medicine, patient, and caregiver sources.
4. Map source fields to the cascade without filling missing joins with assumptions.
5. Verify a small, bounded service area before proposing a national comparison.
6. Replicate all calculations from locked inputs and preserve divergences.
7. Complete domain, medicines-access, red-team, and field-reality review before any allocation-facing output.

## Safe Service-Cascade States

```text
Need-defined -> Referral-offered -> Referral-accepted -> First-contact
First-contact -> Continuing-support -> Transferred -> Closed
Any state -> Lost-to-follow-up
Any state -> Unresolved-or-unsafe
```

These are data states, not clinical instructions. A referral is not a contact; a contact is not continuing support; a transfer is not closure unless the receiving service confirms completion.

## Pilot And Field Boundary

No pilot should begin from this pack alone. Before any person-level collection, the responsible institution must confirm consent, safeguarding, lawful data processing, clinical boundaries, referral ownership, medicine handling, complaints, supervision, and exit or handover. A digital dashboard is not a substitute for staffed care.

## Cheapest Disconfirming Tests

Stop or redesign before broader data collection if:

- no compatible need denominator can be constructed for the named setting
- listed services cannot be verified as operating or referral-capable
- medicine data cannot distinguish availability from consumption or appropriate use
- patients or caregivers do not freely consent or cannot withdraw safely
- providers cannot record continuing care, transfer, unresolved cases, and loss to follow-up
- data burden or privacy risk exceeds the value of the proposed decision
- the decision-maker cannot identify an allocation that the evidence would change

Future thresholds must be pre-specified with local domain and field reviewers. This pack does not invent universal acceptable coverage, response, stock, or outcome thresholds.

## Non-Obvious Second-Order Risks

- A service-count target may reward opening nominal programmes while hiding poor continuity or unreachable rural populations.
- Morphine-consumption targets may create unsafe prescribing incentives or punish facilities that appropriately restrict use.
- Measuring only people who reach care can make exclusion appear to be low need.
- Prognosis or diagnosis data may expose people to stigma, insurance discrimination, or family pressure.
- Donor-funded pilots may create short-lived services and leave patients without a safe transition when funding ends.
- Families or providers may report satisfaction while patient goals, symptoms, or caregiver burden worsen.
