# mcpjunction.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcpjunction.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcpjunction.ai/mcp` | 5 | [`b10ef210a8fb`](a7aa59d66a026f38fb27.json) | 2026-08-30 |

## Tools at `https://mcpjunction.ai/mcp`

- `get_dataset_info`: `Dataset metadata: entry counts, generation timestamp, source, and licensing terms for bulk or training use.`
- `get_server`: `Get the full directory entry for one MCP server by id ('owner--repo', e.g. 'microsoft--playwright-mcp'). Includes install hint, license, st…`
- `list_categories`: `List all directory categories with slugs, names, and active-server counts.`
- `list_topics`: `List the curated GitHub topics that have a directory page, with active-server counts. Topics are assigned by repository owners and imported…`
- `search_servers`: `Search the MCP server directory by keyword and/or filters. Keyword matches name, description, and GitHub topics. Returns active servers sor…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcpjunction.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
