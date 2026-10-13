# H03 - Structured-source and crawler expansion

**Period:** 4-19 March 2026  
**Primary commits:** `acfde20`, `4fb6caf`

## Engineering problem

Extend the research platform beyond configured URL ingestion into structured
corporate sources and repeatable targeted crawling.

## Contemporaneous technical evidence

- `acfde20` added Companies House query collection and structured CSV
  extraction across five files and 562 inserted lines.
- `4fb6caf` added crawler, search, profiles, tagging and dispatcher integration
  across 28 files, with 3,798 insertions and 206 deletions.
- The main dispatcher explicitly supported both the existing case-driven
  ingestion path and the newer crawler path.
- Redaction helpers were introduced for email addresses, telephone numbers, IP
  addresses, invite links, handles and URLs.

## Research significance

The platform could now investigate how source acquisition method affected the
material available for classification and relationship analysis, while making
privacy controls part of processing rather than an afterthought.

## Limitation and next step

Multiple collection paths increased capability but also exposed the need for a
single evidence model that could preserve provenance consistently across
source types.
