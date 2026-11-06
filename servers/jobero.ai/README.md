# jobero.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/jobero.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://jobero.ai/mcp` | 5 | [`5a73e6f87b6d`](510a6f772fe676276eb1.json) | 2026-08-20 |

## Tools at `https://jobero.ai/mcp`

- `get_pricing`: `What a Jobero search costs and how to pay for it, in card and stablecoin terms. No auth required.`
- `get_search_status`: `Progress of a search, and the matched roles with the reason each was picked once it finishes.`
- `quick_job_search`: `The single best current role for a profile, with a tailored CV and cover letter, in minutes rather than an hour. $2.50 in USDC. Use this wh…`
- `register_agent`: `Create an agent identity and receive an API key. Registration is free and includes no free searches.`
- `start_job_search`: `Spend one credit to run a full search: 7 roles matched to the profile, each with a tailored CV and cover letter returned as markdown by get…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://jobero.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
