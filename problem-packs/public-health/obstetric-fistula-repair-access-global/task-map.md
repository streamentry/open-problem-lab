# Task Map

## Active Work Claims

The machine-readable task list is `tasks.json`.

## Work Sequence

```mermaid
flowchart TD
  A["Source inventory"] --> B["Measurement reconciliation note"]
  B --> C["Country feasibility selection"]
  C --> D["Backlog-versus-incidence decision artifact"]
  D --> E["Red-team review"]
  D --> F["Field reality check"]
  E --> G["Reviewed output"]
  F --> G
```

## Merge Discipline

1. Source-family inventory before country selection.
2. Measurement reconciliation before any comparison.
3. Country feasibility before any ranking.
4. Red-team and field-reality review before publication.
