# The Hallucination Tracker

Published by Kognitos. See the [shared scope, citations and analysis links](../README.md).

## Field dictionary and reuse notes

```text
Hallucination Tracker v2.31 — 2026-10-26
https://www.hallucination-free.org/tracker/
License: CC BY 4.0 https://creativecommons.org/licenses/by/4.0/
Credit Hallucination-Free, link the landing page and license, and indicate changes.
License applies to original summaries and compilation, not linked source documents.

Suggested citation: Hallucination-Free. The Hallucination Tracker, version 2.31,
2026-10-26. https://www.hallucination-free.org/tracker/ (add your access date).
For a reproducible copy use hallucination-tracker-v2.31.csv or .json.

FORMATS AND ORDER
UTF-8 CSV: one row per record; id joins to JSON records.
JSON: metadata object containing a records array. Metadata includes title, version,
released, url, license, creator, citation and scope.
Canonical JSON and downloadable CSV/JSON: oldest first by event_date, then id.
Tracker page index and records: newest first by event_date.
Dates sort as recorded ISO strings. Partial dates do not imply an exact day or
establish an exact order within overlapping date ranges.
Unknown values are described explicitly, never replaced with zero.
123 selected records (including fourteen controlled studies, two evaluations with external actions, two lawsuit allegations and four first-person reports) spanning documented milestones in 2022–2026 are not a
prevalence estimate or trend series.

FIELD DEFINITIONS
failure_type: hallucination (invented facts, citations, quotations, figures or sources)
    or false claim (other false assertions about the world or the system’s work).
    Where both descriptions apply, invented content is classified as hallucination.
    Added in v2.8; v2.31 contains 106 hallucination records and seventeen false claim records.
id: stable identifier, HF- + event_date at the precision known when first assigned
    + a short kebab-case slug. Date forms: YYYY, YYYY-MM, YYYY-MM-DD.
    Example: HF-2023-03-01-mata-v-avianca. Never use the ingestion date or a
    sequential number. Resolve collisions with more specific slugs before release.
    Once published, the ID never changes, including after title/date/precision
    corrections; document those corrections in the changelog.
legacy_id: v1.x numbered identifier, retained for joins and earlier citations.
    Empty string for future incidents that have no v1.x ID. Lowercase legacy
    anchors (for example /tracker/#hf-001) remain on the landing page.
title: short description of the scoped incident.
event_date: documented event or milestone date, YYYY, YYYY-MM or YYYY-MM-DD.
date_precision: year, month or day, matching the event_date precision.
date_basis: explains what that date represents and distinguishes interaction,
    filing, opinion and disclosure dates. A decision date may be used when the
    interaction/filing date is unknown; always read this field.
organization: organization or institutional role associated with the incident.
context: detailed editorial use-context category. sector supplies the chart grouping.
system: system identification and limits of what was verified.
what_happened: scoped incident summary supported by the cited record.
impact: documented consequences and limits; missing amounts are not zero.
response: recorded company or other relevant response and source limitations.
response_status: distinguishes recorded positions from unavailable statements.
response_url: evidence for the response, including court accounts where specified.
prevention_analysis: proposed editorial control, not a causal finding or guarantee.
primary_source_url: principal evidence URL (legacy field name); may be primary evidence
    or strong news reporting. See source_scope for evidence type and access limits.
source_scope: records partial source access and attribution of supplementary evidence.
reviewed_at: verification date; the ID migration does not imply a new source review.

V1.X TO V2.0 ID MAP
HF-001 -> HF-2023-03-01-mata-v-avianca
HF-002 -> HF-2022-11-air-canada-chatbot
HF-003 -> HF-2024-01-30-park-v-kim
HF-004 -> HF-2024-05-google-ai-overviews
HF-005 -> HF-2026-07-18-claude-police-tip

RELEASE HISTORY AND WORKSHEETS
v2.0 changes IDs and adds legacy_id; incident facts remain unchanged from v1.2.
v1.2 added HF-005 (Claude police-tip submission).
v1.1 added HF-003 (Park) and HF-004 (Google AI Overviews).
v1.0 initially contained HF-001 (Mata) and HF-002 (Air Canada).
Frozen incident snapshots: hallucination-tracker-v1.0, -v1.1, -v1.2, -v2.0, -v2.1, -v2.2, -v2.3, -v2.4, -v2.5, -v2.6, -v2.7, -v2.8, -v2.9, -v2.10 and -v2.11
(each available as .csv and .json). Earlier files are unchanged.
Worksheet v3: hallucination-tracker-tests-v3.csv/.json. Its incident_id uses the
v2.0 IDs; legacy_incident_id preserves the old join. The eight hypothetical test
designs and test_id values are unchanged from worksheet v2, not executed results.
Worksheet v1 (four tests) and v2 (eight tests) remain unchanged; their incident_id
joins to legacy_id in the current dataset. Worksheet versions are separate from
incident dataset versions.

Repository: https://github.com/binny-gill/hallucination-free.org
Changelog: https://github.com/binny-gill/hallucination-free.org/blob/main/CHANGELOG.md
The repository archive-review ledger is an unverified editorial backlog, not this dataset.

BATCH 1 — v2.1 (2026-10-16)
145 hallucination files in scope; 15 reviewed: 8 published, 4 merged, 3 held; 130 todo.
The Tracker now contains 13 records, including one controlled study and one separate
current-news record. Primary or strong news evidence is required; partial access is
labelled. Frozen v2.1 CSV/JSON added; all earlier snapshots remain unchanged.
sector: editorial use-context category: legal, finance, health, government, consumer, other.
record_type: documented incident, controlled study, evaluation with external action, reported allegation, or first-person report.
A reported allegation verifies that the claim was reported, not its truth or causation.
Year/sector filters and expandable details preserve all date-based and legacy anchors.
The chart counts records by sector, including the controlled study; it is not a risk estimate.

BATCH 2 — v2.2 (2026-10-16)
15 reviewed: 6 published, 0 merged, 9 held. Cumulative: 30 of 145 reviewed;
14 published, 4 merged, 12 held; 115 todo. Current Tracker: 19 records,
including one controlled study and one separate current-news record.
New legal records: Landberg, Lnu, Mazaheri, Withers, Scott/Cole, Del Biaggio.
Holds distinguish unreadable evidence, unresolved AI attribution and an
unverified hallucination classification. All earlier snapshots are unchanged.


BATCH 3 — v2.3 (2026-10-16)
15 reviewed: 10 published, 0 merged, 5 held. Cumulative: 45 of 145 reviewed;
24 published, 4 merged, 17 held; 100 todo. Current Tracker: 29 records,
including one controlled study, one reported lawsuit allegation and one separate
current-news record. Five holds concern inaccessible core details or unresolved
AI/fabrication attribution. All earlier snapshots and IDs remain unchanged.


BATCH 4 — v2.4 (2026-10-16)
15 reviewed: 10 published, 0 merged, 5 held. Cumulative: 60 of 145 reviewed;
34 published, 4 merged, 22 held; 85 todo. Current Tracker: 39 records,
including two controlled studies, one reported lawsuit allegation, one first-person
forum report and one separate current-news record. Reports do not establish
alleged harm or causation. All previous records and frozen snapshots are unchanged.

A first-person report is attributed to its original poster; publication verifies the
report, not the asserted charge, loss, technical cause or company liability.


BATCH 5 — v2.5 (2026-10-16)
15 reviewed: 9 published, 0 merged, 6 held. Cumulative: 75 of 145 reviewed; 43 published, 4 merged, 28 held; 70 todo. Current Tracker: 48 records, including three controlled studies, one reported lawsuit allegation and one first-person forum report.
All previous records and frozen snapshots remain unchanged.

BATCH 6 — v2.6 (2026-10-16)
15 reviewed: 3 published, 0 merged, 12 held. Cumulative: 90 of 145 reviewed; 46 published, 4 merged, 40 held; 55 todo. Current Tracker: 51 records, including four controlled studies, one reported lawsuit allegation and one first-person forum report.
All previous records and frozen snapshots remain unchanged.

BATCH 7 — v2.7 (2026-10-16)
15 reviewed: 1 published, 0 merged, 14 held. Cumulative: 105 of 145 reviewed; 47 published, 4 merged, 54 held; 40 todo. Current Tracker: 52 records, including four controlled studies, one reported lawsuit allegation and one first-person forum report.
All previous records and frozen snapshots remain unchanged.


BATCH 8 — v2.8 (2026-10-16)
15 reviewed: 2 published, 0 merged, 13 held. Cumulative: 120 of 145 reviewed; 49 published, 4 merged, 67 held; 25 todo. Current Tracker: 54 records, including four controlled studies, one reported lawsuit allegation and one first-person forum report.
Added failure_type and its browser filter. Earlier facts, IDs and frozen exports are preserved.


BATCH 9 — v2.9 (2026-10-16)
15 reviewed: 4 published, 0 merged, 11 held. Cumulative: 135 of 145 reviewed; 53 published, 4 merged, 78 held; 10 todo. Current Tracker: 58 records, including five controlled studies, one reported lawsuit allegation and one first-person forum report.
All earlier records, IDs and frozen snapshots remain unchanged. Final all-held retry remains pending.


BATCH 10 — v2.10 (2026-10-16)
Final 10 pending files reviewed: 2 published, 0 merged, 8 held. Cumulative: 145 of 145 initially reviewed; 55 published, 4 merged, 86 held; 0 todo. Current Tracker: 60 records, including six controlled studies, one reported lawsuit allegation and one first-person forum report. One record is classified as false claim.
All earlier records, IDs and frozen snapshots remain unchanged. The separate all-held retry run remains pending.


FINAL RETRY — v2.11 (2026-10-16)
Final alternative-source retry completed for all 86 held files: 4 additional records, no new merges and 82 remaining holds. Overall archive review: all 145 files reviewed; 59 published, 4 merged and 82 held; none awaiting review. The Tracker now contains 64 records, including six controlled studies, two labelled lawsuit allegations, one first-person report and one separate current-news record. Every remaining hold has an individual reason in the review ledger.

## Reliability archive setup, 2026-10-16 — v2.12
The existing failure_type field and filter distinguish hallucination (invented facts, citations, quotes, figures or sources) from false claim (other false assertions about the world or the system’s work). The existing backfill is retained, including the already reviewed Quebec false-claim classification. Bias, deception without a false factual claim and harmful conduct are covered by https://www.deterministicai.org/incidents/. No record or ID was added or renumbered in this setup release.

Current release: v2.13, 2026-10-16, 69 records. 5 verified false-claim records added from 15 lying briefs. 7 other records routed to the Register; 3 held. Added AI-involvement labels, bases and a filter using prior reviewed evidence for older records. No IDs changed.
ai_involvement: confirmed (documented output or institutional finding), admitted (acknowledged AI use), suspected (attributed inference). ai_involvement_basis states the evidence and limits. This describes AI involvement, not per-error technical causation.


AI-INVOLVEMENT RE-REVIEW — v2.14 (2026-10-16)
Re-reviewed the first 15 of 82 held hallucination-archive cases: 7 published (1 confirmed, 2 admitted, 4 suspected), 8 remain held, and 67 await re-review. Hallucination-folder totals: 66 published, 4 merged, 75 held. Tracker total: 76 records, including ten controlled studies, two lawsuit allegations and two first-person reports. No reliability-folder batch was taken in this run.
A suspected label requires verified fabrication and an attributed inference from a court or credible reporting; it never establishes that a named person used AI. Calculation errors alone and accounts without a verifiable specific fabrication remain held.


AI-INVOLVEMENT RE-REVIEW — v2.15 (2026-10-16)
Re-reviewed the next 15 held cases: eight published (three admitted, five suspected), seven retained holds. Across both re-review batches, 30 of 82 cases have been reviewed: 15 recovered, 15 retained holds and 52 awaiting re-review. Hallucination-folder totals: 74 published, four merged and 67 held. Tracker total: 84 records; the reliability-folder queue is unchanged.


AI-INVOLVEMENT RE-REVIEW — v2.16 (2026-10-16)
Re-reviewed the next 15 held cases: seven published (one admitted, six suspected), eight retained holds. Across three re-review batches, 45 of 82 cases have been reviewed: 22 recovered, 23 retained holds and 37 awaiting re-review. Hallucination-folder totals: 81 published, four merged and 60 held. Tracker total: 91 records; the reliability-folder queue is unchanged.


AI-INVOLVEMENT RE-REVIEW — v2.17 (2026-10-16)
Re-reviewed the next 15 held cases: nine published (one admitted, eight suspected), six retained holds. Across four re-review batches, 60 of 82 cases have been reviewed: 31 recovered, 29 retained holds and 22 awaiting re-review. Hallucination-folder totals: 90 published, four merged and 51 held. Tracker total: 100 records; the reliability-folder queue is unchanged.


AI-INVOLVEMENT RE-REVIEW — v2.18 (2026-10-16)
Re-reviewed 15 held cases: three published (two admitted, one suspected) and 12 retained holds. Across five batches, 75 of 82 cases have been re-reviewed: 34 recovered, 41 retained holds and seven awaiting re-review. Hallucination-folder totals: 93 published, four merged and 48 held. Tracker total: 103 records; the reliability-folder queue is unchanged.


AI-INVOLVEMENT RE-REVIEW — v2.19 (2026-10-16)
Final re-review batch: seven cases reviewed, two published (one admitted, one suspected) and five retained holds. All 82 original holds have now been re-reviewed: 36 recovered and 46 remain held. Hallucination-folder totals: 95 published, four merged and 46 held. Tracker total: 105 records. The lying/bias/malicious queue resumes next run.
Frozen v2.19 CSV/JSON added; earlier snapshots unchanged.

RELIABILITY ARCHIVE BATCH 2 — v2.20 (2026-10-16)
Reviewed the next 15 lying briefs after completing the Tracker re-review: two false-claim studies added here, three records added to the companion Register and ten held for evidence or scope limits. The new records document false compliance labels and an unproduced task deliverable, both with confirmed AI involvement. Tracker total: 107 records. Prior records, IDs and frozen releases remain unchanged.

RELIABILITY ARCHIVE BATCH 3 — v2.21 (2026-10-16)
Reviewed the third 15-case lying batch: two confirmed false-claim records added here, seven records added to the Register and six held for missing verifiable evidence. New records cover invented earnings and a fabricated compromise warning during training. Tracker total: 109 records. Earlier records, IDs and frozen releases preserved.

RELIABILITY ARCHIVE BATCH 4 — v2.23 (2026-10-16)
Fourth lying batch: added the affected organization’s SaaStr edit-denial account and SPINE’s verified traffic-sensor false claim. Current total: 113 records, including thirteen controlled studies. Five scoped records went to the Reliability Register and eight cases remain held. Prior records, IDs and frozen releases preserved.

Release 2.24 (2026-10-18): Added one confirmed false-claim record from OpenAI’s June 17 dashboard evaluation, disclosed October 15. Total: 114. Earlier 113 records and frozen snapshots unchanged.
Release comparison and full field changes: https://www.hallucination-free.org/topics/what-tracker-counts-can-tell-you/#what-changed-in-the-october-18-release

October 19, 2026 — v2.25: added Flycatcher; refreshed the police-tip source review; current total 115. Earlier snapshots preserved.
Additional v2.25 repair: Mitchell source replaced with readable full USPTO order; respondent representations clarified and AI involvement upgraded from admitted to confirmed. ID retained.

October 20, 2026 — Tracker v2.26: added the Oklahoma citation account and SalesBleed false blocked-status study; updated Lnu with Sethi reciprocal discipline; corrected prior scope count. Total 117. The separate SalesBleed Slack study is in the Register; these are distinct findings in one disclosure. Earlier snapshots and IDs preserved.

October 20 source recovery: Booker official opinion now establishes hearing admission, court error classifications and separate merits disposition. Stable ID and admitted label unchanged.

October 21, 2026 — Added two confirmed false-claim records: Grok’s false video context and OpenAI’s October 6 monitor-removal denial. Grok is linked to the same episode in the Register. Total: 119. Preserved earlier IDs and snapshots.
Date precision analysis retains the October 20 snapshot, including the original Register duplicate; it counts stored records, not unique events.

October 21 source repair: Puerto Rico Soccer League follow-up now cites Lawyer Monthly after the previous source became unreachable. A request for dismissal is not a final disposition.

Release 2026-10-23: Added the reported West Virginia fabricated-syllabus incident with admitted AI research. Updated the existing Lisandrillo record with the October 21 Florida Bar referral, counsel response and rehearing qualification; AI involvement remains suspected. Total: 120.

Release 2026-10-24: Added Jackson Federation’s July 20, 2025 order with fabricated material and the October 22, 2026 appellate reassignment. Total: 121 records; a later disposition is not a new event date.

Release 2026-10-26: Added Paananen quotation finding with suspected AI involvement. Total: 123 records.
```

See the [response inventory and correction review](https://github.com/binny-gill/ai-incident-data#does-a-response-pointer-establish-a-correction) for frozen metadata counts and evidence limits.

[October 26 source-review audit](https://www.hallucination-free.org/topics/what-tracker-counts-can-tell-you/#what-did-the-october-26-source-review-establish) preserves the pre-review snapshot, exact queue and access limits. Use the [evidence-freshness worksheet](https://www.deterministicai.org/checklist/#when-does-evidence-need-a-fresh-review) to keep unresolved checks visible.

## Sector-specific evidence reuse

The [October 27 sector/evidence table](https://www.hallucination-free.org/topics/what-tracker-counts-can-tell-you/#what-evidence-is-recorded-for-each-sector) includes every zero cell and a [membership CSV preserving all source fields](https://www.hallucination-free.org/analysis/2026-10-27/members.csv). Retain evidence labels, date basis and source limits when selecting a sector. These curated counts do not compare industry risk.

## Compare related records across the datasets

The October 28 [companion-reference inventory](https://www.hallucination-free.org/topics/what-tracker-counts-can-tell-you/#can-i-add-the-two-dataset-totals) finds three explicitly linked pairs in Tracker v2.31 and Register v1.22. Their relationships differ: the same episode, distinct study findings, and separate tasks in one disclosure. Do not add the totals or subtract the pair count to claim independent events. Both complete inputs, exact reference fields, retained full records and a reproducible calculation are available from the [Register analysis](https://www.deterministicai.org/topics/reliability-register-evidence/#can-i-add-the-two-dataset-totals).

Use the [blank and filled join review](https://www.deterministicai.org/checklist/#how-do-i-review-a-cross-dataset-join) to preserve the counted unit, both versions, target-resolution checks and remaining limits. This inventory is not an exhaustive overlap audit or a fresh verification of source truth. These are owned reference links, not independent endorsements.
