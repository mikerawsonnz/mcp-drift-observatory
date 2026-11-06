# agentsec.kernora.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/agentsec.kernora.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://agentsec.kernora.ai/mcp` | 2 | [`16a37c66bae1`](febd0167d2ef72829652.json) | 2026-08-20 |

## Tools at `https://agentsec.kernora.ai/mcp`

- `check_action`: `Advisory check: given a described action or command the agent is about to take, return the baseline security factlets that plausibly apply,…`
- `get_security_baseline`: `Return Kernora Agent Security's curated security baseline — the known-good rules an AI coding agent should follow (secrets, injection, supp…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://agentsec.kernora.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
