# b4-index.vercel.app: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/b4-index.vercel.app.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://b4-index.vercel.app/mcp` | 5 | [`b5ae8ae0fba1`](bd4afb01e8fdddfdfa3d.json) | 2026-10-05 |

## Tools at `https://b4-index.vercel.app/mcp`

- `b4_audit`: `For a list of vendor or product names (a stack), with an optional description per row. Example: {"tools": ["Salesforce", {"name": "Lydia Vo…`
- `b4_browse`: `For browsing, filtering, or finding the index's name for something. Example: {"query": "warehouse picking", "domain": "Supply Chain"}. Sear…`
- `b4_compare`: `For one exact category name or id when the question is the build path against the buy path. Example: {"category": "Order Management (OMS)"}…`
- `b4_recommend`: `For a need or problem in words, not a vendor name. Example: {"description": "we need to route warehouse pickers by voice"}. Get B4 Index re…`
- `b4_score`: `For one exact category name or id. Example: {"category": "Expense Management", "org": "medium"}. Score a software category using the B4 Ind…`

## Changes

- 2026-10-05: [description changed](../../deltas/2026-10-05/bd4afb01e8fdddfdfa3d.json): `1 field(s) changed`
- 2026-09-23: [description changed, schema changed](../../deltas/2026-09-23/bd4afb01e8fdddfdfa3d.json): `27 field(s) changed; signals: length_more_than_doubled`
- 2026-09-20: [description changed, schema changed](../../deltas/2026-09-20/bd4afb01e8fdddfdfa3d.json): `48 field(s) changed; signals: length_more_than_doubled`
- 2026-09-08: [description changed, schema changed](../../deltas/2026-09-08/bd4afb01e8fdddfdfa3d.json): `120 field(s) changed; signals: url_introduced`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://b4-index.vercel.app/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
