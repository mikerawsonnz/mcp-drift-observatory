# llmintel.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/llmintel.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://llmintel.ai/v1/mcp` | 5 | [`4750ec90c571`](2c301e604b7175d1bd54.json) | 2026-08-20 |

## Tools at `https://llmintel.ai/v1/mcp`

- `check_model`: `Check whether an LLM model id is safe to use, deprecated, or retired, and what to migrate to. Accepts the exact string used in code (e.g. '…`
- `list_retiring_models`: `List tracked models scheduled to retire within a time window, soonest first. Use this to audit a codebase or plan migration work.`
- `recent_lifecycle_changes`: `Lifecycle state changes across all tracked providers, newest first. Use this to answer 'what model deprecations happened recently?'.`
- `search_models`: `List tracked models, optionally filtered by provider and lifecycle state. Use this to discover what is currently available from a provider.`
- `suggest_replacement`: `Given a deprecated or retiring model, return the provider's recommended replacement(s) and, when none is published, active models from the…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://llmintel.ai/v1/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
