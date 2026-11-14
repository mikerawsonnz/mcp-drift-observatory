# MCP Drift Observatory

First-hand observations of public [Model Context Protocol](https://modelcontextprotocol.io)
servers: what tools each one **declared**, byte-exactly, and when that declaration changed.

One commit per crawl cycle. A change to a server's tool surface appears as a diff.

## Latest crawl: 2026-11-14 02:02 UTC

18 of 251 observable servers changed their declared tools. Attempted 277: 251 observable, 22 auth-walled, 3 unreachable, 1 blocked.

- [ad.pantheon/mcp](deltas/2026-11-14/c385e5b261a52bf286e2.json): annotation changed, description changed, field changed, schema changed; 244 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled **(notable)**
- [ae.propick/propick](deltas/2026-11-14/91748b15f7242e1c689f.json): description changed, schema changed, tool added, tool removed; 1 tool(s) added; 1 tool(s) removed; 17 field(s) changed
- [agency.thirdhemisphere/ai-authority-index](deltas/2026-11-14/b750b5af8da6e753c90e.json): description changed; 6 field(s) changed
- [ai.a2uicatalog/catalog](deltas/2026-11-14/57663a025cf9685e6622.json): description changed, field changed, schema changed; 25 field(s) changed; signals: length_more_than_doubled
- [ai.agenticfabricationnetwork/ufp](deltas/2026-11-14/db3010688319f7ebe01c.json): count changed, description changed, schema changed, tool added; 8 tool(s) added; 232 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled **(notable)**
- [ai.agilex.service/docs](deltas/2026-11-14/4f9bb92e8706287aa594.json): description changed; 2 field(s) changed
- [ai.ahel/ahel](deltas/2026-11-14/f81cefdfba92e36c524a.json): schema changed; 1 field(s) changed; signals: length_more_than_doubled
- [ai.ankra/docs](deltas/2026-11-14/e88cfce9285473e78a88.json): description changed; 1 field(s) changed
- [ai.annsa/annsa](deltas/2026-11-14/59d41e60a9e6430b00b0.json): field changed, schema changed; 17 field(s) changed
- [ai.apexrunner/signals](deltas/2026-11-14/d855f635094083c31457.json): count changed, description changed, tool added; 1 tool(s) added; 1 field(s) changed
- [ai.athenahq/mcp](deltas/2026-11-14/d1c9dc97b241abc09e4e.json): annotation changed; 5 field(s) changed
- [ai.atmy/air-quality](deltas/2026-11-14/5f23f4a4f55342a166a0.json): count changed, tool added; 1 tool(s) added
- [ai.bareun/bareun](deltas/2026-11-14/433537aec8fde738c83b.json): annotation changed, description changed, schema changed; 51 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled **(notable)**
- [ai.beliefstate/investor-research](deltas/2026-11-14/d29176e06366706dabab.json): description changed, schema changed; 8006 field(s) changed; signals: length_more_than_doubled, url_introduced
- [ai.betslipdoctor/mcp](deltas/2026-11-14/f29327f2a9147dd897c0.json): count changed, tool added; 1 tool(s) added
- [ai.bezal/local-commerce](deltas/2026-11-14/4cca1c526a32cc31d3b0.json): schema changed; 1 field(s) changed
- [ai.bowmark/bowmark](deltas/2026-11-14/e742a173e323c903336e.json): schema changed; 6 field(s) changed
- [ai.bowmark/bowmark](deltas/2026-11-14/5f2d24be930573ed8878.json): schema changed; 6 field(s) changed

Changes per day: [2026-11-08](deltas/2026-11-08/) 11, [2026-11-09](deltas/2026-11-09/) 12, [2026-11-10](deltas/2026-11-10/) 9, [2026-11-11](deltas/2026-11-11/) 15, [2026-11-12](deltas/2026-11-12/) 17, [2026-11-13](deltas/2026-11-13/) 13, [2026-11-14](deltas/2026-11-14/) 18

## What this is

`servers/<host>/<key>.json` is the current declared tool surface for one server, and
`servers/<host>/` has a page listing its tools and every observed change. [`servers/`](servers/) lists every host.
`deltas/<date>/<key>.json` is a single observed change, with the hash before and after.
`index.json` summarises coverage, including the servers we could **not** observe.

Hashes are SHA-256 over canonical JSON with `ensure_ascii=False` and tools sorted by
name, so reordering is not drift and a non-ASCII description does not change the hash
depending on who serialised it.

## What this does NOT prove

We observe **declarations, not behaviour**. A server whose tool name, description and
schema stay byte-identical while its remote implementation changes is invisible here —
as it is to every client-side defence. If you need behavioural assurance, this is not it.

We also do not claim completeness. Roughly three quarters of discovered MCP servers
require authentication and cannot be observed by anyone without credentials; they are
counted in `index.json` rather than dropped, so the denominator stays visible.

## Verifying independently

Each observed change is also sealed to [VDA Witness](https://witness.getvda.ai). A seal
proves that at time T this observer recorded this hash — **not** that the underlying
claim is true. Verification needs no account:

```bash
curl -sX POST https://witness.getvda.ai/api/witness/verify \
  -H 'content-type: application/json' -d '{"record": <the record>}'
```

The git history is the second, independent record: clone this repo and the commit graph
shows what was published and when, without trusting us or Witness.

## Use it from an agent

- **MCP / A2A:** `https://drift.getvda.ai/mcp` and `https://drift.getvda.ai/a2a/`. `drift_status`, `drift_check`
  (has this server changed since a hash you hold?) and `drift_hash` (reproduce our hash yourself) are free.
- **Signed feed (RSS-A):** https://storage.googleapis.com/c2md-493808-gosce-rssa/feeds/drift/feed.rss, one entry
  per crawl with changes.
- **Follow one server:** each server page links an Atom feed of changes to that server alone
  (`https://github.com/<this repo>/commits/main/servers/<host>.atom`), quiet unless its declared tools change.
- **The RSS-A Agent Network board:** the observatory posts each crawl's changes there,
  https://hub.rssa.getvda.ai/network/board?via=drift-archive
- **Telegram:** the same digest after each crawl, https://t.me/mcp_drift_alerts

_Generated by [GOSCE](https://agents.getvda.ai). Not affiliated with any server listed._
