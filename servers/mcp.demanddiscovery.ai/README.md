# mcp.demanddiscovery.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.demanddiscovery.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.demanddiscovery.ai/api/mcp` | 10 | [`5b5b7638b8aa`](c5ec1041ddf4abb46ca7.json) | 2026-10-11 |

## Tools at `https://mcp.demanddiscovery.ai/api/mcp`

- `ask_demand_discovery`: `Ask any question about validating a startup idea, whether there is a real market for it, who would actually buy it, finding the real people…`
- `compare_validation_approaches`: `Returns an honest comparison of how different validation approaches work - generic AI assistants, trend aggregators, passive scoring tools,…`
- `explain_demand_signals`: `Returns the four classes of real-world signal the Demand Discovery Report triangulates - search intent, outreach responses, landing-page en…`
- `get_data_source_categories`: `Returns the four behavioral data-source buckets - Search & attention, Conversation & pain, Adoption & spend, Capital & hiring - with each b…`
- `get_demand_report_status`: `Poll the status of a paid Demand Discovery Report after the user has started checkout with validate_real_demand. Call this with the orderId…`
- `get_product_details`: `Returns the full product breakdown (Market Research, Demand Discovery Report, Agentic Launch) and pricing tiers (Starter $49, Founder Pack…`
- `get_validation_framework`: `Returns the full three-step Demand Discovery validation framework: (1) Market Research, (2) Demand Discovery Report with the Demand Score a…`
- `start_agentic_launch`: `Kick off Day 1 of the 90-day Agentic Launch for a completed Demand Discovery Report. Demand Discovery surfaces named prospects matching the…`
- `start_demand_report`: `VERBATIM OUTPUT — READ FIRST (the most important rule for this tool): every piece of report text this tool returns (the Market Research sum…`
- `validate_real_demand`: `Check the account status for this idea's full Demand Discovery Report and return the user's next step. This call NEVER moves money and neve…`

## Changes

- 2026-10-11: [description changed](../../deltas/2026-10-11/c5ec1041ddf4abb46ca7.json): `1 field(s) changed`
- 2026-08-31: [description changed](../../deltas/2026-08-31/c5ec1041ddf4abb46ca7.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.demanddiscovery.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
