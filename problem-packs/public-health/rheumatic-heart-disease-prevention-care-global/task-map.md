# Task Map

## Active Work Claims

The machine-readable task list is `tasks.json`.

## Work Sequence

```mermaid
flowchart TD
  A["Source inventory"] --> B["Cascade measure dictionary"]
  B --> C["De-identified baseline and linkage audit"]
  C --> D["Implementation comparison"]
  C --> E["Red-team review"]
  D --> F["Field-reality review"]
  E --> F
  F --> G["Replicated programme-facing artifact"]
```

## Merge Discipline

Work may happen in parallel, but canonical outputs preserve this order:

1. Evidence before claims.
2. Measure definitions before aggregation.
3. Denominator and missingness audit before comparison.
4. Domain review before clinical or allocation interpretation.
5. Red-team and field-reality review before publication.
6. Independent replication before any quantitative output is treated as accepted knowledge.
