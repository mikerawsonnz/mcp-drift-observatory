# app.myriade.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/app.myriade.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://app.myriade.ai/mcp` | 18 | [`cfd67f1ff99e`](3608fd764f29a713c1d7.json) | 2026-08-26 |

## Tools at `https://app.myriade.ai/mcp`

- `myriade_ask`: `Ask a natural language question about a database using Myriade's data analyst agent. The agent will explore the database schema, search the…`
- `myriade_get_check`: `Get a monitoring check (name, SQL, severity, cadence, status) and its most recent run results, newest first. On governed databases the SQL…`
- `myriade_get_database_info`: `Get detailed information about a specific database connection. Returns information about the database including its name, engine type, desc…`
- `myriade_get_query_results`: `Re-execute a saved Myriade query and return fresh results. The query's SQL always re-runs under the caller's governance policies (table per…`
- `myriade_get_table_schema`: `Get the column-level schema for a specific table. Returns column names, data types, and descriptions for the table. Raises if the user has…`
- `myriade_list_databases`: `List databases configured in Myriade (paginated, sorted by name). Returns paginated database connections with their IDs, names, engines, an…`
- `myriade_list_reports`: `List or search reports (documents) written in Myriade. Without ''query'' returns the most recently updated reports first; with ''query'' re…`
- `myriade_list_tables`: `List tables in a database (paginated, sorted by database/schema/name). Returns a flat, paginated list of tables. Each item has database_nam…`
- `myriade_monitoring_overview`: `Snapshot of a database's monitoring board: check count, standing alerts (open / acknowledged / known) with their headlines, recent notifica…`
- `myriade_propose_check`: `Propose a monitoring check for the user to review in Myriade. This creates a PROPOSAL, never an active check: nothing runs until a database…`
- `myriade_query`: `Execute a read-only SQL query against a database. Write operations (INSERT, UPDATE, DELETE, DROP, etc.) are blocked. Returns up to 50 rows…`
- `myriade_read_asset`: `Get detailed information about a catalog object (table, column, schema, or glossary term — assets and terms share one id space). Returns th…`
- `myriade_read_report`: `Read a report's full markdown content. Applies the same visibility rule as the web app; a report the caller may not see returns a "not foun…`
- `myriade_request_catalog_change`: `Propose a catalog change for the data team to review (no edit rights needed). Creates a reviewable suggestion routed to the asset's reviewe…`
- `myriade_sample_data`: `Get sample rows from a table to understand the data. Returns a random sample of up to ''limit'' rows (max 20).`
- `myriade_search_catalog`: `Search the data catalog for tables, columns, or terms by name/description. Uses fuzzy matching and full-text search. Keep queries short (1-…`
- `myriade_triage_alert`: `Triage an alert (requires manage access: database owner or org admin). - ''resolve'': the underlying problem is handled or gone. - ''acknow…`
- `myriade_update_asset`: `Update a catalog asset's documentation (requires edit rights). - ''description'' replaces the existing description (auto-sets status to "dr…`

## Changes

- 2026-08-26: [count changed, description changed, tool added](../../deltas/2026-08-26/3608fd764f29a713c1d7.json): `6 tool(s) added; 1 field(s) changed`
- 2026-08-25: [description changed](../../deltas/2026-08-25/3608fd764f29a713c1d7.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://app.myriade.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
