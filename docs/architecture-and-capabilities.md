# Original architecture and capabilities

## Initial processing path

```text
Case and source configuration
    -> collector routing
       (HTTP / Tor / RSS / API / plain text)
    -> raw-content retention in object storage
    -> configurable sieve and NLP processing
    -> pattern and entity extraction
    -> selected snippet persistence in PostgreSQL
    -> analyst export and review
```

The local Docker configuration also evidenced OpenSearch and dashboards,
PostgreSQL, Redis, and MinIO development services. The services were bound to
localhost and configured through environment variables. No environment values
are reproduced in this bundle.

## Capability groups evidenced in the repository

### Collection

- Collector routing by source type.
- HTTP, RSS, API, plain-text, and Tor-oriented collection modules.
- Targeted crawling with storage-layout and crawl-state support.
- Companies House search and structured extraction.
- Reddit-oriented API collection experiments.

### Processing

- Configurable text sieves.
- Lightweight pattern and entity extraction.
- URL extraction and rule-based tagging.
- Experimental TF-IDF, classification, and adaptive term discovery.

### Case and profile management

- Multiple case configurations selected at runtime.
- Reusable profiles and shared source packs.
- Nine-stage individual EDD workflow.
- Validation and dry-run tooling.
- Separation between case inputs and reusable analytical logic.

### Storage and traceability

- Raw-content storage using an S3-compatible object service.
- Structured records in PostgreSQL.
- Search services using OpenSearch.
- Crawl/audit logs and case-scoped output layouts.

### Reporting and controls

- Structured EDD report template and evidence-register concept.
- Evidence and corroboration rules.
- Restrictions against unsupported intent, diagnosis, attribution, or paid
  checks without documented authorisation.

## Evolution into Charon Core

The original system was predominantly organised around collection,
configuration, snippets, and experimental analysis. The July prototype changed
the organising principle to a durable evidence chain:

```text
Source
    -> Evidence
    -> Observation
    -> Entity mention
    -> Resolved entity / relationship
    -> Assessment finding
    -> Analysis
    -> Report
```

That change is the principal architectural bridge between the original OSINT
Pipeline and standalone Charon Core.
