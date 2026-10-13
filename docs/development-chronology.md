# Development chronology

## November-December 2025: exploratory OSINT pipeline

The earliest local file dates begin on 22 November 2025. The first Git
snapshot, commit `9f4fb19` on 5 December, recorded a working exploratory
pipeline with 40 files and 2,345 inserted lines.

The system selected an appropriate collector for HTTP, Tor, RSS, API, or plain
text sources; retained raw content in object storage; applied configurable
text sieves; extracted patterns and entities; and stored selected snippets in
PostgreSQL for later analysis. Its initial use was exploratory infrastructure
mapping rather than a complete case-to-report investigation system.

On 7 December, `c6451d8` reorganised the initial `CharonProject` layout into a
standard `src/charon` Python package. On 13 December, `7dbc491` cleaned and
Dockerised the project, while `5e46347` introduced environment-selectable
source and sieve configurations for multiple cases.

## December 2025: profile-driven enhanced due diligence

Commit `05a3561` on 15 December added a reusable individual EDD architecture:
nine staged investigation dimensions, shared collection-source packs, a case
template, dry-run validation, and a structured report template. Evidence rules
separated reusable analytical logic from case-specific subject data and
required observable, attributable evidence rather than unsupported inference.

## March 2026: collection and crawler expansion

Commit `acfde20` on 4 March added Companies House query collection and CSV
extraction. Commit `4fb6caf` on 19 March added targeted crawling, search
components, tagging, additional profiles and cases, and main-dispatcher
integration. The repository then contained both the original case-driven
ingestion route and a newer crawler route.

## April-June 2026: research experiments

Standalone research scripts explored Reddit signal analysis, adaptive term
discovery, TF-IDF, classification, entity extraction, and coded-dataset repair.
These files demonstrate experimentation feeding later design decisions; they
should not be represented as a single integrated production pipeline.

## July 2026: evidence-first Charon prototype

Commit `065e662` on 11 July preserved the existing research repository and
introduced a second, evidence-first Charon package. Its domain vocabulary
covered sources, evidence, observations, entity mentions, resolved entities,
relationships, findings, analysis, orchestration, and reporting.

At 10:39 that morning, the separate `charon-core` repository began with commit
`d387ca7`, `Initialize Charon Core evidence foundation`. The close timing,
overlapping package structure, and shared domain concepts establish that the
new repository evolved from the prototype preserved in `osint-pipeline`.

## July-October 2026: standalone Charon Core

The standalone project subsequently added persistent evidence ingestion,
entity resolution, knowledge graphs, assessment, reporting, corporate
collection, CLI case management, external discovery, corporate lifecycle and
network findings, persisted analytical reasoning, structured reports,
financial assessment, and Gazette intelligence. The latest inspected commit
was `2122caa` on 13 October 2026.

## Development interpretation

The defensible portfolio narrative is:

1. collector and snippet pipeline;
2. configurable multi-case OSINT system;
3. profile-driven EDD and crawler research platform;
4. evidence- and provenance-centred Charon prototype;
5. independently developed standalone Charon Core.

This chronology describes evidenced development milestones. It does not claim
that every experimental component was production-ready or end-to-end complete.
