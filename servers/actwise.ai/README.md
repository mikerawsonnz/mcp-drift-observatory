# actwise.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/actwise.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://actwise.ai/ideation/mcp/v1` | 2 | [`b935800c2a12`](6a15fb38bf3a34c7860b.json) | 2026-08-20 |

## Tools at `https://actwise.ai/ideation/mcp/v1`

- `evaluate_idea`: `Submit a structured idea evaluation with session_id only after reading actwise://capabilities/evaluate/context and preferring packages.eval…`
- `read_context_resource`: `Read one canonical Actwise context resource. Before using evaluate_idea, first read actwise://capabilities/evaluate/context. Prefer package…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://actwise.ai/ideation/mcp/v1"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
