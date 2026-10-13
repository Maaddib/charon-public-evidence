# Charon - Technical Development Evidence

This repository presents a public, record of the development
of Charon, an independently developed investigative-intelligence platform.

It traces the work from the original OSINT Pipeline experiments in late 2025
through the evidence-centred Charon Core architecture developed during 2026.
The emphasis is on technical progression, engineering decisions, provenance,
and reproducible evidence rather than operational investigation content.

## Development overview

```text
2025: OSINT collection and snippet processing
  -> configurable multi-case pipeline
  -> profile-driven enhanced due diligence
2026: targeted crawling and structured-source collection
  -> analytical research experiments
  -> evidence-first Charon prototype
  -> standalone Charon Core
  -> structured financial, graph, assessment and reporting workflows
```

See [Development chronology](docs/development-chronology.md) for the dated
evidence behind this sequence.

## Evidence of progression

The principal evidence is chronological rather than feature-led:

1. [Exploratory OSINT pipeline, November-December 2025](evidence/01-original-osint-pipeline.md)
2. [Research-led EDD architecture, December 2025](evidence/02-research-led-edd.md)
3. [Collection and crawler expansion, March 2026](evidence/03-collection-expansion.md)
4. [Research experimentation, April-June 2026](evidence/04-research-experiments.md)
5. [Evidence-first Charon Core, July-October 2026](evidence/05-charon-core.md)

Each exhibit identifies the research problem, contemporaneous technical
evidence, limitations discovered, and the architectural response. The current
CLI, extraction, graph, assessment and reporting views belong in a separate
[current-system appendix](docs/current-system-appendix.md); they are not used
to imply that those capabilities existed at the beginning of the project.

The [provenance manifest](docs/provenance-manifest.md) records the private Git
objects or content hashes used to verify each exhibit while keeping the
underlying repositories and research data confidential.

Assessors can browse the [inspectable evidence index](evidence/README.md) to
review the compact commit records, historical excerpts, research controls and
repository-transition evidence supporting the narrative.

## Architecture

The original OSINT Pipeline was organised primarily around collectors,
configurable text sieves, snippets, and supporting storage services. Charon
Core changed the central model to a traceable investigation chain:

```text
Source
  -> Evidence
  -> Observation
  -> Entity mention
  -> Resolved entity and relationship
  -> Assessment
  -> Structured analysis
  -> Report
```

See [Architecture and capabilities](docs/architecture-and-capabilities.md) for
the documented comparison.

## Disclosure boundary

This repository intentionally does not contain:

- Charon's complete private source code;
- credentials, infrastructure secrets, or environment files;
- client, subject, or investigation data;
- collected documents or proprietary datasets;
- detailed assessment thresholds, prompts, or commercial methodology; or
- production database exports and operational logs.

The public material demonstrates engineering capability without making the
underlying investigative system or sensitive evidence public. See the full
[disclosure statement](docs/disclosure-boundary.md).

## Research relationship

The early system supported research into mapping digital-fraud infrastructure
through public-source discourse and NLP. Research requirements around privacy,
sampling, non-attribution, traceability and reproducibility progressively
shaped Charon's architecture. See [Research and engineering progression](docs/research-progression.md).

## Status

This is a local preparation copy. It has not yet been published and no GitHub
visibility setting has been changed.
