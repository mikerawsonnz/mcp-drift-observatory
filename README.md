# MCP Drift Observatory

First-hand observations of public [Model Context Protocol](https://modelcontextprotocol.io)
servers: what tools each one **declared**, byte-exactly, and when that declaration changed.

One commit per crawl cycle. A change to a server's tool surface appears as a diff.

## Latest crawl: 2026-11-12 02:03 UTC

17 of 259 observable servers changed their declared tools. Attempted 290: 259 observable, 26 auth-walled, 4 unreachable, 1 blocked.

- [ac.mizan/registry](deltas/2026-11-12/70c77423ed2d6ce6e69e.json): schema changed; 19 field(s) changed; signals: length_more_than_doubled
- [agency.thirdhemisphere/ai-authority-index](deltas/2026-11-12/b750b5af8da6e753c90e.json): field changed; 1 field(s) changed
- [ai.a2uicatalog/catalog](deltas/2026-11-12/57663a025cf9685e6622.json): field changed; 14 field(s) changed
- [ai.agentgates/compute](deltas/2026-11-12/8e123eb71203886e049b.json): annotation changed, description changed, field changed, schema changed; 26 field(s) changed
- [ai.ahel/ahel](deltas/2026-11-12/f81cefdfba92e36c524a.json): annotation changed, description changed, field changed, schema changed, tool added, tool removed; 1 tool(s) added; 1 tool(s) removed; 34 field(s) changed
- [ai.aibotoffice/bot-office](deltas/2026-11-12/0850381780b97d0055f6.json): description changed, schema changed; 8 field(s) changed; signals: credential_shaped_string_introduced **(notable)**
- [ai.analyticslegends/sap-analytics](deltas/2026-11-12/44700875edd0c1c1f674.json): schema changed; 4 field(s) changed
- [ai.annsa/annsa](deltas/2026-11-12/59d41e60a9e6430b00b0.json): schema changed; 10 field(s) changed
- [ai.appgoat/mcp](deltas/2026-11-12/9aff2500785fcb6529f4.json): description changed, schema changed; 28 field(s) changed
- [ai.athenahq/mcp](deltas/2026-11-12/d1c9dc97b241abc09e4e.json): description changed, schema changed; 36 field(s) changed
- [ai.bamf/bamf](deltas/2026-11-12/bcec739ff4350c4ddf27.json): count changed, schema changed, tool added; 10 tool(s) added; 13 field(s) changed
- [ai.beatra/beatra](deltas/2026-11-12/4f93d616eb97e76f800a.json): count changed, description changed, schema changed, tool added; 2 tool(s) added; 107 field(s) changed
- [ai.beliefstate/investor-research](deltas/2026-11-12/d29176e06366706dabab.json): schema changed; 3 field(s) changed
- [ai.bezal/local-commerce](deltas/2026-11-12/4cca1c526a32cc31d3b0.json): description changed; 1 field(s) changed
- [ai.bitroad/bitroad](deltas/2026-11-12/e36f79dd929c8eb0f088.json): count changed, description changed, tool added; 2 tool(s) added; 4 field(s) changed; signals: length_more_than_doubled
- [ai.blast-radius/blast-radius](deltas/2026-11-12/6e0fc9f43e7d724c3c48.json): description changed; 1 field(s) changed
- [ai.bluerate/loan-officers](deltas/2026-11-12/8480c0b3b383f5f74749.json): annotation changed, description changed, schema changed; 4 field(s) changed

Changes per day: [2026-11-06](deltas/2026-11-06/) 19, [2026-11-07](deltas/2026-11-07/) 18, [2026-11-08](deltas/2026-11-08/) 11, [2026-11-09](deltas/2026-11-09/) 12, [2026-11-10](deltas/2026-11-10/) 9, [2026-11-11](deltas/2026-11-11/) 15, [2026-11-12](deltas/2026-11-12/) 17

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
