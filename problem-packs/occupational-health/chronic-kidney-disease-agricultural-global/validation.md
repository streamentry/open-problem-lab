# Validation

## Validation Layers

| Layer           | Gate                                                                                                 |
| --------------- | ---------------------------------------------------------------------------------------------------- |
| Structure       | `pnpm validate` passes schemas and problem-pack completeness checks                                  |
| Evidence        | Every source record has a dated URL, method, confidence, and specific limitations                    |
| Measurement     | CKD persistence, phenotype, etiology label, denominator, and exposure mode are documented separately |
| Reproducibility | Crosswalks and quantitative artifacts include rerunnable field-level steps and input provenance      |
| Review          | Nephrology or occupational-health domain review is recorded                                          |
| Replication     | Quantitative, causal, or field-facing outputs are independently reproduced                           |
| Safety          | Red-team and field-reality review are required before operational publication                        |

## Persistent Kidney-Disease Requirements

Any CKD or CKDu prevalence estimate must document:

- eGFR equation and creatinine assay or calibration;
- urine albumin/protein marker and collection method where available;
- repeat-test timing, with at least 90 days for a confirmed CKD classification unless the source justifies another protocol;
- how low first measurements that normalize were classified;
- how dehydration, infection, pregnancy, nephrotoxic medication, and other AKI explanations were handled;
- numerator, denominator, age/sex, worker status, industry, recruitment exclusions, and sampling frame; and
- missingness, referral, loss to follow-up, and privacy constraints.

## CKDu/CINAC Classification Requirements

No study may be called CKDu, CKDnt, CINAC, or Mesoamerican nephropathy in a cross-setting matrix without:

- the source's exact operational label;
- traditional-risk-factor exclusions and their measurement quality;
- proteinuria/albuminuria or tubular-phenotype fields;
- distinction between suspected, probable, and confirmed categories where the source provides one; and
- a non-comparability flag if another study uses a different case definition.

## Exposure Requirements

Exposure fields must distinguish:

- objective worksite temperature or heat measurements from self-reported heat;
- measured water or environmental contaminants from reported water source;
- biological samples from recalled agrochemical use;
- medication, infection, nutrition, and socioeconomic variables; and
- exposure timing relative to kidney testing and work cycle.

No association may be called causal without a prespecified design, confounding assessment, temporal ordering, uncertainty interval, domain review, and independent replication.

## Publication and Non-Use Requirements

No output may:

- diagnose an individual;
- order a pesticide ban, water restriction, work-rest rule, screening programme, or employment action;
- rank a country, employer, crop, or worker group as responsible for CKDu;
- use total CKD burden as a CKDu denominator; or
- infer a cause from a regional correlation, self-report, or single kidney-function test.

The first publishable artifact is a bounded measurement crosswalk or a negative result showing that the studies cannot be compared.
