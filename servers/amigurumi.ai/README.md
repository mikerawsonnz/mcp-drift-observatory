# amigurumi.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/amigurumi.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://amigurumi.ai/mcp` | 3 | [`6b02235325be`](d1c2489bf9c91392e3dd.json) | 2026-11-16 |

## Tools at `https://amigurumi.ai/mcp`

- `circle_calculator`: `Work out the rounds for an amigurumi circle, ball or tube of a given size: sc in a spiral from a magic ring, staggered increases and decrea…`
- `get_toy`: `Show one amigurumi pattern from amigurumi.ai: picture, size, difficulty, hook, yarn weight and colours with metres, and links to the full p…`
- `search_toys`: `Search the free amigurumi (crochet toy) patterns on amigurumi.ai. Every pattern has a 3D model and exact round-by-round instructions. Use i…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://amigurumi.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
