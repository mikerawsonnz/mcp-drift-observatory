# MCP Drift Observatory

First-hand observations of public [Model Context Protocol](https://modelcontextprotocol.io)
servers: what tools each one **declared**, byte-exactly, and when that declaration changed.

One commit per crawl cycle. A change to a server's tool surface appears as a diff.

## Latest crawl: 2026-11-18 02:03 UTC

15 of 258 observable servers changed their declared tools. Attempted 285: 258 observable, 20 auth-walled, 7 unreachable, 0 blocked.

- [ae.brainy/grocery-prices](deltas/2026-11-18/f6d1febd0eda9114989e.json): schema changed; 9 field(s) changed
- [ae.brainy/grocery-prices](deltas/2026-11-18/9443ab886276db8be110.json): schema changed; 9 field(s) changed
- [ai.agentgates/compute](deltas/2026-11-18/8e123eb71203886e049b.json): schema changed; 30 field(s) changed
- [ai.ahel/ahel](deltas/2026-11-18/f81cefdfba92e36c524a.json): description changed; 1 field(s) changed; signals: imperative_language_introduced **(notable)**
- [ai.annsa/annsa](deltas/2026-11-18/59d41e60a9e6430b00b0.json): schema changed; 28 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled **(notable)**
- [ai.arcangel/trademark-search](deltas/2026-11-18/51dbd3b220397cebf7d7.json): count changed, description changed, field changed, schema changed, tool added; 3 tool(s) added; 20 field(s) changed
- [ai.athenahq/mcp](deltas/2026-11-18/d1c9dc97b241abc09e4e.json): schema changed; 1 field(s) changed
- [ai.avasis.agents/avasis](deltas/2026-11-18/13be9a5c0441e3f603e0.json): count changed, tool added; 2 tool(s) added
- [ai.bamf/bamf](deltas/2026-11-18/bcec739ff4350c4ddf27.json): count changed, tool added; 2 tool(s) added
- [ai.beatra/beatra](deltas/2026-11-18/4f93d616eb97e76f800a.json): count changed, description changed, schema changed, tool added; 4 tool(s) added; 10 field(s) changed; signals: imperative_language_introduced **(notable)**
- [ai.beliefstate/investor-research](deltas/2026-11-18/d29176e06366706dabab.json): schema changed; 4012 field(s) changed; signals: length_more_than_doubled, url_introduced
- [ai.betslipdoctor/mcp](deltas/2026-11-18/f29327f2a9147dd897c0.json): count changed, description changed, schema changed, tool added; 2 tool(s) added; 15 field(s) changed
- [ai.bittuitive.api/bittuitive](deltas/2026-11-18/c0c8c3bdf1cbda3c2fcd.json): description changed, field changed, schema changed; 4 field(s) changed
- [ai.bowmark/bowmark](deltas/2026-11-18/5f2d24be930573ed8878.json): description changed, schema changed; 2 field(s) changed
- [ai.bowmark/bowmark](deltas/2026-11-18/e742a173e323c903336e.json): description changed, schema changed; 2 field(s) changed

Changes per day: [2026-11-12](deltas/2026-11-12/) 17, [2026-11-13](deltas/2026-11-13/) 13, [2026-11-14](deltas/2026-11-14/) 18, [2026-11-15](deltas/2026-11-15/) 9, [2026-11-16](deltas/2026-11-16/) 11, [2026-11-17](deltas/2026-11-17/) 21, [2026-11-18](deltas/2026-11-18/) 15

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
