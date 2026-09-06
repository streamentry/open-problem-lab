# Evidence Ledger

## Interpretation Rule

Each record states what a dated source can support at its own grain. The ledger does not turn a facility service ladder into uptime, an improved water source into safe water, a WASH FIT score into clinical benefit, or a national financing statement into a facility allocation. Every quantitative or operational statement in this pack must point to an evidence ID in `evidence.json`.

## Current Records

| Evidence ID                              | Source layer                                   | What it supports                                                                                                               | Confidence | Boundary                                                                                  |
| ---------------------------------------- | ---------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ | ---------- | ----------------------------------------------------------------------------------------- |
| `jmp-wash-hcf-2024`                      | WHO/UNICEF global data update                  | Dated global no-service estimates, older basic-service estimates, and the current data-coverage limitation                     | high       | Broad health-care-facility context; not primary-care-only, continuous, or causal          |
| `who-unicef-wash-hcf-tracker-2025`       | WHO/UNICEF country tracker update              | Country-level standards, baselines, financing, and tracker coverage                                                            | high       | Not facility uptime, expenditure amount, service quality, or impact                       |
| `who-hcf-wash-core-2018`                 | WHO/UNICEF monitoring guideline                | Harmonized service definitions and candidate questions                                                                         | high       | Normative instrument, not current observed coverage or continuity                         |
| `who-hhfa-comprehensive-guide-2023`      | WHO facility-assessment framework              | Sampling, audit, observation, interview, record-review, and interpretation methods                                             | high       | Point-in-time facility capacity, not daily service or population access                   |
| `who-hhfa-combined-questionnaire-2023`   | WHO facility questionnaire                     | Concrete availability, readiness, management, and finance collection structure                                                 | high       | Instrument is not evidence that the fields were collected or linked                       |
| `who-wash-fit-guide-2022`                | WHO facility improvement guide                 | Facility-led risk assessment and improvement-cycle design                                                                      | high       | Adaptation and implementation guidance, not representative or causal evidence             |
| `guo-rural-hcf-wash-2017`                | Primary multicountry facility study            | Rural facility access, continuity, quality, quantity, reliability, and water-quality measurement                               | high       | Six-country rural cross-section; not current global or primary-care-only coverage         |
| `kanyangarara-wash-hcf-2021`             | Primary secondary analysis of facility surveys | Historical 18-country sub-Saharan African comparison and its definition gap                                                    | high       | 2013–2018 survey data; not later basic-service or uptime evidence                         |
| `washfit-togo-pilot-2018`                | Primary implementation evaluation              | Repeated WASH FIT assessment, facility-led change, and implementation barriers                                                 | high       | Three selected facilities, no comparator, no causal or transportability claim             |
| `who-ipc-global-report-2024`             | WHO global IPC report                          | Why WASH conditions and IPC implementation belong in the same decision context                                                 | high       | IPC status and WASH conditions are not interchangeable or a WASH treatment effect         |
| `who-wash-hcf-framework-2024`            | WHO/UNICEF global framework                    | Named policy, financing, and implementation decision pathway                                                                   | high       | Global framework is not local performance or an allocation recommendation                 |
| `washfit-global-report-2025`             | WHO/UNICEF implementation report               | Current implementation and scaling context for WASH FIT                                                                        | high       | Selected cases and implementation analysis are not a representative continuity estimate   |
| `ayalew-amhara-hcf-wash-continuity-2025` | Primary Ethiopia mixed-methods study           | Health-centre service standards, continuity/adequacy bottlenecks, maintenance, point-of-care hygiene, and citizen report cards | high       | Three woredas; cross-sectional; not a national denominator, time series, or causal effect |

## Measurement Breaks That Must Stay Separate

### Service ladder versus continuity

The JMP and core-question records provide a shared language for no, limited, and basic service. A facility may still fail on days when its source is dry, a pump is broken, a tank is empty, a pipe is contaminated, soap is out of stock, or a station is inaccessible. A point-in-time basic-service observation is therefore a baseline state, not an uptime estimate.

### Facility versus patient or population

HHFA, SARA, SPA, and WASH FIT observe facilities or facility staff. They do not by themselves establish how many people can reach the facility, whether all service areas are open, whether patients receive care, or whether an infection or death was caused by a WASH failure. Population-weighted figures in the JMP update are useful for global context but must not be substituted for a primary-care facility denominator.

### Availability versus quality and quantity

An improved source classification does not establish microbial safety. A source that is safe at collection may be recontaminated in transport or storage. The Guo study is useful precisely because it measured source conditions, continuity, quantity, reliability, and _E. coli_ separately. Future work must preserve these fields rather than create one composite “water access” number.

### Point of care versus compound presence

Hand hygiene must be mapped to named points of care and toilets, with the station's function, water, soap or alcohol-based rub, hand-drying, accessibility, and observation time recorded. A toilet or tap elsewhere on the compound is not evidence that a clinician, patient, cleaner, or caregiver can use a functioning station at the moment of care.

### Improvement process versus health outcome

The Togo pilot and WASH FIT records support a feasible improvement process and show why repeated assessments can reveal non-uniform change. They do not prove fewer infections, lower mortality, greater care seeking, or cost-effectiveness. Any downstream outcome analysis needs its own patient, exposure, confounding, and replication design.

### New country-bounded continuity evidence

The 2025 Ethiopia study is a useful primary addition because it observes the distinction this pack is designed to preserve: a water-service standard includes continuous functionality at each premises, while the field assessment still found continuity, adequacy, maintenance, water-quality capacity, and nonfunctional handwashing stations as bottlenecks. It also combines facility observation with citizen report cards. The study does not turn those observations into a national gap estimate or a causal service-delivery recommendation; it is a country-bounded source for testing the next facility-frame and continuity crosswalk.

## Discovery Handoff

The selected discovery wedge is ready for a first source-inventory contribution. A contributor should inventory country and facility records that can answer, separately:

1. whether water is available when needed;
2. how much water is available and where it is distributed;
3. whether the water is tested or treated and how quality is maintained;
4. whether hand-hygiene stations function at named points of care and toilets;
5. whether soap, alcohol-based hand rub, hand-drying, pumping, storage, and repairs are observable; and
6. which data are missing, refused, not applicable, or not representative.

The first task must not produce a country ranking or a procurement recommendation. It should either identify a compatible facility-level path in one named setting or document why the proposed comparison is not auditable. The Ethiopia study is a candidate starting point for the next country-bounded crosswalk, not a completed replication. A negative result is a valid completion if the method and the blocked join are explicit.

## Source Decay

JMP estimates, national trackers, facility assessments, and WASH FIT implementation records have different update cycles. Before any country-facing output, refresh the facility frame, service definitions, financing status, water-quality method, continuity window, and point-of-care observations. If a source moves or a national instrument changes, preserve the historical record and create a dated replacement rather than silently overwriting the series.
