# Inspectable evidence

The files in this directory are the assessor-facing evidence layer. Each stage
contains a narrative exhibit and one or more compact primary-evidence records
derived from the retained private repositories.

| Stage | Narrative | Primary evidence |
|---|---|---|
| H01 | [Original OSINT Pipeline](01-original-osint-pipeline.md) | [Initial commit record](artifacts/H01-initial-commit.txt), [historical entry-point excerpt](artifacts/H01-entry-point-excerpt.py.txt) |
| H02 | [Research-led EDD](02-research-led-edd.md) | [EDD structure recorded by Git](artifacts/H02-edd-structure.txt) |
| H03 | [Collection expansion](03-collection-expansion.md) | [Crawler and dispatcher commit record](artifacts/H03-collection-expansion.txt) |
| H04 | [Research experiments](04-research-experiments.md) | [Dated experiment manifest](artifacts/H04-research-experiment-manifest.txt), [research ethics controls](artifacts/H04-research-ethics.yaml.txt) |
| H05 | [Charon Core](05-charon-core.md) | [Repository transition record](artifacts/H05-repository-transition.txt), [domain-model progression](artifacts/H05-domain-model-progression.txt) |

These records are intentionally small. They establish dates, structure and
development decisions without publishing the complete application, research
corpus, investigation data or commercial methodology.

## Verification model

- Commit hashes, dates and change statistics were read directly from the local
  Git object databases.
- Historical source excerpts were retrieved from the named commit, not from the
  present working tree.
- Git blob identifiers and SHA-256 values are recorded in the
  [provenance manifest](../docs/provenance-manifest.md).
- Research files that lacked individual contemporaneous commits are explicitly
  identified as weaker, timestamp-supported evidence.
