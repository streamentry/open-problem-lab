# Dataset Inventory

## Candidate Sources

| Source family                           | Grain                                  | Status                             | Permitted use                                                    | Blocking limitation                                                    |
| --------------------------------------- | -------------------------------------- | ---------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------------- |
| WHO Chagas fact sheet and NTD report    | Global/country program summary         | Usable for framing                 | Burden estimates, roadmap targets, and reported program presence | Not an end-to-end cascade denominator                                  |
| National antenatal-care registers       | Facility, pregnancy, or person episode | Candidate, requires audit          | Maternal screening and referral denominators                     | May omit private care, migrants, or undocumented follow-up             |
| Laboratory information systems          | Test/specimen/result event             | Candidate, requires linkage review | Confirmation and test-timing analysis                            | Duplicate specimens and non-standard assays can distort counts         |
| Birth and newborn registers             | Birth or infant episode                | Candidate, requires audit          | Exposed-newborn identification and testing windows               | Linkage may be unavailable or unsafe without de-identification         |
| NTD medicine and treatment registers    | Patient or facility episode            | Candidate, requires audit          | Treatment initiation and completion proxy                        | Dispensing is not ingestion, cure, or retained follow-up               |
| WHO Chagas database and country reports | Country/program                        | Limited until metadata is verified | Discovery of candidate countries and reporting systems           | Coverage definitions and reporting completeness may differ             |
| Unlinked prevalence surveys             | Household or selected population       | Limited for cascade work           | Context and sampling-frame review                                | Cannot establish the number of infected pregnancies or treated infants |

## Required Fields For Any Accepted Cascade Dataset

- Country, facility, and service setting, with administrative-boundary version.
- Pregnancy or infant episode identifier that is de-identified before analysis.
- Test type, specimen date, result, and repeat-test status.
- Maternal infection status and whether the newborn was exposed.
- Infant test timing, treatment start, treatment completion, and follow-up outcome.
- Denominator definition, missingness, private-sector coverage, migration handling, and linkage error audit.

## Rejection Rule

Reject a source for cascade performance estimates when it cannot distinguish a policy, procurement event, test event, treatment dispensing event, and completed follow-up outcome. It may remain as contextual evidence if its limitation is explicit.
