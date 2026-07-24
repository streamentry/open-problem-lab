# Long-Distance Elder Care In Viet Nam

## Overview

This pack investigates whether older people with distant family lack timely local response. Keep monitoring, acknowledgement, physical reach, resolution, transfer, and clinical outcome as separate states.

## Key Components

- `evidence.json` and `datasets.md`: source claims and the incompatible measure families behind the care-gap denominator.
- `tasks.json` and `task-map.md`: evidence-to-field sequencing and review ownership.
- `playbooks.md`: the canonical master plan, manual-service gate, disconfirming tests, trade-offs, and software authorization rule.
- `playbooks-vietnamese.md`: the Vietnamese operational translation. Keep it aligned with `playbooks.md`; it does not replace the canonical plan.
- `validation.md`: denominator, event-state, consent, safeguarding, and prohibited-claim gates.
- `outputs.md`: candidate artifacts and mandatory non-use language.

## Diagrams (Mermaid)

### Flowchart

```mermaid
flowchart TD
  A["Source inventory"] --> B["Care-gap denominator"]
  B --> C["Verified responder workflow"]
  C --> D["Manual service protocol"]
  D --> E["Red-team and field review"]
  E --> F["Stop, iterate, or authorize software"]
```

### Component Diagram

```mermaid
flowchart LR
  Evidence["Evidence and datasets"] --> Denominator["Care-gap denominator"]
  Denominator --> Workflow["Local response workflow"]
  Workflow --> Pilot["Manual pilot"]
  Pilot --> Safety["Safety and field review"]
  Safety --> Decision["Go, iterate, or stop"]
```

### Sequence Diagram

```mermaid
sequenceDiagram
  participant Elder as Older person
  participant Family as Distant family
  participant Responder as Local responder
  participant Service as Clinical or social service
  Elder->>Responder: Consented request
  Responder->>Elder: Reach and assess within scope
  Responder->>Service: Transfer when outside scope
  Service-->>Responder: Confirm receipt
  Responder-->>Elder: Confirm resolution or unresolved state
  Responder-->>Family: Minimal authorized update
```
