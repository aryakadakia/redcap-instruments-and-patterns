# REDCap instruments and configuration patterns

Instrument definitions and written documentation from building multi-site
screening and assessment databases in REDCap.

## Instrument definitions

Seven REDCap project XML exports covering screeners, clinical assessment
batteries and waitlist management:

| File | Instruments | Fields |
|---|---|---|
| `U01OptimizationDatab_*.xml` | 37 | 839 |
| `PCORIClientAssessmen_*.xml` | 14 | 283 |
| `GhanaR01Clinical_*.xml` | 17 | 316 |
| `MalingeringTest2_*.xml` | 9 | 159 |
| `U01OptimizationScree_*.xml` | 7 | 117 |
| `PCORIClientScreener_*.xml` | 3 | 76 |
| `WaitlistOnlineScreen_*.xml` | 7 | 62 |

These are project metadata exports in CDISC ODM format. They contain form
definitions, field types, validation rules, branching logic and value labels.
They contain no participant records, and can be imported into REDCap to
recreate the instrument structure.

## Documentation

Two write-ups covering configuration patterns rather than any particular study:

- **REDCap features and functions** covers survey queues, action tags,
  conditional logic, alerts and notifications, scheduling, e-consent
  configuration and duplicate detection.
- **Screening protocol** covers the recruitment and data collection flow, from
  screener through eligibility determination to enrolment.

Both have been generalised. Study identifiers, site names, contact details,
survey URLs and incentive amounts have been removed, along with the
screenshots that contained participant data.

## A note on screener design

One pattern worth calling out, because it is not obvious and is easy to get
wrong. An ineligibility notification should not be sent immediately. An instant
response tells a respondent exactly which answer disqualified them, which makes
it straightforward to re-enter the screener with adjusted answers. Delaying the
alert removes that feedback loop.

## Licence

Copyright (c) 2026 Arya Kadakia, licensed under
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). This repository holds
instrument definitions and documentation rather than code, so a content licence
is more appropriate than a software one. You may share and adapt the material,
including commercially, with attribution.
