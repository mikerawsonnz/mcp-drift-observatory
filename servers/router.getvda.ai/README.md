# router.getvda.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/router.getvda.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://router.getvda.ai/mcp` | 2 | [`29e5b8c3632f`](37bb5bfc5fb80d7ae462.json) | 2026-08-20 |

## Tools at `https://router.getvda.ai/mcp`

- `invoke`: `Single entry point for the GOSCE portfolio: routes orchestrators to verified agents by capability, with real example output from the router…`
- `selftest`: `FREE, no payment required. Runs this agent's real capability on a fixed canned input and returns the genuine result, an honest assertion gr…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://router.getvda.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
