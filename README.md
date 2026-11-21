# MCP Drift Observatory

First-hand observations of public [Model Context Protocol](https://modelcontextprotocol.io)
servers: what tools each one **declared**, byte-exactly, and when that declaration changed.

One commit per crawl cycle. A change to a server's tool surface appears as a diff.

## Latest crawl: 2026-11-21 02:03 UTC

11 of 265 observable servers changed their declared tools. Attempted 290: 265 observable, 22 auth-walled, 3 unreachable, 0 blocked.

- [ad.pantheon/mcp](deltas/2026-11-21/c385e5b261a52bf286e2.json): count changed, description changed, field changed, schema changed, tool added; 1 tool(s) added; 17 field(s) changed; signals: length_more_than_doubled
- [ai.aetherya/mcp](deltas/2026-11-21/0ec8f666c7c4e4781c4d.json): count changed, tool added, tool removed; 26 tool(s) added; 27 tool(s) removed; signals: imperative_language_introduced **(notable)**
- [ai.agenticfabricationnetwork/ufp](deltas/2026-11-21/db3010688319f7ebe01c.json): annotation changed, description changed, schema changed; 17 field(s) changed
- [ai.agentsrank/agentsrank](deltas/2026-11-21/e901088f2b853a367dca.json): description changed; 1 field(s) changed
- [ai.apexrunner/signals](deltas/2026-11-21/d855f635094083c31457.json): count changed, description changed, schema changed, tool added; 2 tool(s) added; 9 field(s) changed
- [ai.assistable/assistable](deltas/2026-11-21/3fd8dc5dfbb162dc18d8.json): description changed, schema changed; 208 field(s) changed; signals: length_more_than_doubled
- [ai.bamf/bamf](deltas/2026-11-21/bcec739ff4350c4ddf27.json): count changed, description changed, schema changed, tool added; 1 tool(s) added; 19 field(s) changed; signals: length_more_than_doubled
- [ai.bittuitive.api/bittuitive](deltas/2026-11-21/c0c8c3bdf1cbda3c2fcd.json): count changed, description changed, schema changed, tool added; 1 tool(s) added; 9 field(s) changed
- [ai.botappetit/bot-appetit](deltas/2026-11-21/e19ce61dadbaa55281fe.json): description changed; 2 field(s) changed; signals: length_more_than_doubled
- [ai.bowmark/bowmark](deltas/2026-11-21/e742a173e323c903336e.json): description changed; 1 field(s) changed
- [ai.bowmark/bowmark](deltas/2026-11-21/5f2d24be930573ed8878.json): description changed; 1 field(s) changed

Changes per day: [2026-11-15](deltas/2026-11-15/) 9, [2026-11-16](deltas/2026-11-16/) 11, [2026-11-17](deltas/2026-11-17/) 21, [2026-11-18](deltas/2026-11-18/) 15, [2026-11-19](deltas/2026-11-19/) 12, [2026-11-20](deltas/2026-11-20/) 15, [2026-11-21](deltas/2026-11-21/) 11

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
