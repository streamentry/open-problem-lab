# Evidence Ledger

## Current Evidence Records

The machine-readable ledger is `evidence.json`.

## Evidence Notes

### modis-viirs-fire-detection

Use MODIS and VIIRS fire-count data as the primary spatial indicator of burning activity. MODIS at 1km resolution systematically misses small fires common in fragmented agricultural landscapes. VIIRS at 375m improves detection but still misses smoldering burns. Cloud cover during October-November monsoon withdrawal blocks detection for days. Do not use fire counts as a direct proxy for PM2.5 emissions — fire count and emission magnitude are different things. GFED emissions estimates layer additional modeling assumptions on top of burned-area algorithms with known error rates.

### cpcb-monitoring-network-south-asia

CPCB's approximately 300 stations provide the only official ground-truth for PM2.5 in India, but roughly one station per 4.7 million people is grossly inadequate for rural agricultural belt monitoring. Most Punjab-Haryana burning districts have zero monitors. Any satellite-to-PM2.5 validation using CPCB data will be biased toward urban sites. Document this sparsity explicitly in every analysis that uses CPCB data for validation. Do not extrapolate urban monitor readings to rural burning areas without acknowledging the data gap.

### crop-residue-management-program-india

Use this source for context on intervention effectiveness, not for causal claims about burning reduction. Machine distribution numbers do not equal adoption. VIIRS fire counts show burning continues at scale despite eight years of subsidies. The 50-70 percent residual burning estimate is contested — different measurement approaches give different numbers. Do not cite program statistics as evidence of declining burning without independent satellite verification.

## Evidence Quality Rule

Evidence is not accepted because it sounds plausible. It is accepted when the source, method, limitations, and confidence are explicit enough for a reviewer to attack.
