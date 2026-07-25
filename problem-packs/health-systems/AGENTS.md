# Health Systems Packs

## Overview

Health-systems packs must separate national policy or supply indicators from facility-level service performance. Blood availability is a high-safety example: readiness, stock interruption, referral delay, compatibility, issue, and transfusion are different measurements.

## Key Components

- Pack-local `problem.json` and `problem.md`: decision, scope, and non-use boundaries.
- Pack-local `tasks.json`: staged roles, reviewer routing, and safety risk.
- Pack-local `evidence.json` and `datasets.md`: source grain, indicator definitions, and provenance.
- Pack-local `validation.md`, `outputs.md`, and `playbooks.md`: replication and field-use gates.

## Diagrams (Mermaid)

### Flowchart

```mermaid
flowchart TD
  A["National supply evidence"] --> B["Facility readiness and interruption measures"]
  B --> C["Referral, compatibility, issue, and transfusion records"]
  C --> D["Domain and red-team review"]
  D --> E["Replicated field-use decision"]
```

### Component Diagram

```mermaid
flowchart LR
  Problem["problem.*"] --> Tasks["tasks.json"]
  Tasks --> Evidence["evidence.json / datasets.md"]
  Evidence --> Validation["validation.md"]
  Validation --> Outputs["outputs.md / playbooks.md"]
```

### Sequence Diagram

```mermaid
sequenceDiagram
  participant Contributor
  participant Source as Source inventory
  participant Facility as Facility data
  participant Reviewer as Domain and red-team reviewers
  participant Replicator
  Contributor->>Source: Classify grain and limitations
  Source->>Facility: Define measurable pathway
  Facility->>Reviewer: Submit bounded artifact
  Reviewer->>Replicator: Require independent rerun for quantitative use
  Replicator-->>Reviewer: Confirm or reject reproducibility
```
