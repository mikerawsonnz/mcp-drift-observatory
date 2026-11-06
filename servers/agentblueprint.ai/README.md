# agentblueprint.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/agentblueprint.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://agentblueprint.ai/mcp` | 4 | [`1696dc16ac28`](c66f724ebb6312c16f24.json) | 2026-11-05 |

## Tools at `https://agentblueprint.ai/mcp`

- `check_agent_one_page`: `Checks the structure of a one-page agent summary written from Agent Blueprint's template (https://agentblueprint.ai/agent-one-page-template…`
- `estimate_agent_cost`: `Estimates the tokens and dollar cost of an AI agent task from the measured benchmark job closest to it. For jobs where cost grows with how…`
- `list_benchmark_jobs`: `Lists the ten everyday jobs in Agent Blueprint's measured agent cost benchmark (2 November 2026): what each job was, how big its input was,…`
- `render_agent_map`: `Turns an agent's own inventory of its connections into Agent Blueprint's one-page access map: a single offline HTML page showing what the a…`

## Changes

- 2026-11-05: [description changed](../../deltas/2026-11-05/c66f724ebb6312c16f24.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://agentblueprint.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
