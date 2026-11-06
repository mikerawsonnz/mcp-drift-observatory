# mcp.exa.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.exa.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.exa.ai/mcp` | 2 | [`6786a32a1c87`](fbe825d2014575c816dc.json) | 2026-09-12 |

## Tools at `https://mcp.exa.ai/mcp`

- `web_fetch_exa`: `Read a webpage's full content as clean markdown. Use after web_search_exa when highlights are insufficient or to read any URL. Best for: Ex…`
- `web_search_exa`: `Search the web for any topic and get clean, ready-to-use content. Best for: Finding current information, news, facts, people, companies, or…`

## Changes

- 2026-09-12: [schema changed](../../deltas/2026-09-12/fbe825d2014575c816dc.json): `5 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.exa.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
