# Master Plan

## Strategic Thesis

The product is verified local response, not remote observation. Software is deferred until a manual service proves that older people want it, responders can deliver it, escalations close reliably, and the full labor and supervision cost is supportable.

## Named Users And Decisions

| User                            | Decision                                                                                   |
| ------------------------------- | ------------------------------------------------------------------------------------------ |
| Older person                    | What assistance and information sharing to accept, refuse, or revoke.                      |
| Distant family member           | Whether a verified local service is needed and which escalation role to retain.            |
| Local responder or supervisor   | Whether a request is routine, urgent, outside scope, resolved, transferred, or unresolved. |
| Commune or primary-care partner | Whether an older person should enter an existing assessment or referral pathway.           |
| Program operator                | Whether to stop, redesign, continue manually, or authorize software development.           |

## Phase 0: Define The Service Boundary

1. Choose one compact service area.
2. Define "older person," "distant family," and a meaningful response window without claiming those thresholds are nationally valid.
3. Separate companionship, activities-of-daily-living support, care coordination, clinical care, and emergency response.
4. Record services explicitly excluded.
5. Name the licensed clinical and emergency services that retain responsibility.

Exit gate: every service class has an owner, a non-use case, and an escalation destination.

## Phase 1: Measure The Care-Response Gap

Construct separate fields for:

- living arrangement
- older-person preferences
- functional need
- existing paid and unpaid care
- family travel time and actual availability
- trusted neighbor or community support
- local service availability
- communication access

Do not publish a market-size estimate when any load-bearing field is absent. Report an identified subset and an unknown remainder.

Exit gate: a replicator can reconstruct the denominator and missingness.

## Phase 2: Verify The Local Response Network

For each responder and fallback:

1. verify identity, role, training, hours, catchment, travel mode, and supervision
2. test the contact path
3. identify tasks they may and may not perform
4. document handoff to primary care, social work, family, and emergency services
5. record what happens when nobody is available

Exit gate: no safety pathway ends at an unverified listing, volunteer assumption, or unanswered number.

## Phase 3: Run A Manual Concierge Pilot

The proposed starting design is a small six-week operational pilot using telephone, existing messaging tools, and structured forms. The sample size is for workflow learning, not health-effect estimation.

Candidate service functions:

- scheduled consented check-in
- medication-list and appointment reconciliation without prescribing
- basic home-safety observation
- companionship and service navigation
- local visit when a prespecified non-clinical trigger occurs
- transfer to licensed or emergency services when outside scope
- verified closure update to the older person and authorized family

Required event states:

`requested -> acknowledged -> reached -> resolved | transferred | unresolved`

Required metrics:

- eligible, approached, enrolled, refused, and withdrawn counts
- scheduled check-in completion
- response and reach time distributions
- resolved, transferred, and unresolved events
- false or unnecessary escalations
- privacy, safeguarding, and complaint events
- older-person and responder burden
- travel, labor, supervision, and communication cost
- family payment or public-funding evidence, kept separate from stated interest

This pilot must not estimate mortality reduction, emergency prevention, hospital avoidance, or clinical efficacy.

## Phase 4: Cheapest Disconfirming Tests

Stop or redesign before software if any of the following holds:

- older people do not freely consent or withdraw frequently because the service feels intrusive
- no reliable local responder can reach participants inside the promised service window
- unresolved events are hidden, reclassified, or systematically concentrated outside staffed hours
- responder travel and supervision cost exceeds credible funding
- families value reassurance but will not fund the human service behind it
- local services cannot accept transfers
- the service increases conflict, coercion, fraud, neglect, or unsafe medication handling

Thresholds for a future go/no-go decision must be preregistered with local reviewers. This pack does not invent universal acceptable rates.

## Phase 5: Software Authorization

Software may be proposed only after the manual service survives Phases 0-4. The first software should reduce verified operational friction:

- consent and proxy records
- scheduling
- structured event states
- escalation routing
- audit trail
- minimal authorized family updates
- unresolved-event review

Do not begin with continuous surveillance, predictive risk scores, automated diagnosis, or opaque prioritization.

## Trade-Offs

| Choice                  | Benefit                                    | Cost or failure mode                                               |
| ----------------------- | ------------------------------------------ | ------------------------------------------------------------------ |
| More monitoring         | Earlier signals may be available           | Surveillance, false alarms, loss of autonomy, and unstaffed alerts |
| Faster response promise | Strong family value proposition            | Higher staffing cost and catastrophic failure when coverage breaks |
| Volunteer network       | Lower direct cost and community legitimacy | Variable availability, burnout, supervision, and safeguarding risk |
| Paid workforce          | Clearer accountability and availability    | Higher price, recruitment constraints, and rural unit economics    |
| Family dashboard        | Reassurance and coordination               | Family pressure, privacy leakage, and false confidence             |
| Narrow geography        | Better density and supervision             | Lower initial reach and weaker generalizability                    |

## Non-Obvious Second-Order Risks

- Distant relatives may substitute purchased reassurance for meaningful involvement.
- Providers may select healthier, denser, wealthier households to improve metrics.
- Volunteers may become an unrecognized clinical workforce without training or protection.
- A dashboard may make an unresolved event appear managed because it was acknowledged.
- Successful pilots may disappear when grant funding ends, leaving dependency without continuity.
- Household risk data may attract fraud, exploitation, or discriminatory pricing.

## Final Decision Rule

Proceed to software only when independent review finds that:

1. the target denominator is measurable
2. consent and autonomy are real
3. the responder network closes requests
4. unresolved events remain visible
5. unit economics include human delivery and supervision
6. public and clinical services accept their handoffs
7. the service remains valuable without claiming unmeasured health benefits
