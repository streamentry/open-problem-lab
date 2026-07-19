# Evidence Ledger

## Current Evidence Records

The machine-readable ledger is `evidence.json`.

## Evidence Notes

### WHO Deafness and Hearing Loss Fact Sheet (2026)

The primary source for global prevalence (430M disabling hearing loss), LMIC distribution (80%), economic burden (~US$1T annually), and cost-effectiveness (US$1.40/person, 16:1 return). Updated March 2026. Use as the backbone reference for scale and tractability arguments. Do not use as a substitute for country-level coverage data.

### WHO World Report on Hearing (2021)

The strategic framework document. 252 pages synthesizing evidence on hearing loss prevalence, causes, interventions, service delivery models, and cost-effectiveness. This is the foundation reference for the field. Its limitation as a pack source is that it is a synthesis, not a primary dataset, and it does not provide a standardized sub-national coverage dataset.

### Childhood Hearing Loss Prevention

The 60% preventable childhood hearing loss figure and the 1 billion at-risk youth figure are WHO estimates useful for framing the prevention case. They are global aggregates and need country-level triangulation before use in national policy arguments.

### GBD 2019 Hearing Loss Study

This is the strongest identified source for comparable modeled prevalence because it defines hearing loss using better-ear pure-tone averages and carries uncertainty through the model. It is weaker for coverage. The model drew hearing-aid coverage inputs from 44 countries and the authors explicitly report severe regional sparsity. Use it to define need and expose uncertainty, not to claim observed country coverage.

### Ear And Hearing Care Workforce Study

The 2021 WHO-authored study is the most direct identified route to audiologist availability, covering 102 countries. It is a provenance map, not a finished baseline: six input families, different country reference years, and heterogeneous professional definitions mean that every country row needs source recovery before reuse.

### WHO Assistive Technology Progress Indicators

The 2021 GHO data distinguish hearing-related services and hearing-related human resources. That makes them useful for screening and for preserving explicit missingness. Their values remain official country responses and categorical capacity signals. They cannot be converted into audiologists per million or effective hearing-aid access.

### rATA Product-Level Negative Result

The public GHO met-need endpoint was queried on 15 July 2026. Although the dimension dictionary defines digital hearing aids and batteries as a product category, the endpoint exposed only total assistive-product categories. A hearing-aid filter returned zero rows. This blocks a hearing-aid coverage estimate from that endpoint and prevents the common error of relabeling total assistive-technology access as hearing-aid access.

## Evidence Quality Rule

Evidence is not accepted because it sounds plausible. It is accepted when the source, method, limitations, and confidence are explicit enough for a reviewer to attack. The inventory now separates four incompatible measure families: audiometric need, professional availability, categorical system capacity, and product access. None may substitute for another.

## Suggested Next Issue

Review `source-inventory` before starting the workforce baseline. The reviewer should verify the GBD source counts, the workforce study's mixed provenance, the GHO hearing-domain codes, and the rATA zero-row query. Only then should a data cleaner recover country-level audiologist numerator sources and matched population denominators.
