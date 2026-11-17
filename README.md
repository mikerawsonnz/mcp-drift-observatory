# MCP Drift Observatory

First-hand observations of public [Model Context Protocol](https://modelcontextprotocol.io)
servers: what tools each one **declared**, byte-exactly, and when that declaration changed.

One commit per crawl cycle. A change to a server's tool surface appears as a diff.

## Latest crawl: 2026-11-17 02:02 UTC

21 of 253 observable servers changed their declared tools. Attempted 279: 253 observable, 20 auth-walled, 2 unreachable, 4 blocked.

- [ad.pantheon/mcp](deltas/2026-11-17/c385e5b261a52bf286e2.json): count changed, tool added; 5 tool(s) added
- [ae.brainy/grocery-prices](deltas/2026-11-17/9443ab886276db8be110.json): schema changed; 336 field(s) changed
- [ae.discond/discond](deltas/2026-11-17/cd7db03de9f0ecc82710.json): schema changed; 35 field(s) changed; signals: imperative_language_introduced **(notable)**
- [aero.events/events](deltas/2026-11-17/0ab3287c5fc33c6e22e5.json): description changed, schema changed; 2 field(s) changed
- [ai.agentboard/agentboard](deltas/2026-11-17/89334b6ae3243e4e2df6.json): count changed, description changed, tool added; 1 tool(s) added; 8 field(s) changed; signals: length_more_than_doubled
- [ai.agentsrank/agentsrank](deltas/2026-11-17/e901088f2b853a367dca.json): count changed, description changed, schema changed, tool added; 3 tool(s) added; 13 field(s) changed; signals: length_more_than_doubled
- [ai.annsa/annsa](deltas/2026-11-17/59d41e60a9e6430b00b0.json): schema changed; 6 field(s) changed
- [ai.appgoat/mcp](deltas/2026-11-17/9aff2500785fcb6529f4.json): description changed, schema changed; 9 field(s) changed
- [ai.arcangel/trademark-search](deltas/2026-11-17/51dbd3b220397cebf7d7.json): count changed, field changed, tool added; 3 tool(s) added; 6 field(s) changed
- [ai.arclan/registry](deltas/2026-11-17/0b01ebd7cd8a49a80df5.json): count changed, tool added; 2 tool(s) added
- [ai.arcreport/ask](deltas/2026-11-17/5990de195db11012fcfb.json): count changed, description changed, schema changed, tool added; 1 tool(s) added; 10 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled **(notable)**
- [ai.arcreport/mcp](deltas/2026-11-17/5b7f6412bf3c3e91b70c.json): schema changed; 6 field(s) changed; signals: length_more_than_doubled
- [ai.athenahq/mcp](deltas/2026-11-17/d1c9dc97b241abc09e4e.json): description changed, schema changed; 15 field(s) changed
- [ai.avasis.agents/avasis](deltas/2026-11-17/13be9a5c0441e3f603e0.json): count changed, tool added, tool removed; 3 tool(s) added; 4 tool(s) removed
- [ai.beatra/beatra](deltas/2026-11-17/4f93d616eb97e76f800a.json): schema changed; 8 field(s) changed
- [ai.betslipdoctor/mcp](deltas/2026-11-17/f29327f2a9147dd897c0.json): description changed, schema changed; 16 field(s) changed
- [ai.bidclub/bidclub](deltas/2026-11-17/aec34e730ed613f0048d.json): description changed; 1 field(s) changed
- [ai.bittuitive.api/bittuitive](deltas/2026-11-17/c0c8c3bdf1cbda3c2fcd.json): count changed, description changed, field changed, schema changed, tool added; 12 tool(s) added; 49 field(s) changed; signals: imperative_language_introduced, url_introduced **(notable)**
- [ai.booqer/booqer](deltas/2026-11-17/9bb78baa139078dd6da5.json): description changed, schema changed; 3 field(s) changed
- [ai.bowmark/bowmark](deltas/2026-11-17/5f2d24be930573ed8878.json): description changed, schema changed; 4 field(s) changed
- [ai.bowmark/bowmark](deltas/2026-11-17/e742a173e323c903336e.json): description changed, schema changed; 4 field(s) changed

Changes per day: [2026-11-11](deltas/2026-11-11/) 15, [2026-11-12](deltas/2026-11-12/) 17, [2026-11-13](deltas/2026-11-13/) 13, [2026-11-14](deltas/2026-11-14/) 18, [2026-11-15](deltas/2026-11-15/) 9, [2026-11-16](deltas/2026-11-16/) 11, [2026-11-17](deltas/2026-11-17/) 21

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
