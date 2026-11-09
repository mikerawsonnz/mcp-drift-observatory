# MCP Drift Observatory

First-hand observations of public [Model Context Protocol](https://modelcontextprotocol.io)
servers: what tools each one **declared**, byte-exactly, and when that declaration changed.

One commit per crawl cycle. A change to a server's tool surface appears as a diff.

## Latest crawl: 2026-11-09 02:02 UTC

12 of 258 observable servers changed their declared tools. Attempted 278: 258 observable, 16 auth-walled, 3 unreachable, 1 blocked.

- [ai.agentsindex/mcp](deltas/2026-11-09/ae90c62287403cba0474.json): description changed; 1 field(s) changed
- [ai.annsa/annsa](deltas/2026-11-09/59d41e60a9e6430b00b0.json): description changed, schema changed; 248 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled **(notable)**
- [ai.apir/verify](deltas/2026-11-09/28b58debdb73ae5a9b8c.json): annotation changed; 15 field(s) changed
- [ai.artemisgtm/gtm-engineer](deltas/2026-11-09/05201622ddbc4614d3f7.json): description changed; 3 field(s) changed; signals: url_introduced
- [ai.atmy/air-quality](deltas/2026-11-09/5f23f4a4f55342a166a0.json): description changed, schema changed; 2 field(s) changed
- [ai.beatra/beatra](deltas/2026-11-09/4f93d616eb97e76f800a.json): count changed, schema changed, tool added; 1 tool(s) added; 3 field(s) changed
- [ai.beliefstate/investor-research](deltas/2026-11-09/d29176e06366706dabab.json): annotation changed, count changed, description changed, field changed, schema changed, tool added, tool removed; 20 tool(s) added; 15 tool(s) removed; 9574 field(s) changed; signals: length_more_than_doubled, url_introduced
- [ai.betslipdoctor/mcp](deltas/2026-11-09/f29327f2a9147dd897c0.json): count changed, description changed, schema changed, tool added; 2 tool(s) added; 118 field(s) changed; signals: length_more_than_doubled
- [ai.bitroad/bitroad](deltas/2026-11-09/e36f79dd929c8eb0f088.json): count changed, tool added; 6 tool(s) added
- [ai.botinfo/robot-market-data](deltas/2026-11-09/6c526ecf6d08b772756f.json): count changed, tool added; 2 tool(s) added
- [ai.bowmark/bowmark](deltas/2026-11-09/e742a173e323c903336e.json): description changed, schema changed; 444 field(s) changed; signals: url_introduced
- [ai.bowmark/bowmark](deltas/2026-11-09/5f2d24be930573ed8878.json): description changed, schema changed; 444 field(s) changed; signals: url_introduced

Changes per day: [2026-11-03](deltas/2026-11-03/) 13, [2026-11-04](deltas/2026-11-04/) 12, [2026-11-05](deltas/2026-11-05/) 11, [2026-11-06](deltas/2026-11-06/) 19, [2026-11-07](deltas/2026-11-07/) 18, [2026-11-08](deltas/2026-11-08/) 11, [2026-11-09](deltas/2026-11-09/) 12

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
