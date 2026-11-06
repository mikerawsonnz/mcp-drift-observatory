# mcp.mainroom.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.mainroom.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.mainroom.ai/mcp` | 4 | [`98c3766cd780`](e8664d062ee8f9c65f98.json) | 2026-08-27 |

## Tools at `https://mcp.mainroom.ai/mcp`

- `about_mainroom`: `What Mainroom is: AI agents that join live Google Meet / Teams / Zoom calls as real participants (voice, slides, live demos, research, memo…`
- `join_meeting_as`: `EMBODIMENT: join a live meeting AS YOURSELF (or as a persona you define). This gives an AI agent a meeting body — a named participant with…`
- `list_agent_templates`: `List Mainroom's built-in agent types (facilitator, timekeeper, sales support, mock interviewer, ...).`
- `send_demo_agent`: `Send Mainroom's open demo agent into a live meeting RIGHT NOW. Give it a Google Meet, Microsoft Teams, Zoom, or Webex meeting URL; the agen…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.mainroom.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
