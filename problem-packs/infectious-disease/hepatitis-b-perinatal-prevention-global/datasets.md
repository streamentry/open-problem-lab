# Dataset Inventory

## Candidate Sources

| Source family                                                       | Grain                                            | Status                                              | Permitted use                                                                                        | Blocking limitation                                                                                                            |
| ------------------------------------------------------------------- | ------------------------------------------------ | --------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| WHO global hepatitis reports                                        | Global, regional, and country programme summary  | Usable for burden and service-coverage framing      | Burden context, reported intervention coverage, product-access context, and country selection        | Does not provide a linked maternal-newborn episode denominator or prove timely administration                                  |
| WHO Global Health Observatory and WHO/UNICEF immunization estimates | Country-year indicator                           | Usable with indicator audit                         | Reported HepB birth-dose or HepB3 coverage and trend discovery                                       | Definitions, denominator sources, timing, and reporting completeness may differ; any-dose coverage is not timely-dose coverage |
| Antenatal-care and maternity registers                              | Pregnancy or delivery episode, facility and date | Candidate; requires data and linkage audit          | Maternal HBsAg testing, result, delivery setting, birth time, and prophylaxis event documentation    | May omit private care, home births, migrants, stillbirths, or test results recorded in another system                          |
| Laboratory information systems                                      | Specimen and result event                        | Candidate; requires assay and duplicate audit       | HBsAg, HBV DNA, and infant serology or infection outcome events                                      | A positive test is not a completed referral or treatment event; repeat specimens and unmatched records can bias denominators   |
| EPI and child-immunization registers                                | Infant or dose event                             | Candidate; requires timing audit                    | Vaccine administration, dose date and time where recorded, product, lot, and subsequent series doses | Stock, dispatch, tally, and administration may be conflated; birth time may be missing                                         |
| Birth registration and civil-registration systems                   | Birth or vital-event episode                     | Limited until linkage and completeness are verified | Live-birth denominator, birth setting, birth time, and population completeness checks                | Registration delay, undocumented births, stillbirth classification, and privacy constraints can change the denominator         |
| Facility readiness, stock, and cold-chain assessments               | Facility-period                                  | Limited for bottleneck hypotheses                   | Whether service capacity, vaccine availability, cold chain, or staffing might explain missed doses   | Availability or stock is not administration, timing, protection, or outcome                                                    |
| Household surveys and demographic-health surveys                    | Household, woman, or child recall episode        | Limited for timing and equity context               | Birth setting, caregiver recall, ANC contact, and subgroup discovery                                 | Recall error, survey timing, dose-card availability, and limited linkage prevent a complete cascade estimate                   |
| Representative HBsAg serosurveys                                    | Population or age cohort                         | Usable for impact validation only                   | Prevalence and age-cohort validation of long-run prevention impact                                   | Cannot reconstruct maternal screening, prophylaxis, birth-dose timing, or infant-series completion                             |

## Required Fields For Any Accepted Cascade Dataset

- Country, administrative area, facility type, reporting period, and boundary
  version.
- De-identified pregnancy, delivery, infant, specimen, or dose episode keys,
  with the linkage method and unmatched-record count.
- Maternal HBsAg test type, specimen date, result, repeat-test handling, and
  whether the record is an observation or a policy field.
- Prophylaxis eligibility basis, offer or initiation event, date, and outcome
  status, without inferring adherence from dispensing.
- Birth date and time, birth setting, dose administration date and time,
  timely-versus-late classification, product, and missing timing status.
- Infant-series dose dates, denominator construction, and the distinction
  between scheduled, received, documented, and unknown doses.
- Impact-measure definition, specimen timing, assay, case definition, and
  whether the measure is observed or modeled.
- Private-sector coverage, home births, migration, stillbirth handling,
  reporting lag, missingness mechanism, and data-protection controls.

## Measurement Boundaries

The minimum event graph is:

```text
policy -> procurement -> stock -> administration -> timely administration -> infant outcome
```

Only the observed event needed for a claim may enter its numerator. A policy,
procurement record, stock log, or dose dispensed is not a birth-dose numerator.
A late dose must not be silently combined with a timely dose. A serosurvey may
validate impact at population or cohort grain, but it cannot fill an absent
maternal-newborn linkage.

## Rejection Rule

Reject a dataset for a cascade performance estimate when it cannot state the
event grain, denominator, time window, timing field, and missingness mechanism,
or when it treats policy, procurement, stock, or availability as administration.
It may remain as context if its limitation and non-use are explicit.
