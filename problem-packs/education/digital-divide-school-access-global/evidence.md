# Evidence Ledger

## Current Evidence Records

The machine-readable ledger is `evidence.json`.

## Evidence Notes

### UNICEF/ITU Digital Divide 2020

Use this source for the global digital divide baseline. The 1.3 billion figure is from 2020 — connectivity may have improved since then but change is not systematically tracked. School connectivity estimates are modeled from surveys, not direct measurement. The 'two-thirds of schools' figure is a low-income-country aggregate masking enormous country-level variation. Always document data year and sub-national variation limitations.

### Giga Project Connectivity 2024

Use Giga as the most comprehensive school-connectivity dataset. Satellite-based classification may misclassify intermittent or mobile-only connectivity. Coverage is concentrated in partner countries. Connectivity classification is a snapshot, not a measure of educational usage. The ML-based school detection has variable false-positive and false-negative rates. Always document classification methodology and coverage limitations.

### Connectivity Quality Dimension

Use this source to document that connectivity existence does not equal educational utility. Electricity, devices, teacher digital literacy, and relevant content are all necessary conditions. Bandwidth requirements vary by content type. Teacher digital-literacy data is almost entirely absent. Always present connectivity claims with quality-dimension caveats.

### School Census ICT Data Limitations and UIS 4.a.1 Definitions

Use the UIS 4.a.1 metadata to keep electricity, internet for pedagogical purposes, and computers for pedagogical purposes as separate fields. It is a definitions source, not proof that a country's school census is current, complete, or independently validated. Always document the country-specific data year, reporting completeness, definitions, and cross-validation status.

### ITU DataHub Household ICT Indicators

Use ITU DataHub for national household and individual ICT context, not school-level localization. Retain the indicator year and metadata for every downloaded series. It is a plausible external check on national connectivity conditions, but it cannot validate which schools are connected.

### GSMA Mobile Connectivity Index

Use the GSMA methodology as a country-level mobile-connectivity context layer. Its composite score is not a school-coverage measure and must not be presented as proof of reliable school internet, electricity, devices, or educational use.

### UNESCO UIS ICT-in-Education Measurement Guide

Use the 2011 UIS guide for historical measurement concepts and administrative-data field design. Treat it as guidance, not as observed evidence of current sub-national connectivity or data completeness; do not describe it as a 2024 source.

### Giga Mapping Service and API

Use Giga's mapping documentation for the source architecture and API surface: government partner data, open data, satellite/ML refinement, and local validation campaigns can coexist in one map. Treat the result as a multi-source compilation. Preserve each layer's source, date, definition, and coverage rather than calling the map ground truth.

### Giga Meter School Performance

Use Giga Meter for the quality dimension: repeated download, upload, latency, and uptime observations can complement a binary connectivity status. The source does not establish national representativeness, all-day reliability, electricity continuity, devices, teacher capability, content, or educational use.

### UIS World Education Statistics 2024

Use this report for data-currency context only. It explicitly distinguishes the latest available SDG 4.a.1 data year from a more representative earlier sample. Retain both fields when comparing global or regional benchmarks, and never convert an aggregate into a school or district map.

### Giga Maps Backend Data-Source Configuration

Use the commit-pinned configuration to inspect how connectivity status/type and quality-of-service fields are separated before extracting data. It is marked DRAFT and contains no observations, so it cannot validate coverage, accuracy, missingness, or cross-validation.

## Cross-Validation Rule

The inventory identifies candidate comparisons but does not perform one. A future country analysis must join Giga school records to an independent school census or field/performance source using a documented school identifier or spatial matching rule, preserve unmatched records, report the match rate, and compare definitions before estimating disagreement. A source listed as “candidate independent check” is not evidence that validation has occurred.

## Evidence Quality Rule

Evidence is not accepted because it sounds plausible. It is accepted when the source, method, limitations, and confidence are explicit enough for a reviewer to attack.
