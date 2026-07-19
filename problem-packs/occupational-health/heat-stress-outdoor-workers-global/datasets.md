# Dataset Inventory

## Candidate Sources

### Exposure Data (Climate)

| Source                        | Grain                       | Temporal Coverage | LMIC Availability                                           | Classification                        | Reason                                                                                                                                                                                                         |
| ----------------------------- | --------------------------- | ----------------- | ----------------------------------------------------------- | ------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ERA5 reanalysis (ECMWF)       | 0.25-degree grid, hourly    | 1940-present      | Global grid, freely accessible via Copernicus CDS           | Usable for WBGT derivation            | Hourly 2m temperature, dewpoint, and radiation at 0.25 degrees permit WBGT calculation using empirical formulas. Does not capture workplace-level exposure variation. Requires registration and preprocessing. |
| MERRA-2 (NASA GMAO)           | 0.5 x 0.625 degrees, hourly | 1980-present      | Global grid, freely accessible via NASA EOSDIS              | Usable with coarser resolution caveat | Coarser than ERA5 and radiation schemes differ; useful as cross-check but not preferred for sub-national LMIC detail. Requires HDF/netCDF preprocessing.                                                       |
| National weather station data | Variable by station         | Variable          | Sparse in most LMICs; many stations inactive or non-digital | Limited                               | Station data could validate reanalysis WBGT but coverage is too sparse and inconsistent for most LMIC sub-national mapping without major digitization effort.                                                  |

### Worker Population Data

| Source                              | Grain                       | Temporal Coverage       | LMIC Availability                                                                        | Classification                            | Reason                                                                                                                                                                                                                                                             |
| ----------------------------------- | --------------------------- | ----------------------- | ---------------------------------------------------------------------------------------- | ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ILOSTAT employment-by-industry      | National; some sub-national | Annual, 1991-present    | Most ILO member states covered; informal sector partial                                  | Usable with coverage caveat               | Provides sector-level employment (ISIC 4-digit) and status-in-employment but predominantly at national grain. Informal employment indicators compiled for only a subset of LMICs. Cannot anchor district-level exposure without sub-national labor survey overlay. |
| National labor force surveys (LMIC) | National, some sub-national | Varies by country round | Exists for most countries but quality, recency, and informal sector coverage vary widely | Limited                                   | Sub-national industry breakdowns are rare and informal sector workers are undercounted. Useful where available for specific countries but not a global solution for district-level worker population denominators.                                                 |
| ILO modelled estimates              | National                    | Annual, 2000-present    | 189 countries                                                                            | Limited (modeled, not directly collected) | National-level modeled estimates fill gaps but cannot substitute for sub-national survey data. Modeled informal sector shares are especially uncertain.                                                                                                            |

### Health Outcome Data

| Source                                             | Grain                        | Temporal Coverage         | LMIC Availability                                                     | Classification                                              | Reason                                                                                                                                                                                                                                                           |
| -------------------------------------------------- | ---------------------------- | ------------------------- | --------------------------------------------------------------------- | ----------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Lancet Countdown 2024 heat-labor indicators        | Global, country-group by HDI | Annual, 2000-2023         | Country-level for selected countries; HDI-group aggregates for others | Usable for framing only                                     | Provides modeled annual potential work-hour loss (490B hours in 2023) but not sub-national district or industry-specific data. Useful for scale and trend framing only.                                                                                          |
| ILO occupational injury and death estimates (2024) | Global, country income group | Modeled annual estimates  | Global with underreporting adjustment for LMICs                       | Usable for framing only                                     | Modeled from climate-labor overlap and relative risks, not from direct surveillance. Sectoral breakdown depends on ILOSTAT which has incomplete LMIC coverage.                                                                                                   |
| Xu et al. 2021 meta-analysis                       | Multi-country pooled         | Varies by included study  | LMIC studies sparse in the pooled sample                              | Usable as effect-size reference with transferability caveat | Pooled OR 1.21 (95 percent CI 1.11-1.32) dominated by high-income country evidence. Effect size should not be generalized to LMIC tropical work settings without noting heterogeneity and transferability gaps.                                                  |
| Occupational injury registries                     | National, variable coverage  | Variable where they exist | Most LMICs have no systematic occupational injury surveillance        | Rejected for burden estimation                              | Cannot produce reliable heat-related injury counts in most LMICs because heat is not a reportable condition and surveillance systems are absent or non-functional. Retained as evidence of surveillance gaps, not as a data source for exposure-outcome mapping. |

### Standards and Frameworks

| Source                                     | Grain                  | Temporal Coverage              | LMIC Availability                                                | Classification                                            | Reason                                                                                                                                                                                                                                                     |
| ------------------------------------------ | ---------------------- | ------------------------------ | ---------------------------------------------------------------- | --------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ISO 7243:2017 WBGT standard                | International standard | Published 2017                 | Standard available for purchase globally; not context-specific   | Usable as threshold framework with acclimatization caveat | Provides WBGT reference values for work-rest regimes by metabolic rate and clothing. Paywalled beyond abstract. Reference values derived from temperate-climate laboratory studies; applicability to chronically heat-exposed tropical workers is debated. |
| WHO/ILO UV radiation joint estimate (2024) | Global modeled         | Cross-sectional                | Methodological precedent for LMIC-attributable burden estimation | Usable as methodological precedent only                   | Covers UV radiation, not heat stress. Demonstrates that global attribution of climate-linked occupational hazards is feasible. Not a data source for heat exposure-outcome mapping.                                                                        |
| Dunne et al. 2013 labor capacity model     | Regional / global grid | Projected to 2050 under RCP8.5 | Global with regional breakdown                                   | Usable as projection context only                         | Modeled future labor capacity loss under high-emission scenario. Not a current estimate and does not account for adaptation. 20 percent is a regional maximum, not a global average.                                                                       |

## Required Dataset Properties

- Exposure metric (WBGT, ambient temperature, heat index, apparent temperature).
- Data source type (ground station, reanalysis grid, satellite-derived).
- Temporal resolution (hourly, daily, monthly) and coverage period.
- Geographic grain (grid cell, district, province).
- Worker population denominator by industry and employment status (formal/informal).
- Health outcome type (injury, illness, productivity loss, mortality).
- Outcome data source (surveillance, compensation claims, household survey, study).
- Missingness patterns and representation of peak heat season.
- License or reuse permission.

## Informal Sector Coverage Assessment

Informal sector workers constitute the majority of the outdoor workforce in most LMICs (60-80 percent in many South Asian and Sub-Saharan African economies, per ILOSTAT documentation). Current data infrastructure cannot anchor a sub-national exposure-outcome map that includes informal workers because:

1. ILOSTAT informal employment indicators are modeled and available for only a subset of LMICs.
2. National labor force surveys rarely break employment by industry and informal status at sub-national grain.
3. Occupational injury surveillance systems, where they exist, cover formal sector workers with employer reporting obligations and miss own-account, unpaid family, and casual day labor workers.
4. Climate-labor exposure models (ILO, Lancet Countdown) use national workforce composition, not sub-national informal sector distributions.

This means any sub-national exposure-outcome artifact built from currently available public data would systematically underrepresent the most heat-exposed worker populations in LMICs.

## Rejection Rule

A data source is rejected for sub-national exposure-outcome mapping if exposure metric, temporal coverage, worker population denominator, or geographic grain cannot be verified. National-level labor force statistics without industry or sub-national breakdown may be listed as context but cannot anchor a district-level exposure estimate. Occupational injury data from countries without systematic surveillance is rejected as a burden estimate, though it may be retained as evidence of surveillance gaps.
