# MCP Drift Observatory

First-hand observations of public [Model Context Protocol](https://modelcontextprotocol.io)
servers: what tools each one **declared**, byte-exactly, and when that declaration changed.

One commit per crawl cycle. A change to a server's tool surface appears as a diff.

## Latest crawl: 2026-11-08 02:02 UTC

11 of 259 observable servers changed their declared tools. Attempted 286: 259 observable, 24 auth-walled, 2 unreachable, 1 blocked.

- [ai.alphabazaar/arena](deltas/2026-11-08/9edc0fb290126b4b5256.json): description changed; 1 field(s) changed
- [ai.analyticslegends/sap-analytics](deltas/2026-11-08/44700875edd0c1c1f674.json): annotation changed, description changed, field changed, schema changed; 29 field(s) changed
- [ai.artemisgtm/gtm-engineer](deltas/2026-11-08/05201622ddbc4614d3f7.json): description changed; 2 field(s) changed; signals: url_introduced
- [ai.asms/asms](deltas/2026-11-08/4e29eb0cd32d68164c8a.json): count changed, description changed, tool added; 2 tool(s) added; 1 field(s) changed
- [ai.beliefstate/investor-research](deltas/2026-11-08/d29176e06366706dabab.json): schema changed; 32408 field(s) changed; signals: length_more_than_doubled
- [ai.betslipdoctor/mcp](deltas/2026-11-08/f29327f2a9147dd897c0.json): count changed, description changed, schema changed, tool added; 2 tool(s) added; 2370 field(s) changed; signals: length_more_than_doubled, url_introduced
- [ai.bezal/local-commerce](deltas/2026-11-08/4cca1c526a32cc31d3b0.json): schema changed; 1 field(s) changed
- [ai.bobwork/emailwarmup](deltas/2026-11-08/05c4b5d497c7d086d782.json): description changed; 1 field(s) changed
- [ai.bowmark/bowmark](deltas/2026-11-08/5f2d24be930573ed8878.json): annotation changed, count changed, description changed, field changed, schema changed, tool added; 1 tool(s) added; 22 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled **(notable)**
- [ai.bowmark/bowmark](deltas/2026-11-08/e742a173e323c903336e.json): annotation changed, count changed, description changed, field changed, schema changed, tool added; 1 tool(s) added; 22 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled **(notable)**
- [ai.bumit/verify-business](deltas/2026-11-08/d0fe06dca65feccd4008.json): count changed, tool added; 2 tool(s) added

Changes per day: [2026-11-02](deltas/2026-11-02/) 13, [2026-11-03](deltas/2026-11-03/) 13, [2026-11-04](deltas/2026-11-04/) 12, [2026-11-05](deltas/2026-11-05/) 11, [2026-11-06](deltas/2026-11-06/) 19, [2026-11-07](deltas/2026-11-07/) 18, [2026-11-08](deltas/2026-11-08/) 11

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
