# grep.boolsai.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/grep.boolsai.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://grep.boolsai.ai/mcp` | 4 | [`544aa0c9f319`](d4797a61e0d00ddc4efd.json) | 2026-08-20 |

## Tools at `https://grep.boolsai.ai/mcp`

- `count_pattern`: `Same as grep_pattern but returns only the count of matching sites. Faster — no per-match serialization. Useful for sizing 'how many sites u…`
- `grep_pattern`: `Run a JavaScript regex across every scan we've ever taken. Returns matching site URLs (and optional snippets). Best for ad-hoc discovery of…`
- `list_signal_types`: `Returns the full catalog of signal_types currently present in id_index, with counts of unique values and unique domains for each.`
- `sites_with_signal`: `Return sites that have a known signal_type=signal_value pair in id_index. MUCH faster than grep_pattern — uses pre-indexed D1 lookup. Use t…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://grep.boolsai.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
