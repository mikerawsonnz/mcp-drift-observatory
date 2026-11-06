# calaf.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/calaf.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://calaf.ai/api/mcp` | 2 | [`2fa0980ebc78`](b821d163c47f060eeac8.json) | 2026-09-27 |

## Tools at `https://calaf.ai/api/mcp`

- `get_seed_format`: `Returns the complete specification (markdown) for calaf_seed: 1 JSON documents — the format to follow when a user asks for a Calaf seed. Re…`
- `validate_seed`: `Runs a draft seed document through the exact parser the Calaf app imports with. Pass the entire JSON document as a string. Returns per-sect…`

## Changes

- 2026-09-27: [schema changed](../../deltas/2026-09-27/b821d163c47f060eeac8.json): `7 field(s) changed; signals: url_introduced`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://calaf.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
