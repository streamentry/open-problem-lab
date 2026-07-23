# Validation

## Validation Layers

| Layer           | Gate                                                                                                       |
| --------------- | ---------------------------------------------------------------------------------------------------------- |
| Structure       | `pnpm validate` passes schemas, links, and problem-pack completeness checks.                               |
| Evidence        | Every factual claim maps to a dated evidence record with method and limitations.                           |
| Denominator     | Living arrangement, family distance, functional need, consent, and responder availability remain separate. |
| Workflow        | Every request state and escalation handoff has a named, verified owner and fallback.                       |
| Safety          | Consent, privacy, safeguarding, clinical boundaries, complaints, and pilot exit are reviewed.              |
| Reproducibility | Denominator and event metrics can be rerun from documented inputs or synthetic fixtures.                   |
| Field reality   | Older people, families, responders, supervisors, and receiving services review the workflow.               |
| Replication     | Quantitative and field-facing claims receive independent replication before acceptance.                    |

## Denominator Requirements

No care-gap estimate is valid unless it states:

- age definition
- living arrangement definition
- family-distance or travel-time definition
- functional-need measure
- current care receipt
- local responder definition
- consent status
- source year, grain, weights, and missingness

Unknown family distance or responder availability remains unknown. It must not be recoded as absent.

## Event Requirements

Every pilot request requires:

- pseudonymous participant and event identifiers
- consent scope
- request type and timestamp
- acknowledgement timestamp
- reach timestamp, if reached
- closure state: resolved, transferred, or unresolved
- actor and evidence supporting closure
- adverse event, complaint, or safeguard flag
- authorized family disclosure, if any

An acknowledgement is not a response. A response is not resolution. A transfer is not resolution unless the receiving service confirms its own completion.

## Safety Stop Conditions

Field activity stops for review when:

- a serious event is missed or concealed
- consent or proxy authority is disputed
- a responder acts outside scope
- medication is changed without licensed authority
- personal data is disclosed outside recorded consent
- abuse, exploitation, fraud, or retaliation is alleged
- the promised response pathway is unavailable
- pilot exit would strand a participant without an agreed transition

## Claims That Remain Prohibited

Without an appropriately powered, reviewed study, the pack cannot claim:

- fewer deaths or hospitalizations
- prevented falls or emergencies
- improved medication adherence
- reduced depression or cognitive decline
- clinical cost savings
- safety equivalence to professional home or emergency care

Operational feasibility is necessary but not sufficient for clinical benefit.
