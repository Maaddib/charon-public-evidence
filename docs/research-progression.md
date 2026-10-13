# Research and engineering progression

Charon's development was driven by a research problem rather than a fixed
product specification. The early work explored whether publicly accessible
discourse could be collected and analysed to map functions within digital-fraud
ecosystems without identifying individuals or attributing criminal conduct.

## Research requirements that shaped the engineering

| Research requirement | Engineering response |
|---|---|
| Collect heterogeneous public sources | Collector routing for HTTP, RSS, API, plain text and Tor-oriented sources |
| Preserve material for reproducibility | Raw-content retention and structured persistence |
| Identify functional signals in text | Configurable sieves, entity extraction, TF-IDF and classification experiments |
| Compare multiple research cases | Runtime-selectable case and source configuration |
| Avoid unsupported attribution | Evidence rules, confidence, corroboration and explicit limitations |
| Protect research participants | Hashed or removed usernames, excluded identifiers and aggregate reporting |
| Explain analytical outputs | Provenance-linked observations, entities, relationships and findings |
| Move from research prototype to reusable system | Evidence-first Charon Core domain model and staged orchestration |

## Evidenced research context

The preserved research configuration describes a study titled *Mapping
Cybercrime Infrastructures of Digital Fraud: An OSINT-NLP Approach to
Resilience and Collaborative Security*. It defined six ecosystem functions and
used public Reddit discourse. Its ethics configuration prohibited interaction,
deception, private-message collection, doxxing, attempts to identify offenders,
and direct attribution of criminal conduct. Its privacy controls required
usernames to be hashed or removed and analysis to be reported at aggregate or
functional level.

The public repository records these methodological facts but excludes the
corpus, usernames, quotations, source URLs, subreddit selections and coded
records.

## Progression

```text
Research collection problem
  -> configurable OSINT ingestion
  -> functional text classification experiments
  -> multi-case and profile-driven investigation design
  -> limitations around provenance and entity identity
  -> evidence-first domain model
  -> persistent assessment, analysis and reporting
```

This is a development narrative, not a claim that the December 2025 prototype
already possessed the capabilities of the October 2026 system.
