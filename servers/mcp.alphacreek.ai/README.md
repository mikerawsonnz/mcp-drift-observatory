# mcp.alphacreek.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.alphacreek.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.alphacreek.ai/mcp` | 5 | [`8dc53a2f855a`](4004fb8534a1ce9d6ae1.json) | 2026-10-13 |

## Tools at `https://mcp.alphacreek.ai/mcp`

- `get_filing_toc`: `Return the full filing table of contents for one filing. If artifact_document_id is omitted, resolves the single latest filing for ticker/c…`
- `get_latest_filing`: `Return latest filing metadata for a company or ticker. If ticker and company are omitted, return newly ingested filings newest-first. Omit…`
- `list_filings`: `List available filings for a ticker (newest first) with artifact_document_id and dates. Use filing_registry=fca_nsm for UK FCA NSM reports.…`
- `read_node_content`: `Return content for one or more navigation nodes in a filing. Pass one node via node_id or several via node_ids, using the node ids from TOC…`
- `search_sec_event_filings`: `Search US SEC filing nodes for a disclosure claim. The search covers 8-K, 6-K, 10-K, 10-Q, and 20-F. Omit document_type to search all of th…`

## Changes

- 2026-10-13: [description changed, schema changed](../../deltas/2026-10-13/4004fb8534a1ce9d6ae1.json): `26 field(s) changed`
- 2026-10-02: [annotation changed, description changed, schema changed](../../deltas/2026-10-02/4004fb8534a1ce9d6ae1.json): `7 field(s) changed`
- 2026-09-26: [description changed, schema changed](../../deltas/2026-09-26/4004fb8534a1ce9d6ae1.json): `22 field(s) changed`
- 2026-09-03: [description changed, schema changed](../../deltas/2026-09-03/4004fb8534a1ce9d6ae1.json): `4 field(s) changed; signals: length_more_than_doubled`
- 2026-08-30: [description changed, schema changed](../../deltas/2026-08-30/4004fb8534a1ce9d6ae1.json): `58 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.alphacreek.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
