# Evidence Ledger

## Current Evidence Records

The machine-readable ledger is `evidence.json`.

## Evidence Notes

### INPE PRODES

Use this source as the gold-standard reference dataset for Amazon deforestation. PRODES is the official Brazilian monitoring system and the most authoritative long-term deforestation record. Its 6.25 ha minimum mapping unit means small clearings are missed. Brazilian Amazon only — other Amazon countries lack an equivalent system.

### Barlow et al. 2016 Nature

Use this source for the combined effect of deforestation and disturbance on Amazon biodiversity across multiple taxonomic groups. The record now uses the primary DOI `10.1038/nature18326`; the previously stored `nature19305` URL was the wrong article identifier and returned 404 during source verification. This is the verify:sources protocol working correctly — broken source identity was corrected rather than silently retained.

### Hansen/GLAD Alerts

Use this source for near-real-time deforestation detection. GLAD enables weekly monitoring but detects tree cover loss generically — it does not distinguish between deforestation, fire, and selective logging.

### GBIF Occurrence Data

Use this source for species occurrence records to estimate ranges and intersect with deforestation. Occurrence density is severely biased toward accessible areas near research stations and rivers. Vast Amazon interior is under-sampled. Records reflect sampling effort, not species distribution. Cannot establish population decline without repeated survey data.

### IUCN Red List Range Maps

Use this source for expert-drawn species range polygons to intersect with deforestation data. Range maps are extent-of-occurrence polygons that overestimate actual occupancy. Static snapshots may not reflect recent range contractions. Intersection with 30 m deforestation data implies false precision at range edges. Biased toward vertebrates; many Amazon species are not assessed.

### MapBiomas Land Cover

Use this source for land cover classification and deforestation-to-land-use transition analysis. Brazil-only coverage. 30 m resolution with 25+ classes and a transition matrix. ML classification can produce temporal inconsistencies. Accuracy varies by biome and year. Does not attribute causal drivers.

### Hansen et al. 2013 Global Forest Change

Use this source as the global 30 m forest change baseline. Measures tree cover loss, not deforestation. Plantation harvest, fire, and natural dieback all counted as loss. Forest definition threshold (canopy cover percentage) affects results. Annual updates available via Global Forest Watch.

### Global Forest Watch Platform

Use this source for integrated access to multiple forest monitoring datasets. Aggregates Hansen loss maps, GLAD alerts, GLAD-S2 alerts, and fire alerts with different definitions, resolutions, and update frequencies. These products must not be conflated in analysis. Does not provide land cover classification.

### Global Forest Watch Driver-Aware Alerts

Use this source for the current driver-aware alert layer as a model-assisted candidate for separating natural and human-caused disturbance. The source reports 11 driver classes at 10 m across the Amazon, Congo, and Indonesia basins. Driver labels are not legal attribution, confirmed land-use change, or biodiversity impact; the production URL currently redirects to the Global Nature Watch surface and should be rechecked before long-term citation.

### MapBiomas Amazon Collection 10

Use this source for annual Amazon biome land-use and land-cover classification from 1985–2024 and for its documented class, sample, and accuracy fields. Collection 10 reports aggregate Level 1 and Level 2 accuracy, but those values are not deforestation-specific precision and do not make the product comparable to PRODES, Hansen, GLAD, or species-range data without a temporal and definition crosswalk.

## Source-Inventory Handoff

The source-inventory task now includes the corrected Barlow primary DOI and two current method/data records. `datasets.md` classifies annual reference maps, near-real-time alerts, driver models, occurrence points, range polygons, and land-cover classes as separate measurement families. The task is ready for domain review; no species-range ranking or extinction-risk claim is being advanced by this inventory.

## Evidence Quality Rule

Evidence is not accepted because it sounds plausible. It is accepted when the source, method, limitations, and confidence are explicit enough for a reviewer to attack.
