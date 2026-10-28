# MCP Drift Observatory

First-hand observations of public [Model Context Protocol](https://modelcontextprotocol.io)
servers: what tools each one **declared**, byte-exactly, and when that declaration changed.

One commit per crawl cycle. A change to a server's tool surface appears as a diff.

## Latest crawl: 2026-10-28 02:04 UTC

18 of 247 observable servers changed their declared tools. Attempted 348: 247 observable, 94 auth-walled, 5 unreachable, 2 blocked.

- [ai.1court.state/court-directory](deltas/2026-10-28/c36a3ccafbf96b7eca38.json): description changed, schema changed; 3 field(s) changed
- [ai.agentlookups/counterscript](deltas/2026-10-28/dd2c3869e34da13c6fa0.json): description changed; 1 field(s) changed
- [ai.agentlookups/groundrules](deltas/2026-10-28/ca5a5fcdc8fec39a1452.json): description changed, schema changed; 5 field(s) changed
- [ai.agentlookups/groundtruth](deltas/2026-10-28/e4737c6c08d0e753c7d6.json): description changed; 3 field(s) changed
- [ai.agentlookups/overassessed](deltas/2026-10-28/c6dae6909013339ef565.json): description changed, schema changed; 3 field(s) changed
- [ai.agentlookups/plumbline](deltas/2026-10-28/7279f3c88a6837829bbe.json): description changed, schema changed; 2 field(s) changed; signals: length_more_than_doubled
- [ai.agentmash/agentmash](deltas/2026-10-28/ebf7dd27800b023a6de2.json): schema changed; 4 field(s) changed
- [ai.analyticslegends/sap-analytics](deltas/2026-10-28/44700875edd0c1c1f674.json): description changed; 9 field(s) changed
- [ai.appgoat/mcp](deltas/2026-10-28/9aff2500785fcb6529f4.json): count changed, description changed, schema changed, tool removed; 3 tool(s) removed; 2 field(s) changed
- [ai.atako/mcp](deltas/2026-10-28/77558449d7b666a698fe.json): annotation changed, description changed, schema changed; 13 field(s) changed
- [ai.athenahq/mcp](deltas/2026-10-28/d1c9dc97b241abc09e4e.json): count changed, tool added; 1 tool(s) added
- [ai.atmy/air-quality](deltas/2026-10-28/5f23f4a4f55342a166a0.json): count changed, tool added; 5 tool(s) added
- [ai.azquo/azquo](deltas/2026-10-28/a27acba80c8350153e96.json): count changed, description changed, tool added; 1 tool(s) added; 2 field(s) changed
- [ai.beatra/beatra](deltas/2026-10-28/4f93d616eb97e76f800a.json): count changed, description changed, schema changed, tool added; 1 tool(s) added; 100 field(s) changed
- [ai.beliefstate/investor-research](deltas/2026-10-28/d29176e06366706dabab.json): description changed, schema changed; 40618 field(s) changed; signals: length_more_than_doubled
- [ai.betslipdoctor/mcp](deltas/2026-10-28/f29327f2a9147dd897c0.json): description changed, schema changed; 7 field(s) changed
- [ai.bitroad/bitroad](deltas/2026-10-28/e36f79dd929c8eb0f088.json): description changed, schema changed; 312 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled **(notable)**
- [ai.buildersinfintech/fintech-data](deltas/2026-10-28/5838aac513603a4cf3ab.json): description changed, schema changed; 5 field(s) changed

Changes per day: [2026-10-22](deltas/2026-10-22/) 11, [2026-10-23](deltas/2026-10-23/) 7, [2026-10-24](deltas/2026-10-24/) 15, [2026-10-25](deltas/2026-10-25/) 13, [2026-10-26](deltas/2026-10-26/) 7, [2026-10-27](deltas/2026-10-27/) 16, [2026-10-28](deltas/2026-10-28/) 18

## What this is

`servers/<host>/<key>.json` is the current declared tool surface for one server.
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
- **The RSS-A Agent Network board:** the observatory posts each crawl's changes there,
  https://hub.rssa.getvda.ai/network/board

_Generated by [GOSCE](https://agents.getvda.ai). Not affiliated with any server listed._
