# Evidence Ledger

## Current Evidence Records

The machine-readable ledger is `evidence.json`.

## Evidence Notes

### ILO Heat Exposure Report (2024)

Use this source for the scale of occupational heat exposure globally (2.2 billion workers) and the LMIC-versus-high-income exposure gap. The DALY and injury estimates are modeled, not directly reported by surveillance systems. Do not use the national-level exposure prevalence as a district-level exposure measure.

### Xu et al. 2021 Systematic Review

Use this source for the peer-reviewed evidence that extreme heat is associated with increased occupational injuries. The pooled estimate (OR 1.21, 95 percent CI 1.11-1.32) is robust but dominated by high-income country studies. Do not generalize the effect size to LMIC settings without noting the heterogeneity and transferability limitations.

### WHO/ILO UV Radiation Joint Estimate (2024)

Use this source as methodological precedent for quantifying climate-linked occupational hazards at global scale. It covers UV radiation, not heat stress, but demonstrates the counterfactual attribution approach that could be applied to heat. Do not cite it as evidence about heat stress outcomes.

### ISO 7243:2017 WBGT Standard

Use this source for the internationally recognized WBGT threshold framework. The standard is paywalled beyond the abstract, so specific threshold values should be verified against the purchased document before operational use. Do not assume WBGT thresholds from temperate-climate studies apply unchanged to acclimatized tropical workers.

### Dunne et al. 2013 Labor Capacity Model

Use this source for projected labor capacity loss under climate change scenarios. The 20 percent regional figure is a maximum under RCP8.5, not a likely global average. Do not use it as a current estimate of labor loss, and do not assume the model captures adaptation through scheduling or mechanization.

### ILO Injury and Death Estimates (2024)

Use this source for the estimated annual occupational injuries (26.2 million) and deaths (18,970) attributable to excessive heat. These are modeled estimates with underreporting adjustment, not direct surveillance counts. Do not use them as country-specific injury rates without checking the underlying methodology.

### ERA5 Reanalysis (ECMWF)

Use this source for gridded climate data to derive WBGT exposure estimates at 0.25-degree, hourly resolution from 1940 onward. ERA5 is the preferred reanalysis for sub-national WBGT derivation because it is the highest-resolution global product available. Do not treat ERA5 as a worker exposure dataset without overlaying labor force spatial distributions and work-schedule assumptions. Do not assume WBGT values from ERA5 variables without documenting which empirical formula was used, because different formulas can produce different threshold crossings near the ISO 7243 boundaries.

### MERRA-2 Reanalysis (NASA GMAO)

Use this source as a cross-check reanalysis for WBGT derivation where ERA5 gaps or version differences need verification. MERRA-2 is coarser (0.5 x 0.625 degrees) than ERA5 and should not be the primary reanalysis for sub-national LMIC mapping. Do not assume MERRA-2 radiation and humidity schemes produce identical WBGT to ERA5; cross-referencing with local station data is needed before operational local decisions.

### ILOSTAT Employment-by-Industry

Use this source for national-level worker population denominators by industry (ISIC 4-digit) and status in employment. Sub-national breakdowns exist for only a minority of countries. Informal employment indicators are modeled and incomplete for many LMICs. Do not treat ILOSTAT as a sub-national worker distribution dataset without a spatial overlay with local survey or census data. Do not merge ILOSTAT sector estimates with climate grid cells without documenting the spatial interpolation method and its uncertainty.

### Lancet Countdown 2024 Heat-Labor Report

Use this source for the annual framing metric of global heat-related labor loss (490 billion potential work hours in 2023) and for trend comparison across HDI groups. Do not treat the work-hour figure as a direct measurement of worker downtime or income loss. Do not use HDI-group aggregates as sub-national district-level estimates; the model assumes standard work intensity and does not capture local adaptation through scheduling, rest breaks, or acclimatization protocols.

## Evidence Quality Rule

Evidence is not accepted because it sounds plausible. It is accepted when the source, method, limitations, and confidence are explicit enough for a reviewer to attack. Heat exposure estimates must specify the metric (WBGT, ambient temperature, heat index), the data source (station, reanalysis grid, satellite), and the time period. Health outcome estimates must specify the population, industry, surveillance or study method, and geographic coverage.
