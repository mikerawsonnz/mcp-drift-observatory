# data.azquo.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/data.azquo.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://data.azquo.ai/mcp` | 41 | [`783f07d1013d`](a27acba80c8350153e96.json) | 2026-10-30 |

## Tools at `https://data.azquo.ai/mcp`

- `apply_structure`: `Add parent → child relations between names. Idempotent: existing links stay; new ones are added. With createMissing=true (default) names ar…`
- `aql_write`: `Write a 2D region of values into an Azquo database using the same AQL grammar as query_aql. AQL reference: https://www.azquo.com/connect/#a…`
- `audit_cell`: `Explain where one value in a query_aql result came from: the provenance (which import, file, user or write, and when) of every stored value…`
- `copy_azquo_skills`: `Copy azquo_skills (the Azquo usage-skills database) from data.azquo.ai into the current business, so a local or offline Azquo has its own c…`
- `copy_from_library`: `Copy one database from the shared Azquo library into the current business, with its reports, import templates and uploaded file types. ASK…`
- `create_database`: `Create a new, empty Azquo database in the current business (see current_business). Use it to start a new model from scratch; to start from…`
- `create_upload_link`: `Get a link where the USER uploads documents (Word, PDF, Excel, PowerPoint, anything) to keep with a database. Use this whenever a file shou…`
- `current_business`: `Return the currently effective business and user for this MCP session, and whether an acting-as override is in effect. Use before any destr…`
- `delete_database`: `Permanently delete an Azquo database by name, with all its names, values and history. NOT REVERSIBLE - there is no restore, and its backups…`
- `delete_import_template`: `Permanently delete one import template (the workbook of rules that interprets incoming data files) and its file on disk. NOT REVERSIBLE - t…`
- `delete_name`: `Delete a name from the database. Its values are deleted with it, as are the documents and images uploaded to it with create_upload_link (th…`
- `delete_report`: `Permanently delete one online report (an Excel report users run in Azquo): its workbook file, its menu entries, its external data requests…`
- `describe_database`: `Get an overview of an Azquo database: top-level sets with child counts, available attributes, and the 'meta information' subtree (semantic…`
- `describe_query`: `Resolve a name-query expression and return the matched names with full details: parents, attributes (including AI Text bodies and any other…`
- `describe_set`: `Drill into a named set: returns its child names with child counts, plus the parent path. Use after describe_database to explore a specific…`
- `edit_name_attributes`: `Surgical attribute edit on an existing name. Each entry in the attributes map sets that attribute on the named name; an empty string value…`
- `get_report_data`: `Fetch the full data for a report, including all regions and current choice values. Reports in Azquo are Excel-based templates with named da…`
- `history_settings`: `See or change whether a database records history - value history (audit_cell), name attribute history and set membership history (name_hist…`
- `import_file`: `Import SMALL INLINE DATA into an Azquo database - a base64-encoded blob under 'fileContent'. Filename selects the import template. THIS IS…`
- `import_from_query`: `Run SQL against a configured external database connection and import the result into an Azquo database. THE SERVER CONNECTS AND FETCHES - t…`
- `import_from_url`: `Bulk-load a delimited-text or spreadsheet file into a database by URL. THE SERVER DOWNLOADS IT, so the file never passes through your conte…`
- `list_businesses`: `List the businesses this MCP session can switch between. Peers are derived from the API key owner's email — one entry per business that ema…`
- `list_database_sheets`: `List every Excel workbook associated with one database, grouped into the three kinds Azquo holds: 'reports' (online reports users run), 'se…`
- `list_databases`: `List all Azquo databases available to the current user. The shared 'azquo' business overlays two DBs onto every session: 'azquo_skills' (re…`
- `list_deleted_names`: `Names that have been deleted, most recent first, with who deleted them and when, how many children they had and which sets they were in. pa…`
- `list_documents`: `List the documents stored with a database (uploaded via create_upload_link), newest first: id, filename, size, the name they are attached t…`
- `list_external_connections`: `List the external database connections configured for this business. Use the connection NAME with import_from_query. Credentials are never…`
- `list_import_templates`: `List every import template in the current business. An import template is a workbook of rules that tells Azquo how to interpret incoming da…`
- `list_library`: `Browse the shared Azquo library of example/demo databases. Returns every catalogue entry in one call with its full description inline, so n…`
- `list_names`: `Find names in a database by text match on their display name, when you know roughly what something is called but not where it sits. Read-on…`
- `list_reports`: `List the online reports (Excel reports users run in Azquo) the current user can see, across every database in the business. Read-only, no p…`
- `list_users`: `List the user accounts of the current business (see current_business; switch_business to change it). Read-only. Use it to answer who has ac…`
- `name_history`: `History of one name: every earlier version of its attributes (who set them, who replaced them, when), each change to its membership as a se…`
- `open_in_browser`: `A link that opens a report in the person's own web browser, ALREADY SIGNED IN as them - the live report with its Save button, choosers and…`
- `persist_database`: `Flush pending writes for this database to disk. Edits via edit_name_attributes, apply_structure, AQL edit: primitives etc. are queued in-me…`
- `query_aql`: `Query an Azquo database using AQL (Azquo Query Language). AQL reference: https://www.azquo.com/connect/#aql Read-only - this never creates…`
- `read_document`: `Read a stored document (see list_documents) as Markdown - headings, lists, tables, slides and pages kept. Long documents come a page at a t…`
- `read_workbook`: `Read inside one workbook held against a database — a 'report', 'importTemplate' or 'setupSheet' (use list_database_sheets to see what exist…`
- `restore_name`: `Bring back a deleted name (ids from list_deleted_names or name_history). It returns as a NEW name with a new id, its attributes as they wer…`
- `switch_business`: `Switch the active business for subsequent MCP tool calls in this session. The switch is this MCP session's alone: other agents or chats on…`
- `try_on_copy`: `Try changes on a throwaway copy of a database before making them for real. action=start makes an in-memory copy of the database. From then…`

## Changes

- 2026-10-30: [description changed](../../deltas/2026-10-30/a27acba80c8350153e96.json): `5 field(s) changed`
- 2026-10-28: [count changed, description changed, tool added](../../deltas/2026-10-28/a27acba80c8350153e96.json): `1 tool(s) added; 2 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://data.azquo.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
