# Task Map

## Active Work Claim

The machine-readable task list is `tasks.json`. Only `source-inventory` is currently scoped.

## Work Sequence

```mermaid
flowchart TD
  A["Source inventory"] --> B["Care-gap denominator"]
  B --> C["Local response workflow"]
  C --> D["Manual service pilot protocol"]
  D --> E["Red-team safety and autonomy"]
  D --> F["Field reality and economics"]
  E --> G["Reviewed go, iterate, or stop decision"]
  F --> G
  G --> H["Software design only if manual service survives"]
```

## State Machine

```mermaid
stateDiagram-v2
  [*] --> Requested
  Requested --> Acknowledged
  Acknowledged --> Reached
  Reached --> Resolved
  Reached --> Transferred
  Requested --> Unresolved
  Acknowledged --> Unresolved
  Transferred --> Unresolved
  Resolved --> [*]
  Transferred --> [*]
  Unresolved --> SafetyReview
```

## Merge Discipline

1. Evidence before denominator.
2. Denominator before market size.
3. Verified responders before alerts.
4. Manual service before software.
5. Operational reliability before clinical claims.
6. Red-team, field-reality, and replication review before field use.
