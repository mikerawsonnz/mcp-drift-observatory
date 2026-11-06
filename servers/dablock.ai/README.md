# dablock.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/dablock.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://dablock.ai/mcp` | 5 | [`aed3f86a3cd3`](f85983e7a590329700e5.json) | 2026-08-20 |

## Tools at `https://dablock.ai/mcp`

- `get_brand_visibility`: `One brand's standing in the current DABLOCK release: share of answer per engine, rank, quadrant, how many panel prompts name it, and which…`
- `get_history`: `Every DABLOCK release ever published, as a series per brand: share of answer at each weekly measurement with the date and panel version it…`
- `get_methodology`: `The rules behind every figure this server returns: the exact prompt panel and its version, which engines were measured, how share of answer…`
- `get_visibility_index`: `The whole current release in one call: every tracked brand in crypto/Web3 with its rank, share of answer overall and per engine, commercial…`
- `list_tracked_brands`: `The names and slugs of every brand in the DABLOCK index — a lookup table, nothing else. No scores, no ranks. Use it for two things: to turn…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://dablock.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
