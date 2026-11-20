# www.arcreport.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/www.arcreport.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://www.arcreport.ai/api/ask` | 7 | [`1ff3119ed1c1`](5990de195db11012fcfb.json) | 2026-11-20 |
| `https://www.arcreport.ai/api/mcp` | 19 | [`d77cc168ce66`](5b7f6412bf3c3e91b70c.json) | 2026-11-17 |

## Tools at `https://www.arcreport.ai/api/ask`

- `before_checkout`: `Call this right before your agent tries to check out at a store, or when a user asks "can my agent check out at <store>?". Not for an attem…`
- `compare`: `Call this when a user names 2 or more stores for the same item and asks which one to use, or when you must choose between a few stores and…`
- `find_stores`: `Call this when you need to pick a store for a product need and want one where a saved check shows an agent reached checkout. Filters: categ…`
- `guide`: `Call this when a person at a store (a CEO, a marketing or e-commerce manager, or a developer) asks where their store is on the journey to A…`
- `report_outcome`: `Call this right after your agent tried to check out at a store, to log, record or report what happened: it reached checkout, a captcha stop…`
- `store_record`: `Call this when a user asks what ARC recorded for a store, or you need the citable store page. Returns the store page's verdict, checked_at…`
- `why_blocked_and_fix`: `Call this after before_checkout says reaches_checkout is false or null, or when an agent got stuck at a store and you want the reason and t…`

## Tools at `https://www.arcreport.ai/api/mcp`

- `ask_agents_about_brand`: `[Requires sign-in] Ask benchmark personal-agent personas what they think of a brand and whether they would recommend it for a category. Per…`
- `bulk_create_monitors`: `[Requires sign-in] Set up scheduled monitoring for one or more store URLs (the 'set up monitoring' flow). Validates each URL and rejects in…`
- `can_agent_checkout`: `[Requires sign-in] Call when you need a saved checkout-link check for any public store URL, not only Index brands. Use it for 'what stops a…`
- `check_agent_readiness`: `[Requires sign-in] Check whether personal AI agents can reach a product URL, understand it, and reach checkout. Runs ARC's readiness check:…`
- `check_store`: `Check if an AI agent can reach checkout on a store before trying. Call this with a store domain, such as allbirds.com. Returns the saved ch…`
- `find_stores`: `Find stores where a saved check shows an AI agent can reach checkout. Filter by platform, protocol, category, or min_grade (optional, defau…`
- `get_fixes`: `[Requires sign-in] Concrete next steps to get recommended by personal agents and to become reachable, understandable, and buyable. Pass a r…`
- `get_readiness_result`: `[Requires sign-in] Get a readiness check by id. While running, reports progress. When complete, reports whether personal agents could reach…`
- `get_store_hub`: `[Requires sign-in] Look up a free ARC store card by host. Includes saved measurements and brand_claim ownership metadata. Brand statements…`
- `google_checkout_readiness`: `[Requires sign-in] Read saved public Google agentic checkout readiness checks for a store. Free; no new scan or paid calls. Merchant Center…`
- `list_monitors`: `[Requires sign-in] List the workspace's monitors — each store re-checked on a schedule for whether personal agents can still reach it and i…`
- `list_readiness_checks`: `[Requires sign-in] List this workspace's recent readiness checks (newest first) — each store, its score, status, and id. Use an id with get…`
- `monitor_summary`: `[Requires sign-in] Overview of whether monitored stores are still buyable by personal agents: latest score, trend, status, next run, and re…`
- `pause_monitor`: `[Requires sign-in] Pause a monitor so it stops running on schedule (its history is kept). Use the monitor id from list_monitors.`
- `product_data_check`: `Free latest saved product data and return/shipping policy check from the store's pages and structured data. Reads history only; no store fe…`
- `report_checkout`: `Report how far one agent got at one store. Free, no login. Omit contributor_key and ARC issues one. Emails, phones, street addresses, card…`
- `resume_monitor`: `[Requires sign-in] Resume a paused monitor.`
- `run_monitor_now`: `[Requires sign-in] Run a monitor's scan immediately (off-schedule) to establish or refresh its baseline. Runs one scan — only call when the…`
- `update_monitor`: `[Requires sign-in] Change a monitor's cadence (daily/weekly/monthly) or label. Use the monitor id from list_monitors.`

## Changes

- 2026-11-20: [description changed](../../deltas/2026-11-20/5990de195db11012fcfb.json): `2 field(s) changed`
- 2026-11-19: [description changed, schema changed](../../deltas/2026-11-19/5990de195db11012fcfb.json): `6 field(s) changed`
- 2026-11-17: [schema changed](../../deltas/2026-11-17/5b7f6412bf3c3e91b70c.json): `6 field(s) changed; signals: length_more_than_doubled`
- 2026-11-17: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-17/5990de195db11012fcfb.json): `1 tool(s) added; 10 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-11-16: [description changed, schema changed](../../deltas/2026-11-16/5b7f6412bf3c3e91b70c.json): `6 field(s) changed`
- 2026-11-16: [count changed, description changed, schema changed, tool removed](../../deltas/2026-11-16/5990de195db11012fcfb.json): `19 tool(s) removed; 7 field(s) changed`
- 2026-11-07: [description changed, schema changed](../../deltas/2026-11-07/5b7f6412bf3c3e91b70c.json): `9 field(s) changed; signals: length_more_than_doubled`
- 2026-11-07: [annotation changed, count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-11-07/5990de195db11012fcfb.json): `7 tool(s) added; 53 field(s) changed; signals: url_introduced`
- 2026-11-06: [description changed](../../deltas/2026-11-06/5990de195db11012fcfb.json): `2 field(s) changed; signals: url_introduced`
- 2026-11-06: [description changed](../../deltas/2026-11-06/5b7f6412bf3c3e91b70c.json): `1 field(s) changed`
- 2026-11-03: [count changed, description changed, tool added](../../deltas/2026-11-03/5990de195db11012fcfb.json): `1 tool(s) added; 1 field(s) changed`
- 2026-11-02: [description changed](../../deltas/2026-11-02/5b7f6412bf3c3e91b70c.json): `1 field(s) changed`
- 2026-11-02: [count changed, description changed, tool added](../../deltas/2026-11-02/5990de195db11012fcfb.json): `1 tool(s) added; 4 field(s) changed`
- 2026-10-17: [description changed](../../deltas/2026-10-17/5b7f6412bf3c3e91b70c.json): `4 field(s) changed`
- 2026-10-17: [description changed](../../deltas/2026-10-17/5990de195db11012fcfb.json): `1 field(s) changed`
- 2026-10-16: [description changed](../../deltas/2026-10-16/5990de195db11012fcfb.json): `2 field(s) changed`
- 2026-10-15: [description changed](../../deltas/2026-10-15/5b7f6412bf3c3e91b70c.json): `4 field(s) changed`
- 2026-10-15: [count changed, description changed, tool added](../../deltas/2026-10-15/5990de195db11012fcfb.json): `1 tool(s) added; 4 field(s) changed`
- 2026-10-14: [annotation changed, description changed](../../deltas/2026-10-14/5b7f6412bf3c3e91b70c.json): `32 field(s) changed; signals: length_more_than_doubled`
- 2026-10-14: [schema changed](../../deltas/2026-10-14/5990de195db11012fcfb.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://www.arcreport.ai/api/ask"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
