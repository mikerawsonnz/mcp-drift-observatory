# api.dryos.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.dryos.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.dryos.ai/mcp` | 5 | [`53afa16dafbc`](a5525620dd94487c3ad2.json) | 2026-09-18 |

## Tools at `https://api.dryos.ai/mcp`

- `column_values`: `The distinct values of one text column, most rows first — what a filter can be. Args: slug: The stream. column: A text column from describe…`
- `describe_stream`: `One stream in full: every column, the primary key, the source and its health. Also what changed in the collector recently — a change in the…`
- `find_entities`: `Look up the nodes, zones, stations or fuels in a stream, with how far back each goes. Use it before query_stream: names are verbatim and ne…`
- `list_streams`: `Every stream Dryos collects, with its entity column and headline measure. Args: domain: Energy, Weather or Property. operator: A grid opera…`
- `query_stream`: `Read rows from a stream — raw (newest first), each entity's newest, or a rollup. The result carries 'restUrl': this same request as a plain…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.dryos.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
