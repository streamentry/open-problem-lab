# Validation

## Validation Layers

| Layer          | Gate                                                                                                                                        |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| Structure      | `pnpm validate` passes schemas, source identity, link, freshness, and problem-pack completeness checks.                                     |
| Evidence       | Every burden or pathway statement links to a dated evidence record with method, limitations, and confidence.                                |
| Data integrity | Any quantitative artifact documents grain, case definition, denominator, event timing, missingness, linkage, and selection boundaries.      |
| Review         | Public-health and health-systems domain review, red-team review, and field-reality review are recorded before programme-facing publication. |
| Replication    | Any quantitative or operational output is independently rerun from documented inputs and an input hash before it can advance.               |

## Cascade Baseline Requirements

Every baseline must document:

- The named country, district, network, or facility system and its coverage boundary.
- The episode or person grain after de-identification.
- The case definition and screening or diagnostic method for each stage.
- The event date or time window for prevention, prophylaxis, diagnosis, referral, valve care, and follow-up.
- The denominator for each stage and how transfers, duplicates, private care, migration, and loss to follow-up are handled.
- The difference between procurement, stock, dispensing, administration, attendance, adherence, diagnosis, referral, surgery, and outcome.
- The missingness and linkage-error audit, including who is absent from the records.

## Clinical And Allocation Gate

No artifact may be called actionable until it includes:

- the named decision user and decision;
- the observed setting and lead time, if any;
- the false-positive and false-negative or exclusion costs;
- explicit non-use cases;
- domain, red-team, and field-reality review;
- independent replication where the artifact is quantitative or could change resource allocation.

## Kill Conditions For The Pack's Central Hypothesis

The central hypothesis is that a carefully defined cascade measurement can reveal a decision-relevant bottleneck that is invisible in global burden or hospital-only data. It should be narrowed or retired if:

- no named setting can observe at least two cascade stages with defensible denominators after a documented source search;
- apparent bottlenecks disappear entirely under plausible linkage, private-sector, or missingness corrections;
- stage definitions cannot be made comparable without collapsing clinically distinct events; or
- domain and field reviewers find that the output cannot change a real programme decision without unsafe clinical or equity overreach.
