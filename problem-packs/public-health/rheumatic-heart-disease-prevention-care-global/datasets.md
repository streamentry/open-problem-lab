# Dataset Inventory

## Candidate Sources

| Source family                                                     | Likely grain                                              | Status                                                 | Permitted use                                                                                                  | Blocking limitation                                                                                                      |
| ----------------------------------------------------------------- | --------------------------------------------------------- | ------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| WHO burden estimates and mortality products                       | Global, regional, or country model/output                 | Usable for framing; limited for cascade measurement    | Burden context and uncertainty review                                                                          | Does not observe prevention, prophylaxis, diagnosis, referral, surgery, or follow-up events in one denominator           |
| National or regional RF/RHD registries                            | Person or clinical episode; facility and referral network | Candidate, requires audit                              | Case registration, clinical severity, prophylaxis and follow-up events where fields exist                      | Hospital-based registries may overrepresent severe disease and omit people who never reach specialist care               |
| Primary-health-care and school-screening records                  | Encounter, screened person, or facility                   | Candidate, requires case-definition audit              | Screening reach, suspected disease, referral initiation, and population-platform coverage                      | Screening-positive, latent, confirmed, and clinical RHD definitions may be mixed; device and reader variation can matter |
| Pharmacy, procurement, stock, and medicine-administration records | Product, facility, batch, dose, or patient episode        | Limited until event type is separated                  | Supply continuity and possible administered-dose reconciliation                                                | Procurement or stock-on-hand is not a received injection, adherence, or clinical outcome                                 |
| Primary-care, ANC, and hospital encounter records                 | Encounter or episode                                      | Candidate, requires linkage review                     | Suspected streptococcal infection, rheumatic fever, diagnosis, referral, and coexisting pregnancy-related care | Private-sector care, migration, repeated encounters, and missing outcomes can distort denominators                       |
| Echocardiographic screening studies                               | Selected schools, communities, or facilities              | Limited for national ranking; usable for method review | Case-definition and reader-agreement review; hypothesis generation                                             | Convenience samples and changing diagnostic criteria cannot establish national prevalence or programme coverage          |
| Cardiac surgery and valve-care records                            | Procedure, admission, or referral episode                 | Limited for care-capacity and severe-outcome framing   | Definitive-care access, waiting-list, referral, and outcome definitions                                        | People unable to reach surgery are invisible; procedure counts do not measure unmet need or prevention failure           |
| WHO and national essential-medicine availability audits           | Facility, product, and survey round                       | Limited for service delivery                           | Stock and availability context                                                                                 | Availability on survey day cannot prove continuity, administration, adherence, or appropriateness                        |

## Required Dataset Properties

Any accepted cascade dataset must document:

- Person or episode grain after de-identification, with no direct identifiers.
- Facility, district, referral level, and administrative-boundary version.
- Event date and stage definition for prevention, prophylaxis, diagnosis, referral, valve care, and follow-up.
- Case definition, screening device or test method, reader or assessor method where relevant, and confirmation status.
- Denominator construction, repeated encounters, transfer rules, private-sector coverage, migration, and loss-to-follow-up handling.
- Medicine event type: procurement, stock, dispensing, administration, attendance, or adherence.
- Data access permission, license, missingness, linkage error, and validation checks.
- Clinical outcome definitions that are not inferred from a proxy such as dose availability or registry enrollment.

## Rejection Rule

Reject a source for a cascade performance estimate when it cannot distinguish at least one observed event from its upstream capacity proxy and cannot state the denominator, time window, or missingness boundary. It may remain as context if the limitation is explicit.
