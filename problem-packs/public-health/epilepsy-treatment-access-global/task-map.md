# Task map

```mermaid
flowchart TD
  A["Source inventory"] --> B["Cascade measure dictionary"]
  B --> C["Setting-specific cascade baseline"]
  C --> D["Clinical, privacy, and allocation red-team"]
  D --> E["Field-reality decision check"]
  E --> F["Independent replication and publication gate"]
```

| Task                                  | Role                   | Status       | Output                                            | Gate                   |
| ------------------------------------- | ---------------------- | ------------ | ------------------------------------------------- | ---------------------- |
| `source-inventory`                    | Literature Scout       | Needs review | Dated source classification plus evidence records | Domain review          |
| `cascade-measure-dictionary`          | Data Cleaner           | Needs triage | Stage definitions and denominator rules           | Replicator             |
| `cascade-baseline`                    | Implementation Planner | Needs triage | Reproducible setting-specific baseline            | Replicator             |
| `red-team-clinical-allocation-misuse` | Red-Team Reviewer      | Needs triage | Failure-mode review and publication blocks        | Field-reality reviewer |
| `field-reality-decision-check`        | Field-Reality Reviewer | Needs triage | Named user, decision, timing, and non-use cases   | Red-team reviewer      |

The sequence is deliberate. No model, forecast, or allocation recommendation should be attempted before source identity, denominator, and event grain are reviewed.
