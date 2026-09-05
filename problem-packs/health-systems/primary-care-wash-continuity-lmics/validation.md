# Validation

## Validation Layers

| Layer              | Gate                                                                                                                                                                    |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Structure          | `pnpm validate` passes schemas, links, source-title identity, and canonical-file completeness checks.                                                                   |
| Source identity    | Every evidence record has a dated source, stable URL, access date, method, limitations, and a title that identifies one canonical source.                               |
| Service definition | Water and hand-hygiene definitions record source type, location, availability when needed, point of care, supplies, quantity, quality, and observation mode separately. |
| Continuity         | Any uptime, stock-out, repair, or availability result states its time window, start/end event, season, source of the record, and closure or unresolved state.           |
| Facility frame     | Facility type, managing authority, rurality, service area, sampling or census frame, exclusions, and missingness are visible before comparison.                         |
| Quality            | Water-quality results record sample point, date, analyte or indicator, test method, result, chain of custody, and treatment or storage context.                         |
| Reproducibility    | Any tabulation or join can be rerun from locked inputs, field definitions, checksums, and documented commands or procedures.                                            |
| Domain review      | A WASH, primary-care, and health-systems reviewer checks definitions, facility context, and transportability.                                                           |
| Red-team           | Facility blame, privacy leakage, sensitive infrastructure disclosure, false reassurance, unsafe clinical inference, and procurement overreach are tested.               |
| Field reality      | Facility managers, cleaners, health workers, patients, caregivers, WASH actors, and the named decision-maker check feasibility, burden, dignity, and fallback.          |
| Replication        | Quantitative, comparative, causal, or field-facing outputs receive independent replication before acceptance.                                                           |

## Service-State Requirements

Any water or hand-hygiene estimate must state:

- the facility and service-point frame;
- source type, improved or unimproved classification, on- or off-premises location, and distance rule;
- availability when needed, not merely availability at an unspecified visit;
- quantity proxy, storage state, pump or pipe function, repair status, and supply delivery where observed;
- sample point, quality method, result, treatment, and recontamination or storage boundary where water quality is claimed;
- named point of care or toilet, station function, water, soap or alcohol-based hand rub, hand-drying, and accessibility;
- observation, interview, logbook, sensor, sample, or record-review mode and its time window; and
- missing, refused, not observed, inaccessible, and not-applicable states.

An improved source is not automatically safe water. A functioning station at one visit is not uptime. A facility audit is not population access. A WASH or IPC measure is not a clinical outcome.

## Comparison Requirements

Cross-source comparisons are blocked unless the reviewer can reconcile:

1. facility census or sample frame;
2. facility type and managing authority;
3. service definition and minimum threshold;
4. observation date, season, and time window;
5. point-of-care or compound location;
6. self-report, observation, log, sensor, and test methods;
7. missingness, non-response, and excluded facilities; and
8. whether the output is descriptive, predictive, causal, or allocation-facing.

If the fields cannot be reconciled, retain source-specific results and document the non-comparability. Do not create a composite score to hide the mismatch.

## Claims That Remain Prohibited

Without an appropriately designed, reviewed, and replicated study, this pack cannot claim:

- that a facility's static WASH state proves continuous service, safe water, or staff compliance;
- that WASH conditions caused or prevented a named infection, maternal or newborn death, health-care-associated infection, or quality-of-care outcome;
- that one infrastructure, supply, WASH FIT, hand-hygiene, or financing intervention is universally effective;
- that a facility, district, country, worker, or community is responsible for a WASH failure;
- that missing or unobserved service data indicate adequate service;
- that a WASH score should determine procurement, financing, sanctions, clinical triage, or public ranking; or
- that a global or population-weighted gap estimate is a current primary-care facility denominator.

The first publishable artifact is a bounded source and continuity crosswalk or a negative result showing that a proposed allocation comparison is not yet auditable.
