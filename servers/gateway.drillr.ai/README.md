# gateway.drillr.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/gateway.drillr.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://gateway.drillr.ai/mcp/data` | 10 | [`712041b5d81c`](8ad0cc12a0c57c027292.json) | 2026-09-16 |

## Tools at `https://gateway.drillr.ai/mcp/data`

- `ai_adoption`: `Search concrete enterprise AI applications disclosed in US company earnings calls. Filter by ticker, partially match a company name, search…`
- `company_search`: `Use for qualitative company discovery (industry, business model, supply chain, competitors, management background). For numerical screening…`
- `filing_list`: `Use to discover which SEC filings exist for a ticker before searching content. For the actual content use filing_search instead. List index…`
- `filing_search`: `Search one company's SEC filings. Returns '## Facts' (exact as-reported and restated financial values) and '## Passages' (matching filing t…`
- `get_table_schema`: `Column definitions (name, type, description) for a data table, plus its usage note where one exists: required filters, ticker format, and m…`
- `industry_inflections`: `Search industry inflections identified through structured research of earnings calls held by US-listed companies, including the change mech…`
- `list_tables`: `List alternative-data tables under the given categories. Returns each table's name, one-line purpose, and column names (call get_table_sche…`
- `news_search`: `Use for any news, event, development, or statement question about a company, theme, or the market. The 'ticker' filter takes exchange-suffi…`
- `run_sql`: `PostgreSQL SELECT over financial / market / alt-data tables — returns structured rows. Hard rules (query fails otherwise): - SELECT only, n…`
- `ticker_lookup`: `Resolve a company name, brand, or ticker substring to canonical ticker(s). Input: - query (required): company name, brand, or ticker substr…`

## Changes

- 2026-09-16: [description changed, schema changed](../../deltas/2026-09-16/8ad0cc12a0c57c027292.json): `9 field(s) changed`
- 2026-09-05: [count changed, description changed, schema changed, tool added, tool removed](../../deltas/2026-09-05/8ad0cc12a0c57c027292.json): `4 tool(s) added; 2 tool(s) removed; 3 field(s) changed; signals: imperative_language_introduced` **(notable)**
- 2026-08-27: [count changed, tool removed](../../deltas/2026-08-27/8ad0cc12a0c57c027292.json): `1 tool(s) removed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://gateway.drillr.ai/mcp/data"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
