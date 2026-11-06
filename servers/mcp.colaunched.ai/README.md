# mcp.colaunched.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.colaunched.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.colaunched.ai/public` | 4 | [`091ba900da94`](84559fa5fcdd0c54db93.json) | 2026-09-27 |

## Tools at `https://mcp.colaunched.ai/public`

- `get_idea`: `One published idea as its public page shows it: the need, one way to build it, the four score parts and why, how we know (dated evidence, w…`
- `latest_ideas`: `The newest business ideas Colaunched has published from public demand, with each one's public score (0–100) and category. No account needed…`
- `list_categories`: `The categories ideas are filed under.`
- `search_ideas`: `Find published ideas by words in the title or one-liner. No account needed.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.colaunched.ai/public"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
