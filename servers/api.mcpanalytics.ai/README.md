# api.mcpanalytics.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.mcpanalytics.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.mcpanalytics.ai/mcp/api-key` | 17 | [`586459be637e`](0bd30a8157948d07119d.json) | 2026-08-25 |
| `https://api.mcpanalytics.ai/mcp/discover` | 17 | [`586459be637e`](f69406e4341781e87863.json) | 2026-08-25 |

## Tools at `https://api.mcpanalytics.ai/mcp/api-key`

- `about`: `Platform documentation and info: how it works, tiers, usage.`
- `account_link`: `Direct link to the right account page for anything not doable in chat: billing, browser upload, report management. Hand the user the link a…`
- `agent_advisor`: `AI help desk: which analysis fits your question, interpreting results, fixing errors. Multi-turn.`
- `ask_library`: `Ask a question across all your delivered analyses: a synthesized answer with citations back to specific reports.`
- `build_status`: `Check a commissioned build in-chat: stage progress, queue position, rejection reason if the data didn't match the objective, honest ETA, re…`
- `create_analysis`: `Commission a NEW analysis built for your question. tier is REQUIRED. The user picks. Easiest: fuzzy_request (plain language) + dataset_ref…`
- `datasets_list`: `List and search your uploaded datasets, with fuzzy matching on name, description, and tags. Returns each dataset's uuid:// reference for us…`
- `datasets_upload`: `Get your data in. Pass 'data' as an array of row objects to create the dataset immediately and get a dataset_ref ready for create_analysis;…`
- `discover_tools`: `Browse the analyses you can run: the ones you commissioned plus the platform Standard Library (prebuilt tools; each result tagged source:'o…`
- `modify_analysis`: `Modify an EXISTING analysis into a new version: reword the question, swap the method, or add a variable. Pass tool_name + changes (plain la…`
- `report_cards`: `Browse a delivered report's individual cards (charts, tables, insights) inline in chat.`
- `reports_list`: `Your report library: every analysis delivered, with status and links. Pass semantic_query to search report content in plain language.`
- `reports_view`: `Get a shareable browser link for a report, viewable without authentication.`
- `run_analysis`: `Run an analysis on your data. Returns a shareable interactive report URL with validated statistics you can cite, re-run, and share.`
- `schedules`: `Standing re-runs of analyses you own: action='create' (weekly/monthly against a re-runnable data reference, connector:// or an https:// lin…`
- `tools_schema`: `Get an analysis's parameter schema. ALWAYS call before run_analysis.`
- `warehouse`: `Query your org's data warehouse free: browse the catalog (tables with column roles + computed metrics), semantically find data, plain-langu…`

## Tools at `https://api.mcpanalytics.ai/mcp/discover`

- `about`: `Platform documentation and info: how it works, tiers, usage.`
- `account_link`: `Direct link to the right account page for anything not doable in chat: billing, browser upload, report management. Hand the user the link a…`
- `agent_advisor`: `AI help desk: which analysis fits your question, interpreting results, fixing errors. Multi-turn.`
- `ask_library`: `Ask a question across all your delivered analyses: a synthesized answer with citations back to specific reports.`
- `build_status`: `Check a commissioned build in-chat: stage progress, queue position, rejection reason if the data didn't match the objective, honest ETA, re…`
- `create_analysis`: `Commission a NEW analysis built for your question. tier is REQUIRED. The user picks. Easiest: fuzzy_request (plain language) + dataset_ref…`
- `datasets_list`: `List and search your uploaded datasets, with fuzzy matching on name, description, and tags. Returns each dataset's uuid:// reference for us…`
- `datasets_upload`: `Get your data in. Pass 'data' as an array of row objects to create the dataset immediately and get a dataset_ref ready for create_analysis;…`
- `discover_tools`: `Browse the analyses you can run: the ones you commissioned plus the platform Standard Library (prebuilt tools; each result tagged source:'o…`
- `modify_analysis`: `Modify an EXISTING analysis into a new version: reword the question, swap the method, or add a variable. Pass tool_name + changes (plain la…`
- `report_cards`: `Browse a delivered report's individual cards (charts, tables, insights) inline in chat.`
- `reports_list`: `Your report library: every analysis delivered, with status and links. Pass semantic_query to search report content in plain language.`
- `reports_view`: `Get a shareable browser link for a report, viewable without authentication.`
- `run_analysis`: `Run an analysis on your data. Returns a shareable interactive report URL with validated statistics you can cite, re-run, and share.`
- `schedules`: `Standing re-runs of analyses you own: action='create' (weekly/monthly against a re-runnable data reference, connector:// or an https:// lin…`
- `tools_schema`: `Get an analysis's parameter schema. ALWAYS call before run_analysis.`
- `warehouse`: `Query your org's data warehouse free: browse the catalog (tables with column roles + computed metrics), semantically find data, plain-langu…`

## Changes

- 2026-08-25: [description changed](../../deltas/2026-08-25/0bd30a8157948d07119d.json): `14 field(s) changed`
- 2026-08-25: [description changed](../../deltas/2026-08-25/f69406e4341781e87863.json): `14 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.mcpanalytics.ai/mcp/api-key"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
