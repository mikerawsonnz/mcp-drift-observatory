# MCP Drift Observatory

First-hand observations of public [Model Context Protocol](https://modelcontextprotocol.io)
servers: what tools each one **declared**, byte-exactly, and when that declaration changed.

One commit per crawl cycle. A change to a server's tool surface appears as a diff.

## Latest crawl: 2026-11-11 02:04 UTC

15 of 258 observable servers changed their declared tools. Attempted 286: 258 observable, 20 auth-walled, 7 unreachable, 1 blocked.

- [ae.employerofrecord/moha](deltas/2026-11-11/9a53f9818a2eefcb5dfa.json): description changed; 2 field(s) changed
- [agency.zoll/ausfuhr](deltas/2026-11-11/4a6b54c7b92fc67af28d.json): annotation changed, description changed, field changed; 3 field(s) changed
- [ai.1court.state/court-directory](deltas/2026-11-11/c36a3ccafbf96b7eca38.json): count changed, tool added; 2 tool(s) added
- [ai.agentgates/compute](deltas/2026-11-11/8e123eb71203886e049b.json): schema changed; 7 field(s) changed
- [ai.agenticfabricationnetwork/ufp](deltas/2026-11-11/db3010688319f7ebe01c.json): count changed, description changed, schema changed, tool added; 2 tool(s) added; 13 field(s) changed
- [ai.agentsindex/mcp](deltas/2026-11-11/ae90c62287403cba0474.json): count changed, tool removed; 1 tool(s) removed
- [ai.analyticslegends/sap-analytics](deltas/2026-11-11/44700875edd0c1c1f674.json): annotation changed, count changed, description changed, field changed, schema changed, tool added; 2 tool(s) added; 1131 field(s) changed
- [ai.athenahq/mcp](deltas/2026-11-11/d1c9dc97b241abc09e4e.json): count changed, tool added; 4 tool(s) added
- [ai.beliefstate/investor-research](deltas/2026-11-11/d29176e06366706dabab.json): description changed, schema changed; 6011 field(s) changed; signals: length_more_than_doubled
- [ai.betslipdoctor/mcp](deltas/2026-11-11/f29327f2a9147dd897c0.json): count changed, description changed, schema changed, tool added; 1 tool(s) added; 51 field(s) changed; signals: length_more_than_doubled
- [ai.bezal/local-commerce](deltas/2026-11-11/4cca1c526a32cc31d3b0.json): description changed; 5 field(s) changed
- [ai.bluerate/loan-officers](deltas/2026-11-11/8480c0b3b383f5f74749.json): description changed, schema changed; 5 field(s) changed
- [ai.bowmark/bowmark](deltas/2026-11-11/5f2d24be930573ed8878.json): count changed, tool removed; 6 tool(s) removed
- [ai.bowmark/bowmark](deltas/2026-11-11/e742a173e323c903336e.json): count changed, tool removed; 6 tool(s) removed
- [ai.brevium/agent-puzzle-bounty](deltas/2026-11-11/afec8f21ecfee3276880.json): description changed, schema changed; 3 field(s) changed

Changes per day: [2026-11-05](deltas/2026-11-05/) 11, [2026-11-06](deltas/2026-11-06/) 19, [2026-11-07](deltas/2026-11-07/) 18, [2026-11-08](deltas/2026-11-08/) 11, [2026-11-09](deltas/2026-11-09/) 12, [2026-11-10](deltas/2026-11-10/) 9, [2026-11-11](deltas/2026-11-11/) 15

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
