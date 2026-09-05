# Measurement Playbook

## Purpose

This playbook is a measurement protocol skeleton, not a WASH engineering or clinical guide. It is designed to help a named health-system team test whether its facility data can identify the binding water or hand-hygiene continuity constraint before requesting an intervention.

## Measurement Sequence

### 1. Lock the facility frame

Record the facility census or sampling frame, level, managing authority, rurality, service area, operating schedule, maternity or other relevant care points, and facilities excluded from the frame. Do not call a convenience sample a district denominator.

### 2. Define the service state

For water, record source type, location, availability when needed, storage, pumping or pipe function, quantity proxy, treatment, quality test, and the observation or log window. For hand hygiene, record the named point of care or toilet, station function, water, soap or alcohol-based hand rub, hand-drying, accessibility, stock-out, and observation time.

### 3. Define the failure event

Choose the event before extracting data. Examples include “water unavailable at the named point of care during the observation,” “soap absent at the station at the visit,” “source outage began,” “repair request opened,” or “replenishment completed.” A failure must have an owner, timestamp, and closure state where the source supports it.

### 4. Triangulate without erasing disagreement

Compare direct observation, staff report, logbook, sensor, water-quality sample, stock record, maintenance ticket, and patient-exit data only after recording their different observation windows and units. Disagreement is a result to investigate, not a missing value to average away.

### 5. Preserve missingness and consent

Use separate states for missing, refused, not observed, not applicable, inaccessible, and no service. Store only the minimum necessary facility or person data. Facility and worker identifiers should be de-identified or access-controlled before analysis; precise vulnerable-source locations should not be published.

### 6. Name the decision and stop rule

State whether the artifact is intended to inform a source, storage, pumping, supply, maintenance, supervision, or monitoring decision. If the data cannot identify the relevant failure at the relevant care point or time window, stop at a negative result. Do not convert the gap into a procurement recommendation.

## Minimum Crosswalk

| Measurement family           | Minimum fields                                                                                                                    | Must not be called                      |
| ---------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------- |
| Source and location          | source type, improved/unimproved classification, on/off premises, distance rule, facility and care-point location                 | safe or continuous water                |
| Availability and continuity  | when-needed definition, observation window, outage or stock-out start/end, season, repair or replenishment state                  | uptime if only observed once            |
| Quantity and storage         | volume or proxy, tank/storage status, pump/pipe state, delivery interval                                                          | sufficient for all care                 |
| Water quality                | sample date, analyte or indicator, collection point, test method, result, chain of custody                                        | safe water if only source type is known |
| Hand hygiene                 | named point of care/toilet, station function, water, soap or alcohol-based hand rub, hand-drying, accessibility, observation time | staff compliance or infection reduction |
| Patient or population access | catchment frame, travel or referral information, patient report, service use                                                      | facility service availability           |
| Clinical outcome             | case definition, exposure timing, confounders, follow-up, outcome adjudication                                                    | causal effect of WASH                   |

## Stop Conditions

Stop and label the output “not auditable for allocation” if:

- the facility frame cannot be reconstructed;
- the time window is absent for a continuity claim;
- source presence is being used as a proxy for quality or quantity without a stated bridge;
- the point of care is unknown;
- missing or refused observations are silently coded as adequate;
- the analysis identifies a facility or worker for blame rather than a service failure; or
- the proposed output would be used for procurement, clinical action, sanction, or public ranking before the required reviews and replication.
