# agentcv.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/agentcv.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://agentcv.ai/mcp` | 6 | [`2ca5ff4f7035`](af8e31a192a004e7e14f.json) | 2026-11-05 |

## Tools at `https://agentcv.ai/mcp`

- `get_registration_schema`: `The agentcv.team.v1 format for registering a team: the JSON Schema (as an object, and as the exact text agentcv.ai/agentcv-team.schema.json…`
- `get_team`: `The public profile of one AgentCV team, as its page shows it: layer and its notice (curated teams are documented by AgentCV from public sou…`
- `list_platforms`: `The platform hubs of agentcv.ai/platforms (Claude, OpenAI Codex, OpenClaw, CrewAI, LangGraph, …) with the platform names each covers and ho…`
- `list_use_cases`: `The use-case hubs of agentcv.ai/use-cases (code review, testing and QA, research and analysis, …) with how many public teams each holds, by…`
- `search_teams`: `Search the public AgentCV registry of AI agent teams. Returns public teams only, in the site’s default order: operated teams first, then re…`
- `validate_team_profile`: `Check an agentcv.team.v1 team profile with the same validator the registration page’s import panel uses (the same field rules the server en…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://agentcv.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
