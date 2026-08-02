# Obstetric Fistula Repair Access Pack

## Overview

This pack separates untreated prevalent fistula, incident prevention failure, repair output, repair outcomes, and self-reported symptoms. Evidence must identify its measurement family before it is used in an allocation argument.

## Key Components

- `problem.md`: bounded allocation question, scope, and prohibited uses.
- `evidence.json` and `evidence.md`: dated source records with claims and limitations.
- `datasets.md`: source inventory with numerator, denominator, time, grain, and case-finding boundaries.
- `tasks.json`: staged source-inventory, reconciliation, feasibility, red-team, and field-reality work.
- `validation.md`: comparison, replication, and allocation-signal gates.

## Diagrams (Mermaid)

### Measurement flow

```mermaid
flowchart LR
  Symptoms["Self-reported symptoms"] --> Proxy["Proxy measurement"]
  Confirmed["Confirmed cases"] --> Backlog["Untreated backlog"]
  EmOC["Functioning EmOC"] --> Prevention["Prevention-capacity signal"]
  Repairs["Repair records"] --> Outcomes["Repair output and outcomes"]
  Proxy -. "not equivalent" .-> Backlog
  Prevention -. "upstream proxy" .-> Backlog
  Outcomes -. "not proof need fell" .-> Backlog
```

### Allocation review sequence

```mermaid
sequenceDiagram
  participant Scout as Literature Scout
  participant Source as Source record
  participant Reviewer as Domain reviewer
  participant Decision as Program decision-maker
  Scout->>Source: Classify family, numerator, denominator, time, grain
  Scout->>Reviewer: Submit claim and limitations
  Reviewer->>Source: Attack comparability and case-finding gaps
  Reviewer-->>Decision: Release only bounded signals
  Decision-->>Source: Do not rank backlog without missing fields
```
