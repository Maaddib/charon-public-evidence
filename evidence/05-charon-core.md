# H05 - Evidence-first Charon Core

**Period:** July-October 2026  
**Bridge commits:** `065e662` in `osint-pipeline`, followed by `d387ca7` in the
standalone `charon-core` repository on 11 July 2026

## Architectural problem

Replace a snippet- and experiment-centred structure with a durable model that
could support traceable investigation, entity resolution, assessment and
reporting across different source types.

## Contemporaneous technical evidence

The July prototype introduced explicit models for:

```text
Source record
  -> Evidence item
  -> Observation
  -> Entity mention
  -> Resolved entity / relationship
  -> Finding
  -> Analysis
  -> Report
```

The prototype was preserved in `osint-pipeline` at 09:17 on 11 July. The
standalone repository was initialised at 10:39 that morning with the commit
message `Initialize Charon Core evidence foundation`. The timing, overlapping
packages and shared domain vocabulary establish the development bridge.

## Subsequent progression

- 11-16 July: evidence ingestion, entity resolution, assessment, reporting and
  corporate collection.
- 19-24 July: CLI, case repository, knowledge graph and persistent analysis.
- 1 August: external discovery, corporate lifecycle and network rules,
  composite findings and persisted analytical reasoning.
- 23-24 August: structured reporting and deterministic financial assessment.
- 13 October: financial extraction, Gazette intelligence and analytical
  validation (`2122caa`, 36 files, 5,400 insertions and 104 deletions).

## Development outcome

The research prototype had become an evidence- and provenance-centred
investigation platform. Current feature screenshots belong to the endpoint
appendix; the dated commits and architectural transition provide the evidence
of development over time.
