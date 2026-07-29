# Congenital Chagas Cascade Pack

## Overview

This pack measures completion of the maternal-newborn Chagas prevention cascade. It does not provide diagnosis or treatment advice.

## Key Components

- `problem.json`: scope, safety level, canonical files, and review gate.
- `evidence.json`: dated source records with claim grain and limitations.
- `datasets.md`: source-family and measurement boundaries.
- `tasks.json`: one scoped literature-scout task followed by staged analysis and review tasks.

## Diagrams

```mermaid
flowchart LR
  Evidence["Evidence"] --> Measures["Cascade measures"]
  Measures --> Data["De-identified records"]
  Data --> Audit["Linkage and missingness audit"]
  Audit --> Review["Domain, red-team, field review"]
```

```mermaid
sequenceDiagram
  participant MoH as Program decision-maker
  participant Data as De-identified data
  participant Analyst
  participant Reviewer
  MoH->>Analyst: Ask where cascade support is failing
  Analyst->>Data: Build stage-level table
  Analyst->>Reviewer: Submit methods, limits, and non-use cases
  Reviewer-->>MoH: Approve, block, or require replication
```
