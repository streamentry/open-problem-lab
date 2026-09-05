# Expected Outputs

## V0 Output

The first publishable output is a country- or district-bounded source and measurement crosswalk that answers:

- which primary-care facilities are in the frame;
- which water and hand-hygiene states are observed at each facility and named point of care;
- which fields measure presence, function, availability when needed, quantity, quality, supplies, stock-out, repair, or continuity;
- which values are self-reported, observed, logged, sampled, missing, refused, or not applicable; and
- which specific infrastructure, maintenance, supply, supervision, or measurement decision the artifact could inform.

The output must include a non-comparability log. If no compatible source join exists, the output should say so and identify the exact missing field, facility frame, time window, or permission needed.

## Allowed Analytical Outputs

- A dated source inventory with usable, limited, and rejected classifications.
- A field-level measurement dictionary for water and hand hygiene at primary-care facilities.
- A facility-level descriptive table or map only when the frame, geography, access permissions, missingness, and disclosure controls are explicit.
- A continuity table with a defined observation window and start/end events for outage, stock-out, repair, or replenishment.
- A negative result showing that a proposed cross-source comparison, causal estimate, or allocation ranking is not auditable.

## Prohibited Outputs

- A clinical infection-risk score, patient triage tool, or treatment instruction.
- A procurement list, engineering design, budget order, or facility sanction based only on an unreplicated assessment.
- A claim that WASH conditions caused or prevented a specific infection, maternal or newborn death, or quality-of-care outcome without a separate causal design and replication.
- A public ranking that names underperforming facilities, workers, communities, or water sources in a way that creates blame, exclusion, or security risk.
- An imputed “adequate service” value for a facility or point of care with missing, refused, or not-observed data.

## Release Gate

Any output that leaves descriptive measurement framing must name its decision-maker, beneficiary, burden bearer, data owner, reviewer, and replication record. High-safety outputs remain blocked until domain, red-team, field-reality, and independent replication review are complete.
