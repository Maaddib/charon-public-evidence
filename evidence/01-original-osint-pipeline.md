# H01 - Original OSINT Pipeline

**Period:** November-December 2025  
**Primary commit:** `9f4fb19`, 5 December 2025  
**Recorded change:** 40 files and 2,345 inserted lines

## Research problem

Collect heterogeneous public-source material and identify fraud-infrastructure
signals for exploratory research without relying on a single platform or
source format.

## Contemporaneous technical evidence

The first committed entry point described this processing sequence:

```text
case and source configuration
  -> HTTP / Tor / RSS / API / plain-text collector routing
  -> raw content retained in MinIO
  -> configurable text sieves
  -> lightweight pattern and entity analysis
  -> selected snippets persisted in PostgreSQL
```

The historical module explicitly described itself as a one-snippet-per-URL
orchestrator for exploratory digital-fraud infrastructure mapping.

## What this established

- A working collection and processing spine.
- Separation between collection method and downstream analysis.
- Early preservation of raw source material alongside structured snippets.
- A direct link between the software and the research mapping problem.

## Limitation and next step

The prototype centred on selected snippets and lightweight extraction. It did
not yet provide the durable evidence, provenance, entity-resolution and
assessment boundaries later introduced by Charon Core.

## Public-disclosure note

This exhibit paraphrases the historical source and identifies the commit. It
does not publish collector implementations, source URLs, research data or
environment configuration.
