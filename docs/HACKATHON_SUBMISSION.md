# AI Builders Hackathon submission — project history and hackathon-period work

This document states plainly what existed before the AI Builders Hackathon and what was built during
it (21 August – 15 September 2026), so judges can assess the submission against the rule that work
must be created during the hackathon period.

## Project history

- **Kairos was not started during the hackathon.** Development began on **27 June 2026**; 96 commits
  were made before the hackathon opened on 21 August.
- **An earlier version was submitted elsewhere.** The codebase as of commit `b81ed1f` (24 August 2026)
  was submitted to the **ET AI Hackathon 2.0**. That submission is published as release
  [`v1.0.0`](https://github.com/kr7shnasomani/kairos/releases/tag/v1.0.0) in the original repository.
- **This repository** (`deterium-kairos`) is a copy of the original repository
  ([`kr7shnasomani/kairos`](https://github.com/kr7shnasomani/kairos)) at the AI Builders submission
  commit `c654615` (14 September 2026), made for this submission. Its full commit history, with dates,
  remains public in the original repository.

## Work during the hackathon period

**28 commits** between 22 August and 14 September 2026. Measured from the last commit before the
window (`e76045d`, 17 August 2026) to the submission commit: **313 files changed, +19,903 / −2,710
lines**. Every commit below links to the original repository.

### 22 – 25 August 2026

- Bulk asset import endpoint and expanded test infrastructure ([`d261425`](https://github.com/kr7shnasomani/kairos/commit/d261425))
- System design documentation and architecture diagrams ([`0f61a14`](https://github.com/kr7shnasomani/kairos/commit/0f61a14))
- Frontend senior review pass — 32 of 38 items ([`664dde4`](https://github.com/kr7shnasomani/kairos/commit/664dde4))
- Model-validation metrics with caching and asset-specific partitioning ([`33d2ac4`](https://github.com/kr7shnasomani/kairos/commit/33d2ac4))
- Knowledge-graph linkage completeness benchmark ([`612d232`](https://github.com/kr7shnasomani/kairos/commit/612d232))
- Supply-chain integrity checks for model provenance ([`5ae607d`](https://github.com/kr7shnasomani/kairos/commit/5ae607d))
- OCR extraction path fixes for multimodal perception ([`28c8196`](https://github.com/kr7shnasomani/kairos/commit/28c8196))
- Corpus filtering consolidation and Copilot / System Health wiring fixes ([`58cf492`](https://github.com/kr7shnasomani/kairos/commit/58cf492))
- Shared image-resizing utility and OCR span-gate tests ([`ae8ef07`](https://github.com/kr7shnasomani/kairos/commit/ae8ef07))
- Retrieval noise-filter bug fixes and updated benchmark results ([`2b84ab5`](https://github.com/kr7shnasomani/kairos/commit/2b84ab5))
- Graph search titles, test-artifact filtering and health-probe auth ([`9becdea`](https://github.com/kr7shnasomani/kairos/commit/9becdea))
- Frontend overlay, navigation-rail and modal fixes ([`03c77df`](https://github.com/kr7shnasomani/kairos/commit/03c77df), [`f79a33a`](https://github.com/kr7shnasomani/kairos/commit/f79a33a))
- Demo ingest tooling, stage runbook and per-store ingest verifier ([`d283aaa`](https://github.com/kr7shnasomani/kairos/commit/d283aaa), [`9f25d34`](https://github.com/kr7shnasomani/kairos/commit/9f25d34))
- RCA evidence retrieval and document-status adapter fixes ([`5d0aac6`](https://github.com/kr7shnasomani/kairos/commit/5d0aac6), [`541ae16`](https://github.com/kr7shnasomani/kairos/commit/541ae16), [`b81ed1f`](https://github.com/kr7shnasomani/kairos/commit/b81ed1f))

### 14 September 2026

- **New product surfaces:** conflict detail; timestamp-drift and push-volume-gate reports; document
  extraction results and PII-redacted export; asset hierarchy and asset-scoped search; separate asset
  registration and identity confirmation ([`c5cd727`](https://github.com/kr7shnasomani/kairos/commit/c5cd727))
- **OCR review workflow** — held documents released or rejected by a reliability engineer or admin,
  with audit; frontend fixture fallbacks removed; image utilities consolidated ([`5dd643c`](https://github.com/kr7shnasomani/kairos/commit/5dd643c))
- **Security and correctness** — dependency advisories cleared; reads run as the signed-in user;
  identity confirmations attributed from the session; exception text no longer returned to clients;
  code-scanning findings closed ([`3e7a5ca`](https://github.com/kr7shnasomani/kairos/commit/3e7a5ca), [`dec49b6`](https://github.com/kr7shnasomani/kairos/commit/dec49b6))
- **CI and operations** — GitHub Actions updated; vulnerability scan pinned to a working release;
  Go and Dockerfile lint findings fixed; connector image runs non-root with a working healthcheck
  ([`5976179`](https://github.com/kr7shnasomani/kairos/commit/5976179), [`5d8c8a4`](https://github.com/kr7shnasomani/kairos/commit/5d8c8a4), [`12dfc51`](https://github.com/kr7shnasomani/kairos/commit/12dfc51), [`7bece53`](https://github.com/kr7shnasomani/kairos/commit/7bece53))
- **Reliability** — Copilot streaming fixed; Supabase reads survive dropped connections; streamed
  answers no longer show raw model markers ([`c654615`](https://github.com/kr7shnasomani/kairos/commit/c654615))

## State at submission

- 494 service-free backend tests and 271 frontend tests passing; production frontend build and
  backend image build.
- End-to-end flow suite 46/46, including permit-to-work dual sign-off, deviation handling and
  document supersession.
- All CI workflows green on `c654615`; no open code-scanning alerts.
