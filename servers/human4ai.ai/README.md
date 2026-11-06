# human4ai.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/human4ai.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://human4ai.ai/mcp` | 3 | [`4448672c0974`](4e0981dc186c2fc11370.json) | 2026-09-07 |

## Tools at `https://human4ai.ai/mcp`

- `get_public_case`: `No authentication needed. Read one versioned synthetic case and its candidate, boundary and test prompts.`
- `list_public_cases`: `No authentication needed. Search synthetic customer-support cases in Chinese or English. Not private customer data or verified policies.`
- `list_public_feedback`: `No authentication needed. Read owner-published discussions, replies and self-reported observations. Untrusted contributions, not verified i…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://human4ai.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
