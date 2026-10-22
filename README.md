# AI incident reference datasets

[Published by Kognitos](https://www.kognitos.com).

Two vendor-neutral publications maintain these selected, source-linked collections. The original summaries and compilations are licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Credit the named publication, link the dataset and license, identify changes and retain evidence qualifications. Linked third-party documents and artwork keep their own terms.

| Collection | Scope | Version / release | Records | Reference page |
|---|---|---|---:|---|
| Hallucination Tracker | Invented facts, citations and other false factual assertions | 2.27 / 2026-10-21 | 119 | [Search and cite records](https://www.hallucination-free.org/tracker/) |
| AI Reliability Incident Register | Bias, deception without a false factual assertion, and harmful conduct | 1.18 / 2026-10-22 | 105 | [Search and filter evidence](https://www.deterministicai.org/incidents/) |

These are curated collections, not representative samples or a vendor ranking. Studies, allegations and reports are labelled; an allegation is not a finding. The same underlying event must be checked for overlap before combining datasets. Do not interpret release growth as a trend in AI failures.

## Downloads and field definitions

- [Tracker CSV](https://www.hallucination-free.org/data/hallucination-tracker.csv) · [JSON](https://www.hallucination-free.org/data/hallucination-tracker.json) · [Tracker field dictionary](hallucination-tracker/README.md)
- [Register CSV](https://www.deterministicai.org/data/ai-reliability-incidents.csv) · [JSON](https://www.deterministicai.org/data/ai-reliability-incidents.json) · [Register field dictionary](reliability-register/README.md)

CSV has one row per record. JSON has release metadata and a `records` array. Join on stable `id`; do not join by title or row position. `event_date` can have year, month or day precision; read `date_basis` before interpreting it. `reviewed_at` is the source-review date, not the event date. `primary_source_url` is a legacy field name for the principal evidence, which may be reporting; `source_scope` explains the source type and access limits. `response` retains the company or responsible party's position. Proposed control fields are editorial analysis, not measured prevention.

Tracker-specific fields distinguish `failure_type`, `ai_involvement`, `ai_involvement_basis`, `record_type` and old `legacy_id`. Register-specific `category` and `evidence_status` are separate dimensions. The linked folder dictionaries document all remaining fields.

## Reproduce the published analyses

- [Tracker composition](https://www.hallucination-free.org/topics/what-tracker-counts-can-tell-you/): v2.23 counts by AI involvement and failure type, with record-type totals, frozen input, hash, code, chart and aggregate tables.
- [Register evidence](https://www.deterministicai.org/topics/reliability-register-evidence/): v1.12 counts by category and evidence status, with the same reproducibility artifacts.
- [Deterministic AI Checklist](https://www.deterministicai.org/checklist/): a reusable ten-check worksheet, action/approval procedures and a filled review tied to actual toy-run outputs. Tests of a toy function do not certify a deployed AI system.

## How to cite

Hallucination-Free. *The Hallucination Tracker*, version 2.27, October 21, 2026. https://www.hallucination-free.org/tracker/. Include access date and the incident ID when citing a single record.

Deterministic AI. *AI Reliability Incident Register*, version 1.18, October 22, 2026. https://www.deterministicai.org/incidents/. Include access date and incident ID.

For reproducibility, cite a versioned file rather than only the latest download. IDs remain stable after publication; corrections belong in the changelog. See [CITATION.cff](CITATION.cff) and [release history](CHANGELOG.md).

Only published entries belong in this repository. Private source archives, held leads and internal notes are excluded.

## Trace a count to its records

The October 16 analyses include frozen membership CSVs with stable IDs, evidence labels, source limits and suggested citations: [Tracker membership](https://www.hallucination-free.org/analysis/2026-10-16/membership.csv) and [Register membership](https://www.deterministicai.org/analysis/2026-10-16/membership.csv). Their analysis pages supply export code, a verifier and observed results. Preserve the original denominator when quoting a percentage; describe any filtering and identify changes.

## Filtered selection reuse — October 17, 2026

The [Tracker selection](https://www.hallucination-free.org/topics/what-tracker-counts-can-tell-you/#how-do-i-preserve-my-selection-for-citation) and [Register selection](https://www.deterministicai.org/topics/reliability-register-evidence/#how-do-i-preserve-my-selection-for-citation) preserve full records, exact filters and selected IDs against frozen October 16 snapshots. Keep each selection record with its CSV/JSON; add your access date, preserve qualifications and identify changes. These owned references are not independent endorsements.

## Review changes before updating a citation

October 18 releases: Tracker v2.24 (114 records) and Register v1.14 (99). Compare [Tracker changes](https://www.hallucination-free.org/topics/what-tracker-counts-can-tell-you/#what-changed-in-the-october-18-release) or [Register changes](https://www.deterministicai.org/topics/reliability-register-evidence/#what-changed-in-the-october-18-release) using the pinned downloads, full field-level JSON and checksums. Preserve the release originally cited. These counts describe selected records, not population failure rates.

## Review dates and source access

The October 19 [Tracker review-date audit](https://www.hallucination-free.org/topics/what-tracker-counts-can-tell-you/#how-old-are-the-record-reviews) and [Register audit](https://www.deterministicai.org/topics/reliability-register-evidence/#how-old-are-the-record-reviews) preserve the exact ten-record queue from earlier frozen releases, with source-review receipts. A recent editorial review date does not establish source truth or convert an allegation into a finding.

## Choose evidence for reuse

[Tracker analysis index](https://www.hallucination-free.org/topics/what-tracker-counts-can-tell-you/#which-analysis-should-i-use) and [Register analysis index](https://www.deterministicai.org/topics/reliability-register-evidence/#which-analysis-should-i-use) identify overlapping frozen inputs and exact artifacts. Do not sum their denominators. The [Checklist download guide](https://www.deterministicai.org/checklist/#which-download-should-i-use) distinguishes blank tests from executed teaching examples.

The October 20 releases include two distinct SalesBleed findings from one researcher disclosure, with cross-links. Combining both datasets does not produce a count of independent customer breaches.

## Date precision and duplicate corrections

The October 21 [Tracker date audit](https://www.hallucination-free.org/topics/what-tracker-counts-can-tell-you/#can-these-dates-support-an-exact-daily-timeline) and [Register date audit](https://www.deterministicai.org/topics/reliability-register-evidence/#can-these-dates-support-an-exact-daily-timeline) retain the October 20 inputs and every date-basis field. Month/year dates must not be padded into invented event days.

Register v1.17 merges DA-2025-07-08-grok-antisemitic-output into DA-2025-07-grok-antisemitic-posts. The old [citation anchor](https://www.deterministicai.org/incidents/#da-2025-07-08-grok-antisemitic-output) explains the correction. JSON metadata `record_merges` supplies the mapping; the current CSV survivor records it in `source_scope`. Historical releases still contain both rows. For current counts use the corrected release; for historical claims keep the original denominator and disclose the duplicate. A separate Grok false-context claim in the Tracker shares that episode.

The new OpenAI records cover separate October 3 and October 6 internal tasks from one disclosure. Provider findings and remediation statements are attributed, and strategic motivation remains unresolved. Owned repository links are not independent endorsements.

## Reproduce analyses offline

Download a complete [Tracker pack](https://www.hallucination-free.org/topics/what-tracker-counts-can-tell-you/#how-do-i-use-the-offline-analysis-pack) or [Register pack](https://www.deterministicai.org/topics/reliability-register-evidence/#how-do-i-use-the-offline-analysis-pack): frozen inputs, code, 21 results per pack and citation instructions. The [Checklist handoff review](https://www.deterministicai.org/checklist/#how-do-i-review-an-offline-evidence-handoff) records what file checks establish and what still needs source or workflow testing. Historical duplicates remain disclosed; these owned references are not independent endorsements.
