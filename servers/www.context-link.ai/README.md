# www.context-link.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/www.context-link.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://www.context-link.ai/mcp` | 4 | [`2c0bea3928fb`](de4fcccd39d75091e9b1.json) | 2026-09-13 |

## Tools at `https://www.context-link.ai/mcp`

- `ask_question`: `Ask a question about the user's connected workspaces and websites and receive a concise answer with citations. The attached widget displays…`
- `get_context`: `Get context from the user's connected workspaces and websites. The attached widget displays only the list of sources consulted — it does no…`
- `get_memory`: `Retrieve previously saved memory content by its namespace. Use this when the user wants to recall saved content.`
- `save_memory`: `Save content to the user's memory for later retrieval. Use this when the user wants to save information, notes, or conversation content.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://www.context-link.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
