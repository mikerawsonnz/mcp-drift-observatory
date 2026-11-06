# nothumansearch.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/nothumansearch.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://nothumansearch.ai/mcp` | 14 | [`250965414225`](04d603fa9e65c862e569.json) | 2026-08-20 |

## Tools at `https://nothumansearch.ai/mcp`

- `check_url`: `On-demand agentic-readiness check for any URL. Runs the NHS 7-signal crawler live (llms.txt, ai-plugin.json, OpenAPI, structured API, MCP s…`
- `find_mcp_servers`: `List sites in the index that expose a live MCP server, ranked by agentic readiness. The result set carries a query-free discovery receipt a…`
- `get_site_details`: `Get the full agentic readiness report for a specific domain: score, category, all 7 signal checks (llms.txt, ai-plugin.json, OpenAPI, struc…`
- `get_stats`: `Current Not Human Search index stats: total sites, average agentic score, top category, sites added in the last 7 days, count of sites expo…`
- `get_top_sites`: `Get the highest-scored agent-ready sites in the index, optionally filtered by category. Organic order is always readiness-score order. A su…`
- `handoff_provider_action`: `Present the exact ticket bearer returned by prepare_provider_action. NHS records one privacy-safe handoff receipt, then returns the attribu…`
- `list_categories`: `List all categories in the Not Human Search index with site counts and average agentic scores. Use this to understand what kinds of agent-r…`
- `prepare_provider_action`: `Prepare a signed action ticket for a separately disclosed provider-funded offer returned beside a receipt-bearing NHS discovery result. Thi…`
- `recent_additions`: `List agent-ready sites newly added to the Not Human Search index, sorted newest first. A supported category creates a query-free discovery…`
- `record_action_interest`: `Record the caller's attestation that its human or company principal currently wants one controlled next step with a site returned organical…`
- `register_monitor`: `Register an email to get alerted when the indicated domain's agentic readiness score drops. Useful for agents tracking a dependency's agent…`
- `search_agents`: `Search for websites, APIs, and services that AI agents can actually use. Results are ranked by agentic readiness score (0-100) based on llm…`
- `submit_site`: `Submit a URL for NHS to crawl and score. Use when you discover an agent-first tool, API, or service that isn't in the index yet. NHS will f…`
- `verify_mcp`: `Actively probe any URL to check if it is a live, spec-compliant MCP server. Sends a JSON-RPC tools/list request and verifies a valid respon…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://nothumansearch.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
