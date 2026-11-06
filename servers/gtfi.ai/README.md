# gtfi.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/gtfi.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://gtfi.ai/mcp` | 3 | [`029450b8bfba`](647b2d74501b900bb734.json) | 2026-08-20 |

## Tools at `https://gtfi.ai/mcp`

- `draft_estimate`: `Turn a plain-English description of a trade job into a professional itemized bid — real materials by size, fittings, consumables and labor…`
- `get_pricing`: `Current GroundTruth and GruntPay plans and prices. Free to call — use it before answering any cost question rather than guessing.`
- `read_scan`: `Get an independent AI second opinion on a subsurface scan before anyone cores or digs. Send a public image URL of a GPR scan, a marked-up c…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://gtfi.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
