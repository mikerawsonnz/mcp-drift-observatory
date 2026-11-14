# service.agilex.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/service.agilex.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://service.agilex.ai/agilex-docs/mcp` | 5 | [`1eed8ecd5574`](4f9bb92e8706287aa594.json) | 2026-11-14 |

## Tools at `https://service.agilex.ai/agilex-docs/mcp`

- `find_in_doc`: `Locate a passage *inside* one manual, without paging through it. Use this after ''search_docs'' whenever you need a specific table, command…`
- `get_doc`: `Read one documentation page as Markdown. Call this with a ''doc_id'' returned by ''search_docs'' (or a slug such as ''ymZimX7JLe''). Manual…`
- `list_docs`: `List documented pages, optionally inside one space. Use when the caller wants an inventory ("what manuals exist for ranger") rather than an…`
- `list_spaces`: `List the public documentation spaces with page counts. Call this when the caller is unsure which product family a document belongs to, or t…`
- `search_docs`: `Full-text search over the official AGILEX product documentation. Use this first for any question about AGILEX hardware: pinouts, CAN protoc…`

## Changes

- 2026-11-14: [description changed](../../deltas/2026-11-14/4f9bb92e8706287aa594.json): `2 field(s) changed`
- 2026-11-13: [description changed](../../deltas/2026-11-13/4f9bb92e8706287aa594.json): `1 field(s) changed`
- 2026-11-05: [annotation changed, count changed, description changed, schema changed, tool added](../../deltas/2026-11-05/4f9bb92e8706287aa594.json): `1 tool(s) added; 27 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://service.agilex.ai/agilex-docs/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
