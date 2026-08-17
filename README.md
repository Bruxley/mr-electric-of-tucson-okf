---
type: Reference
title: Mr. Electric of Tucson — OKF Knowledge Bundle
description: What this bundle is, where it is served, and where facts live versus knowledge.
timestamp: 2026-07-29
---

# Mr. Electric of Tucson — OKF Knowledge Bundle

An [Open Knowledge Format](https://cloud.google.com/blog/products/data-analytics/how-the-open-knowledge-format-can-improve-data-sharing) (OKF) bundle: curated, agent-readable reference knowledge about Mr. Electric of Tucson.

- **This bundle = knowledge/judgment** (how the business works, what the Southern Arizona Survival Standard is, how services are approached).
- **Facts** (address, phone, hours, license, identifiers) are NOT here — they are served from the identity record at <https://companysignet.com/> and the live facts endpoint.

Served at: `https://companysignet.com/okf/`

Entry point: [`index.md`](/index.md)

## Why .md files are served as text/plain

Correct media type for these files is `text/markdown` (RFC 7763). We serve
`text/plain` instead because major agent fetchers reject `text/markdown`
(verified 2026-08: ChatGPT refuses it; Perplexity misparses it as PDF),
making the bundle unreachable by its intended consumers. Content is identical.
See the comment block in `_headers`. Revert when the ecosystem catches up.
