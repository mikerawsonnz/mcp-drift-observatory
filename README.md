# MCP Drift Observatory

First-hand observations of public [Model Context Protocol](https://modelcontextprotocol.io)
servers: what tools each one **declared**, byte-exactly, and when that declaration changed.

One commit per crawl cycle. A change to a server's tool surface appears as a diff.

## Latest crawl: 2026-11-26 02:03 UTC

15 of 270 observable servers changed their declared tools. Attempted 305: 270 observable, 28 auth-walled, 6 unreachable, 1 blocked.

- [ae.discond/discond](deltas/2026-11-26/cd7db03de9f0ecc82710.json): schema changed; 4 field(s) changed
- [agency.zoll/ausfuhr](deltas/2026-11-26/4a6b54c7b92fc67af28d.json): schema changed; 7 field(s) changed
- [ai.a2uicatalog/catalog](deltas/2026-11-26/57663a025cf9685e6622.json): count changed, tool added; 2 tool(s) added
- [ai.achurch/church](deltas/2026-11-26/f7c5ba7365d810101ae3.json): schema changed; 13 field(s) changed
- [ai.adadvisor/mcp-server](deltas/2026-11-26/c151597f0d7058b04027.json): count changed, description changed, schema changed, tool added; 17 tool(s) added; 5 field(s) changed
- [ai.aeoengine/best-ai-search-agency-aeo-report](deltas/2026-11-26/b4551d53f9e6ab4923f1.json): annotation changed, count changed, description changed, schema changed, tool removed; 2 tool(s) removed; 3 field(s) changed
- [ai.agenlify/catalog](deltas/2026-11-26/af8840ee5a1320cc5990.json): schema changed; 7 field(s) changed
- [ai.agentapigate/amazon-product-walmart-shopify-ecommerce-mcp](deltas/2026-11-26/db2d4296f359addb82c6.json): description changed; 1 field(s) changed; signals: length_more_than_doubled
- [ai.agentsrank/agentsrank](deltas/2026-11-26/e901088f2b853a367dca.json): annotation changed, count changed, description changed, tool added; 13 tool(s) added; 26 field(s) changed; signals: length_more_than_doubled
- [ai.aim-shield/mcp](deltas/2026-11-26/89b62f82cc23b3feb966.json): count changed, tool added; 1 tool(s) added
- [ai.arcreport/mcp](deltas/2026-11-26/5b7f6412bf3c3e91b70c.json): description changed; 1 field(s) changed
- [ai.beatra/beatra](deltas/2026-11-26/4f93d616eb97e76f800a.json): description changed, schema changed; 6 field(s) changed
- [ai.bittuitive.api/bittuitive](deltas/2026-11-26/c0c8c3bdf1cbda3c2fcd.json): count changed, description changed, field changed, schema changed, tool added, tool removed; 6 tool(s) added; 4 tool(s) removed; 438 field(s) changed; signals: length_more_than_doubled, url_introduced
- [ai.bondren/docs](deltas/2026-11-26/12e31449e4419f5ba847.json): schema changed; 1 field(s) changed
- [ai.bootpay/mcp](deltas/2026-11-26/a46719d28a156bbc76f4.json): description changed; 2 field(s) changed; signals: length_more_than_doubled

Changes per day: [2026-11-20](deltas/2026-11-20/) 15, [2026-11-21](deltas/2026-11-21/) 11, [2026-11-22](deltas/2026-11-22/) 6, [2026-11-23](deltas/2026-11-23/) 8, [2026-11-24](deltas/2026-11-24/) 3, [2026-11-25](deltas/2026-11-25/) 10, [2026-11-26](deltas/2026-11-26/) 15

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
