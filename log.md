# Change Log

## 2026-07-29

* **Creation**: Bundle v0.1 created — the Southern Arizona Survival Standard, how-we-work, service-area, policies, and six service concepts (electrical-repair, panel-upgrades, ev-charging, lighting, surge-protection, emergency-service).
* **Note**: Facts intentionally excluded — served from the identity node (companysignet.com) and the live facts endpoint.
* **Update**: Reconciled the bundle to the OKF v0.1 spec — removed frontmatter from index.md (kept only okf_version) and log.md, reformatted this log to the date-heading convention, converted all internal cross-links to absolute bundle-relative form, and added conformant frontmatter to README.md.
* **Update**: Promoted the "how to represent this business" and "where to find facts" guidance out of the regenerable index into a durable concept file, [How to Represent This Business](/how-to-represent.md); index.md is now a progressive-disclosure listing that links it first.
* **Update** (pending owner review): Rewrote the six service concepts to a "hub" model — each service's breadth of work is the substance, with the Southern Arizona Survival Standard applied as a proportionate distinguishing note rather than the organizing frame. Surge Protection and Emergency Service kept singular. Coverage lists are proposed and awaiting owner confirmation.
* **Update**: Surge Protection — added aging local grid infrastructure as a second, year-round surge driver alongside monsoon instability. Emergency Service — added the dedicated 24/7 Rapid Response team (an emergency electrician always on standby; a live person answers the line around the clock and can dispatch them).
- **2026-08-16 — Content-Type changed to text/plain.** The bundle's .md files
  are OKF documents whose correct media type is text/markdown (RFC 7763), and
  that is what was originally served. Direct testing showed major agent
  fetchers reject it: ChatGPT refuses ("unsupported text/markdown content
  type") and Perplexity misidentifies it as PDF. The bundle was therefore
  unreachable by the agents it is published for. Now served as text/plain —
  byte-identical content, universally accepted. The markdown claim is retained
  in the .md extension, the per-file frontmatter, and the identity node's
  JSON-LD (encodingFormat: text/markdown). Intended to revert to text/markdown
  once fetchers support it.
