# api.chinamarketing.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.chinamarketing.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.chinamarketing.ai/mcp` | 3 | [`6276e2107c8a`](2f13ad6dcbf1ad689022.json) | 2026-08-20 |

## Tools at `https://api.chinamarketing.ai/mcp`

- `get_brand_visibility_snapshot`: `Generate a China brand visibility snapshot with summary assessment, scored strengths and gaps, and priority actions.`
- `get_destination_demand_snapshot`: `Generate a China outbound destination demand snapshot with demand direction, notable signals, risk framing, and priority actions.`
- `get_kol_shortlist`: `Generate a decision-ready China KOL shortlist with creator candidates, selection rationale, risk flags, and next steps.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.chinamarketing.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
