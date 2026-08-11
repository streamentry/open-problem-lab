# Playbooks

## Analyst Playbook

1. Read `problem.json`, `evidence.json`, `datasets.md`, and `tasks.json`.
2. Define the cascade stage and denominator before selecting a dataset.
3. Keep policy, procurement, stock, administration, timing, series completion,
   and impact outcome as separate events.
4. De-identify records before linkage and document unmatched episodes,
   duplicates, private-sector omissions, home births, migration, and reporting
   lag.
5. Treat every quantitative output as unverified until independently replicated.

## Reviewer Playbook

Ask:

1. What exact event and denominator are measured?
2. Does the source observe administration and timing, or merely describe policy,
   availability, or stock?
3. Are maternal results, prophylaxis events, birth timestamps, dose timestamps,
   and infant outcomes linked without double-counting?
4. Are home births, private care, migrants, stillbirths, and missing timing
   handled explicitly?
5. What observation would falsify the proposed bottleneck?

## Red-Team Playbook

Test whether the output could be used to stigmatize HBV-positive mothers,
coerce screening, sanction a facility for missing data, deny a child a service,
or infer clinical risk from an incomplete record. Block publication when a
reasonable misuse path has no mitigation.

## Field-Reality Playbook

Name the responsible programme user, the budget or workflow decision, the time
at which the output would be used, the data burden, the appeal path, and at
least one explicit non-use case. A reviewed bottleneck map is not a clinical
protocol and should not bypass national immunization governance.
