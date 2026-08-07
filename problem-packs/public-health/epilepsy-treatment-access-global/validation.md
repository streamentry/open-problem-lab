# Validation and merge gates

## Structural gates

- `problem.json` validates against `schemas/problem.schema.json`.
- Every task in `tasks.json` validates against `schemas/task.schema.json`.
- Every record in `evidence.json` validates against `schemas/evidence.schema.json`.
- Every path listed in `problem.json.canonical_files` exists.
- Evidence source URLs have one canonical title across the repository.

## Evidence gates

Before a source is classified as usable, a reviewer must verify:

- source title, URL, source date, access date, and method;
- case definition and whether the source measures active epilepsy, seizure history, diagnosis, treatment, stock, dispensing, possession, adherence, seizure control, referral, or outcome;
- numerator, denominator, geographic grain, time reference, and missingness;
- whether the source is observed, self-reported, modeled, or commercial;
- at least one specific limitation that blocks an over-broad interpretation.

## Cascade gates

No cascade artifact can be accepted unless it keeps these measures distinct:

1. population or screened denominator;
2. active-epilepsy or case-ascertainment definition;
3. diagnosis or registration;
4. treatment initiation;
5. medicine stock, dispensing, possession, refill continuity, and affordability;
6. adherence or self-reported use;
7. seizure control or clinical outcome;
8. follow-up, referral completion, and loss to follow-up.

Unknown, unobserved, transferred, and outside-system events must remain explicit categories. They must not be counted as untreated, controlled, or failed care.

## High-safety gates

Any output that could affect clinical care, medicine procurement, workforce deployment, or programme ranking requires:

- public-health or health-systems domain review;
- red-team review of clinical, privacy, stigma, equity, and allocation misuse;
- field-reality review of the named user, decision, timing, and non-use case;
- independent replication with an input hash and environment note;
- explicit publication blocking if the evidence cannot support the proposed interpretation.

## Repository commands

Run from the repository root:

```bash
pnpm validate
pnpm reproducibility:check
pnpm verify:sources
pnpm build
pnpm format:check
git diff --check
```

`pnpm build` must be run after any task or problem-pack change so that `tasks-available.json`, `agent-radar.json`, and generated Wiki pages remain synchronized. `docs/wiki/` is generated and must not be hand-edited.
