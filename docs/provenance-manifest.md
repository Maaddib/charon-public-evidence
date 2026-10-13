# Evidence provenance manifest

This manifest records the private source object used to verify each public
historical exhibit. Git object IDs are SHA-1 identifiers from the original
local repositories. SHA-256 values are supplied for working files that were
preserved in a later snapshot rather than committed contemporaneously.

The identifiers support internal verification without publishing the original
repositories or their confidential contents.

| Ref | Source evidence | Date | Verifier |
|---|---|---|---|
| H01 | `osint-pipeline`, commit `9f4fb19`, `CharonProject/Charon/main.py` | 2025-12-05 | Git blob `609c6ea8859c904352394d82f7f8ce3d8e5f9581` |
| H02 | `osint-pipeline`, commit `05a3561`, `profiles/edd_individual_v1/profile.yaml` | 2025-12-15 | Git blob `4f762e857d9e91cb95ddc5f8737d59dbe906076a` |
| H03 | `osint-pipeline`, commit `4fb6caf`, `src/charon/main.py` | 2026-03-19 | Git blob `9cb3258b1481716d41b1d1c8190cdde3e194cf97` |
| H04a | `adaptive_discovery.py` | 2026-04-13 | SHA-256 `08844470b2409789aea1c3476d270771b48cd28f1c532881a62b8035c2b13be4` |
| H04b | `reddit_analysis.py` | 2026-04-13 | SHA-256 `d8d14817f17b44e9b0689586d279cc8d7cb34d34752f5350a1bfe4ff20aa12ab` |
| H04c | `tfidf_analysis.py` | 2026-06-14 | SHA-256 `32616ac41cd5ebffcf2a0afea011d21736e4310bce53f69759a9ed8deb663b34` |
| H04d | `classifier.py` | 2026-06-14 | SHA-256 `01dc89b851c0ea116cb35ffa7156509df10d7f448ad28c1f94f2f8448048c3e2` |
| H04e | `entity_extraction.py` | 2026-06-14 | SHA-256 `8be63460c1b67deba08f5c9288a2098dc8f4e9cee4353c595df1d4e125867e6b` |
| H04f | Research ethics configuration | 2026-06-13 | SHA-256 `c6a335424855ef52d7c84bbd6087d51bf6cd16569b9eccc024164ab683ea4672` |
| H05a | `osint-pipeline`, commit `065e662`, `charon/core/models.py` | 2026-07-11 | Git blob `118122d8a2321a323c4593cbee5c79094604565e` |
| H05b | `charon-core`, commit `2122caa` | 2026-10-13 | Git tree `b8a8ef1bf7ff8cd6a89b33a81a284014bba41d24` |

## Evidential limitations

- A Git object ID proves identity within the retained private repository; an
  assessor cannot independently retrieve a private object from its hash alone.
- For H04, modification times and content hashes document the retained files,
  but do not provide the same strength of dating as individual contemporaneous
  commits.
- The manifest deliberately excludes dataset hashes where naming or possession
  could reveal sensitive research material.
