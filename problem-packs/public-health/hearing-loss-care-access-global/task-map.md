# Task Map

## Active Work Claims

The machine-readable task list is `tasks.json`.

## Work Sequence

```mermaid
flowchart TD
  A["Source inventory"] --> B["Workforce density baseline"]
  B --> C["Coverage gap estimation"]
  C --> D["Red-team allocation framing"]
  C --> E["Field reality check"]
  D --> F["Reviewed output"]
  E --> F
```

## Merge Discipline

Work may happen in parallel, but accepted outputs must preserve this order:

1. Evidence before estimation.
2. Workforce baseline before coverage gap.
3. Coverage estimate before red-team review.
4. Red-team review before field-facing output.
5. Field-reality review before publication.
