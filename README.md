# MCP Drift Observatory

First-hand observations of public [Model Context Protocol](https://modelcontextprotocol.io)
servers: what tools each one **declared**, byte-exactly, and when that declaration changed.

One commit per crawl cycle. A change to a server's tool surface appears as a diff.

## Latest crawl: 2026-11-20 02:03 UTC

15 of 263 observable servers changed their declared tools. Attempted 364: 263 observable, 79 auth-walled, 15 unreachable, 7 blocked.

- [ad.pantheon/mcp](deltas/2026-11-20/c385e5b261a52bf286e2.json): count changed, field changed, schema changed, tool added; 2 tool(s) added; 4 field(s) changed
- [ae.brainy/grocery-prices](deltas/2026-11-20/9443ab886276db8be110.json): schema changed; 42 field(s) changed
- [ae.brainy/grocery-prices](deltas/2026-11-20/f6d1febd0eda9114989e.json): schema changed; 33 field(s) changed
- [ae.discond/discond](deltas/2026-11-20/cd7db03de9f0ecc82710.json): description changed, schema changed; 10 field(s) changed
- [ai.agentgates/compute](deltas/2026-11-20/8e123eb71203886e049b.json): schema changed; 17 field(s) changed; signals: credential_shaped_string_introduced **(notable)**
- [ai.agenticfabricationnetwork/ufp](deltas/2026-11-20/db3010688319f7ebe01c.json): field changed; 6 field(s) changed
- [ai.agentsrank/agentsrank](deltas/2026-11-20/e901088f2b853a367dca.json): count changed, description changed, tool added; 5 tool(s) added; 1 field(s) changed
- [ai.annsa/annsa](deltas/2026-11-20/59d41e60a9e6430b00b0.json): schema changed; 20 field(s) changed; signals: length_more_than_doubled
- [ai.appgoat/mcp](deltas/2026-11-20/9aff2500785fcb6529f4.json): description changed; 2 field(s) changed
- [ai.arcreport/ask](deltas/2026-11-20/5990de195db11012fcfb.json): description changed; 2 field(s) changed
- [ai.beatra/beatra](deltas/2026-11-20/4f93d616eb97e76f800a.json): description changed, schema changed; 180 field(s) changed; signals: length_more_than_doubled
- [ai.bitroad/bitroad](deltas/2026-11-20/e36f79dd929c8eb0f088.json): description changed, schema changed; 5 field(s) changed; signals: length_more_than_doubled
- [ai.bittuitive.api/bittuitive](deltas/2026-11-20/c0c8c3bdf1cbda3c2fcd.json): annotation changed, count changed, description changed, field changed, schema changed, tool added, tool removed; 15 tool(s) added; 29 tool(s) removed; 56 field(s) changed; signals: credential_shaped_string_introduced, imperative_language_introduced, length_more_than_doubled **(notable)**
- [ai.bowmark/bowmark](deltas/2026-11-20/5f2d24be930573ed8878.json): description changed; 1 field(s) changed
- [ai.bowmark/bowmark](deltas/2026-11-20/e742a173e323c903336e.json): description changed; 1 field(s) changed

Changes per day: [2026-11-14](deltas/2026-11-14/) 18, [2026-11-15](deltas/2026-11-15/) 9, [2026-11-16](deltas/2026-11-16/) 11, [2026-11-17](deltas/2026-11-17/) 21, [2026-11-18](deltas/2026-11-18/) 15, [2026-11-19](deltas/2026-11-19/) 12, [2026-11-20](deltas/2026-11-20/) 15

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
