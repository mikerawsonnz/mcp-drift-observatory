# MCP Drift Observatory

First-hand observations of public [Model Context Protocol](https://modelcontextprotocol.io)
servers: what tools each one **declared**, byte-exactly, and when that declaration changed.

One commit per crawl cycle. A change to a server's tool surface appears as a diff.

## Latest crawl: 2026-11-07 02:03 UTC

18 of 263 observable servers changed their declared tools. Attempted 287: 263 observable, 18 auth-walled, 5 unreachable, 1 blocked.

- [ad.tide/mcp](deltas/2026-11-07/cf57e535ac93234bd658.json): description changed, schema changed; 3 field(s) changed
- [ai.1court.state/court-directory](deltas/2026-11-07/c36a3ccafbf96b7eca38.json): annotation changed, count changed, description changed, schema changed, tool added; 3 tool(s) added; 13 field(s) changed; signals: length_more_than_doubled
- [ai.agentgates/compute](deltas/2026-11-07/8e123eb71203886e049b.json): description changed, schema changed; 7 field(s) changed
- [ai.analyticslegends/sap-analytics](deltas/2026-11-07/44700875edd0c1c1f674.json): count changed, tool added; 1 tool(s) added
- [ai.arcreport/ask](deltas/2026-11-07/5990de195db11012fcfb.json): annotation changed, count changed, description changed, field changed, schema changed, tool added; 7 tool(s) added; 53 field(s) changed; signals: url_introduced
- [ai.arcreport/mcp](deltas/2026-11-07/5b7f6412bf3c3e91b70c.json): description changed, schema changed; 9 field(s) changed; signals: length_more_than_doubled
- [ai.artemisgtm/gtm-engineer](deltas/2026-11-07/05201622ddbc4614d3f7.json): description changed; 1 field(s) changed; signals: url_introduced
- [ai.athenahq/mcp](deltas/2026-11-07/d1c9dc97b241abc09e4e.json): count changed, tool added; 2 tool(s) added
- [ai.atmy/air-quality](deltas/2026-11-07/5f23f4a4f55342a166a0.json): description changed; 1 field(s) changed
- [ai.autoposter/autoposter](deltas/2026-11-07/b4c1ac88f1fe4ef8d46e.json): count changed, schema changed, tool added; 2 tool(s) added; 24 field(s) changed
- [ai.bamf/bamf](deltas/2026-11-07/bcec739ff4350c4ddf27.json): count changed, tool added; 3 tool(s) added
- [ai.beatra/beatra](deltas/2026-11-07/4f93d616eb97e76f800a.json): description changed, schema changed; 72 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled **(notable)**
- [ai.betslipdoctor/mcp](deltas/2026-11-07/f29327f2a9147dd897c0.json): description changed, schema changed; 661 field(s) changed; signals: length_more_than_doubled, url_introduced
- [ai.blast-radius/blast-radius](deltas/2026-11-07/6e0fc9f43e7d724c3c48.json): description changed; 1 field(s) changed
- [ai.bowmark/bowmark](deltas/2026-11-07/e742a173e323c903336e.json): annotation changed, count changed, description changed, field changed, schema changed, tool added; 1 tool(s) added; 51 field(s) changed
- [ai.bowmark/bowmark](deltas/2026-11-07/5f2d24be930573ed8878.json): annotation changed, count changed, description changed, field changed, schema changed, tool added; 1 tool(s) added; 51 field(s) changed
- [ai.buildersinfintech/fintech-data](deltas/2026-11-07/5838aac513603a4cf3ab.json): count changed, tool added; 2 tool(s) added
- [ai.centralcity/central-city](deltas/2026-11-07/51d51649944e58301c50.json): schema changed; 2 field(s) changed

Changes per day: [2026-11-01](deltas/2026-11-01/) 11, [2026-11-02](deltas/2026-11-02/) 13, [2026-11-03](deltas/2026-11-03/) 13, [2026-11-04](deltas/2026-11-04/) 12, [2026-11-05](deltas/2026-11-05/) 11, [2026-11-06](deltas/2026-11-06/) 19, [2026-11-07](deltas/2026-11-07/) 18

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

_Generated by [GOSCE](https://agents.getvda.ai). Not affiliated with any server listed._
