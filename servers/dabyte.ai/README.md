# dabyte.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/dabyte.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://dabyte.ai/mcp` | 5 | [`c1e17d652f68`](8f7f7570927c48d5e3d6.json) | 2026-08-20 |

## Tools at `https://dabyte.ai/mcp`

- `get_brand_visibility`: `One brand's standing in the current DABYTE release: share of answer per engine, rank, quadrant, how many panel prompts name it, and which o…`
- `get_history`: `Every DABYTE release ever published, as a series per brand: share of answer at each weekly measurement with the date and panel version it w…`
- `get_methodology`: `The rules behind every figure this server returns: the exact prompt panel and its version, which engines were measured, how share of answer…`
- `get_visibility_index`: `The whole current release in one call: every tracked brand in SaaS & AI tools with its rank, share of answer overall and per engine, commer…`
- `list_tracked_brands`: `The names and slugs of every brand in the DABYTE index — a lookup table, nothing else. No scores, no ranks. Use it for two things: to turn…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://dabyte.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
