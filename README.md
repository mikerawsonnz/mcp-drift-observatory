# MCP Drift Observatory

First-hand observations of public [Model Context Protocol](https://modelcontextprotocol.io)
servers: what tools each one **declared**, byte-exactly, and when that declaration changed.

One commit per crawl cycle. A change to a server's tool surface appears as a diff.

## Latest crawl: 2026-11-28 02:02 UTC

12 of 270 observable servers changed their declared tools. Attempted 305: 270 observable, 24 auth-walled, 11 unreachable, 0 blocked.

- [ad.pantheon/mcp](deltas/2026-11-28/c385e5b261a52bf286e2.json): count changed, description changed, schema changed, tool removed; 1 tool(s) removed; 3 field(s) changed
- [ae.brainy/brainy-48](deltas/2026-11-28/469089a5676175c4aa62.json): count changed, tool added; 1 tool(s) added
- [ae.mrk/dubai-property](deltas/2026-11-28/bb43c026bcc1ebed4e48.json): annotation changed, description changed, field changed; 44 field(s) changed
- [ai.agentapigate/amazon-product-walmart-shopify-ecommerce-mcp](deltas/2026-11-28/db2d4296f359addb82c6.json): description changed, schema changed; 5 field(s) changed
- [ai.agenticfabricationnetwork/ufp](deltas/2026-11-28/db3010688319f7ebe01c.json): description changed; 3 field(s) changed
- [ai.ahel/ahel](deltas/2026-11-28/f81cefdfba92e36c524a.json): description changed, schema changed; 3 field(s) changed
- [ai.alphabazaar/arena](deltas/2026-11-28/9edc0fb290126b4b5256.json): description changed; 2 field(s) changed; signals: length_more_than_doubled
- [ai.augmap/maps](deltas/2026-11-28/84a4400d881dca99e201.json): count changed, description changed, schema changed, tool added; 1 tool(s) added; 17 field(s) changed
- [ai.azquo/azquo](deltas/2026-11-28/a27acba80c8350153e96.json): count changed, description changed, tool added; 5 tool(s) added; 3 field(s) changed; signals: credential_shaped_string_introduced **(notable)**
- [ai.beatra/beatra](deltas/2026-11-28/4f93d616eb97e76f800a.json): description changed, schema changed; 10 field(s) changed; signals: length_more_than_doubled
- [ai.betslipdoctor/mcp](deltas/2026-11-28/f29327f2a9147dd897c0.json): description changed; 1 field(s) changed
- [ai.bittuitive.api/bittuitive](deltas/2026-11-28/c0c8c3bdf1cbda3c2fcd.json): description changed, schema changed; 10 field(s) changed

Changes per day: [2026-11-22](deltas/2026-11-22/) 6, [2026-11-23](deltas/2026-11-23/) 8, [2026-11-24](deltas/2026-11-24/) 3, [2026-11-25](deltas/2026-11-25/) 10, [2026-11-26](deltas/2026-11-26/) 15, [2026-11-27](deltas/2026-11-27/) 8, [2026-11-28](deltas/2026-11-28/) 12

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
