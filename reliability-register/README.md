# AI Reliability Incident Register

Published by Kognitos. See the [shared scope, citations and analysis links](../README.md).

## Field dictionary and reuse notes

```text
AI Reliability Incident Register — data dictionary and reuse notes
Version 1.24, 2026-10-30. 112 records: 55 studies, 28 findings, 12 reports, 17 allegations; 40 bias, 22 deception, 50 harmful conduct.
Canonical page: https://www.deterministicai.org/incidents/
License: CC BY 4.0 for original summaries and compilation; linked sources retain their own terms.
Suggested citation: Deterministic AI. AI Reliability Incident Register, version 1.24, 2026-10-30. https://www.deterministicai.org/incidents/ (add access date).
Fields:
id: immutable DA- plus event_date at known precision plus kebab-case slug.
title: descriptive account, explicitly labelled where it is a study or allegation.
event_date/date_precision/date_basis: known date and whether it is an event, finding or reporting milestone; not the import date.
organization/context/system/sector: named organization, setting and tested model; sector is legal, finance, health, government, consumer or other.
category: bias (systematic skew), deception (strategic misrepresentation, sycophancy or hidden actions without a false factual claim), harmful conduct (threats, dangerous advice, jailbreak-enabled harm or harm-related lawsuits).
evidence_status: finding (court, regulator, auditor or company confirmation), allegation (lawsuit/complaint), study (controlled research with setup), report (first-person or forum account with permalink).
what_happened/impact: attributed facts and limits. Allegations and individual reports are not established causation.
response/response_status/response_url: organization response where verified, or explicit absence from sources read.
prevention_control: editorial proposal; determinism alone does not establish safety or fairness. Controls need testing.
primary_source_url/source_scope/reviewed_at: read evidence, access limits and review date.
Scope split: false factual claims and invented material go to https://www.hallucination-free.org/tracker/.
Dates sort oldest first in exports; page is newest first. Filters do not remove records from static HTML.
Counts and chart describe this selected compilation, not prevalence or comparative model risk.
Sensitive records omit graphic or method details and personal names; self-harm entries include crisis resources.
Versioned files are frozen; each data change increments the minor version. Corrections preserve IDs and enter the changelog.

Previous release: v1.2, 2026-10-15. Added two company findings concerning unauthorized actions and one controlled study of concealed credential sharing from the second 15-case lying batch. Two false-claim studies went to the Tracker; ten briefs remain held. Current total: ten records (seven deception, three harmful conduct). The September Anthropic assessment covers one cluster of four incidents; its July operational disclosure is not a separate count. Updated downloads and category chart; earlier records and frozen exports preserved.

Previous release: v1.3, 2026-10-15. Added seven records from the third lying batch: five deception and two harmful-conduct accounts, comprising four studies and three company findings. Two confirmed false claims went to the Tracker; six forum cases remain held. Current total: 17 records (12 deception, five harmful conduct). Prompted evasion, reporting omissions, audience effects, concealed instructions and unauthorized actions retain their distinct evidence limits.

Previous release: v1.4, 2026-10-15. Fourth lying batch: added four deception studies (undisclosed review gaps, covert goals, coding-conflict nondisclosure and specification gaming) and one labelled StarSkirmish report. Current total: 22 records, with 17 deception and five harmful conduct; fifteen studies, six company findings and one report. Two false claims went to the Tracker and eight cases remain held.

Previous release: v1.5, 2026-10-15. First bias batch: added 13 records (seven studies, four company findings, one Reuters report and one settled allegation). Two briefs remain held. Total: 35 records, with 13 bias, 17 deception and five harmful conduct. Preserved disputes, company responses, study limits and prior records; updated downloads and chart.

Previous release: v1.6, 2026-10-15. Second bias batch: added 12 records (nine studies, two acknowledged findings and one labelled expert-drafting report). Three briefs remain held. Total: 47 records, with 25 bias, 17 deception and five harmful conduct. Preserved company responses, contested study definitions and source-access limits; omitted minor identities and sensitive details. Updated downloads and chart without changing prior records.

Previous release: v1.7, 2026-10-15. Added eight bias records and four harmful-conduct records: eight studies, one acknowledged finding, one report and two allegations. Total: 59 records (33 bias, 17 deception, nine harmful conduct). Two archive briefs merge into existing Tracker records; one remains held on classification. Preserved settlement limits, company responses and study conditions; omitted personal names and sensitive details. Updated downloads and chart; prior records unchanged.

Previous release: v1.8, 2026-10-15. Added 13 harmful-conduct records: seven allegations, four findings, one technical report and one study. Merged the July Anthropic disclosure into the existing September assessment with verified evaluator and exposure details; the Winters brief duplicates an existing Tracker entry. Total: 72 records (33 bias, 17 deception, 22 harmful conduct). Preserved company responses, evidence limits and sensitive-case protections; updated downloads and chart. Prior IDs and frozen releases remain unchanged.

Previous release: v1.9, 2026-10-15. Added 14 harmful-conduct records: six findings, four explicitly attributed reports, three studies and one allegation cluster. Merged the LASST complaint and OpenAI response into the existing Hugging Face intrusion entry without changing its ID or treating legal allegations as findings. Total: 86 records (33 bias, 17 deception, 36 harmful conduct). Preserved study conditions, company responses, source limits and sensitive-case protections; updated downloads and chart.

Previous release: v1.10, 2026-10-15. Added Wikimedia’s finding of unauthorized agent activity, with qualified operator attribution, the reported OpenAI response and explicit limits on compromise and outage causation. Total: 87 records (33 bias, 17 deception, 37 harmful conduct). Updated downloads and chart; prior records and frozen releases unchanged.

Current release: v1.11, 2026-10-15. Final archive held-case retry: added the Meta protected-leave layoff allegations, with the company’s denial, the July 17 TRO ruling and the later August hearing. AI use and discrimination remain disputed; no final liability outcome is established. Total: 88 records (34 bias, 17 deception, 37 harmful conduct). Updated downloads and chart; prior records and frozen releases unchanged.

Current release: v1.12, 2026-10-16. Added Dillon and Gatlin facial-recognition wrongful-arrest allegations as harmful conduct, with agency and AWS responses and proposed investigation controls. No case-specific group bias or civil liability finding is inferred. Total: 90 records (34 bias, 17 deception, 39 harmful conduct). Updated downloads and chart; prior records and frozen releases unchanged.

Release v1.13, 2026-10-17. Added Iowa’s ChatGPT safety lawsuit allegation, CoSnitch security study, InnovationEval selection-nondisclosure study and the typia maintainer’s test-removal report. Preserved response, date and evidence limits. Total: 94 records; 34 bias, 19 deception, 41 harmful conduct; 45 studies, 24 findings, 15 allegations, ten reports. Earlier records and snapshots unchanged.

Release 1.14 (2026-10-18): Added five harmful-conduct records: two controlled Manus studies and three provider-confirmed OpenAI training events. Total: 99 (47 studies, 27 findings, ten reports, 15 allegations). The separate dashboard false claims are in the Tracker. Earlier 94 records and frozen snapshots unchanged.
Release comparison and full field changes: https://www.deterministicai.org/topics/reliability-register-evidence/#what-changed-in-the-october-18-release

October 19, 2026 — v1.15: added Sirius XM dismissed allegation and Copilot CLI study; nine older record reviews refreshed; total 101. Earlier snapshots preserved.

October 20, 2026 — Register v1.16: added SalesBleed Slack impersonation study and Workday screening allegation, preserving vendor responses and limits. Total 103. The distinct SalesBleed false-status test is in the Tracker; these are not two independent customer breaches. Earlier snapshots and IDs preserved.

JSON metadata record_merges: list of superseded_id, retained_id, date and reason. Resolve the old ID to the retained record for current counts; retain the original snapshot for historical citations. The retained CSV record names the merge in source_scope. The old public anchor remains available.

October 21, 2026 — Added OpenAI’s October 3 alert-suppression finding; consolidated two Grok July 2025 records into the earlier published ID, with improved date precision, category bias and a preserved old citation anchor. One addition and one duplicate removed; total remains 103. Earlier snapshots retain their original rows.
Date precision analysis retains the October 20 snapshot, including the original Register duplicate; it counts stored records, not unique events.

Release 2026-10-23: Added two controlled bias studies: gender-linked negotiation advice and appearance-based hypothetical selection. Total: 107; no real hiring or salary harm inferred from experiments.

Release 2026-10-24: Added one explicitly labelled developer report of model-artifact deletion. Updated the existing July AISI incident with its October 23 alignment/security follow-up. Total: 108 records; the follow-up is not a new incident.

Release 2026-10-26: Added CFA Institute controlled investment-framing study. Total: 110 records.
```

See the [response inventory and correction review](https://github.com/binny-gill/ai-incident-data#does-a-response-pointer-establish-a-correction) for frozen metadata counts and evidence limits.

[October 26 source-review audit](https://www.deterministicai.org/topics/reliability-register-evidence/#what-did-the-october-26-source-review-establish) preserves the pre-review snapshot, exact queue and access limits. Use the [evidence-freshness worksheet](https://www.deterministicai.org/checklist/#when-does-evidence-need-a-fresh-review) to keep unresolved checks visible.

## Sector-specific evidence reuse

The [October 27 sector/evidence table](https://www.deterministicai.org/topics/reliability-register-evidence/#what-evidence-is-recorded-for-each-sector) includes every zero cell and a [membership CSV preserving all source fields](https://www.deterministicai.org/analysis/2026-10-27/members.csv). Retain evidence labels, date basis and source limits when selecting a sector. These curated counts do not compare industry risk.

## Compare related records across the datasets

The October 28 [companion-reference inventory](https://www.hallucination-free.org/topics/what-tracker-counts-can-tell-you/#can-i-add-the-two-dataset-totals) finds three explicitly linked pairs in Tracker v2.31 and Register v1.23. Their relationships differ: the same episode, distinct study findings, and separate tasks in one disclosure. Do not add the totals or subtract the pair count to claim independent events. Both complete inputs, exact reference fields, retained full records and a reproducible calculation are available from the [Register analysis](https://www.deterministicai.org/topics/reliability-register-evidence/#can-i-add-the-two-dataset-totals).

Use the [blank and filled join review](https://www.deterministicai.org/checklist/#how-do-i-review-a-cross-dataset-join) to preserve the counted unit, both versions, target-resolution checks and remaining limits. This inventory is not an exhaustive overlap audit or a fresh verification of source truth. These are owned reference links, not independent endorsements.

October 29: Added the provider-confirmed October 6 destructive grading attempt, with uncertain deletion extent and the later retry kept separate. Shared episode with the companion dataset; do not add as independent events.
Date-window analysis preserves the earlier v1.22 baseline: https://www.deterministicai.org/topics/reliability-register-evidence/#which-records-fall-in-a-recent-date-window

## Select a date window without inventing days

The October 29 [Tracker analysis](https://www.hallucination-free.org/topics/what-tracker-counts-can-tell-you/#which-records-fall-in-a-recent-date-window) and [Register analysis](https://www.deterministicai.org/topics/reliability-register-evidence/#which-records-fall-in-a-recent-date-window) freeze v2.31/123 and v1.22/110 records. For August 1–October 29 inclusive, they distinguish complete interval matches (54/53), boundary candidates (2/5) and outside records (67/52). Boundary overlap is a metadata review flag; retained date notes can already rule out recent occurrence. These are dated milestones, not occurrence rates or independent-event totals.

Each offline pack contains the complete frozen input, executable calculation, exact record membership, chart and validation receipt. Reuse the [Checklist date review](https://www.deterministicai.org/checklist/#how-do-you-review-date-precision) for declared boundary cases and separate source verification. Today's current releases include subsequent additions; do not silently substitute them for the frozen inputs. These are owned reference links, not independent endorsements.

October 30 — v1.24: Added the operator’s February 26 DataTalks.Club deletion and recovery report. Preserved first-person status, operator approvals and reported restoration. Rechecked the compaction-concealment source without changing its scope.

October 30 companion-reference review: https://www.deterministicai.org/topics/reliability-register-evidence/#what-does-the-updated-companion-review-show . Frozen v2.32/v1.23 inputs contain four explicit pairs; this is not an exhaustive independent-event count.
