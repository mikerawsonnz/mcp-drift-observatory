# getminds.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/getminds.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://getminds.ai/mcp` | 24 | [`30b7f9bb16cb`](4aa1efd007b57cd82e91.json) | 2026-09-19 |

## Tools at `https://getminds.ai/mcp`

- `ask_audience`: `Submits exactly one respondent-visible standalone question to one existing Audience, identified by exact ID or fuzzy name. It creates a pri…`
- `ask_study`: `Submits exactly ONE respondent-visible question in an existing Study. Applicability: one standalone question, or one adaptive follow-up who…`
- `create_audience_from_brief`: `Supports operationId-only requests to read a previously accepted preview or creation job and retrieve its result without creating another A…`
- `create_study`: `Creates a new Study workspace from existing Audiences or inline Audience configurations; it does not ask questions or run research. Follow-…`
- `export_audience`: `Exports an Audience brief through the same unified branded renderer used by the web app. Supports Markdown, PDF, DOCX, and PPTX. Binary art…`
- `export_heatmap`: `Exports a completed website heatmap from a Study result, identified by the message ID reported with the completed result. Returns the same…`
- `export_mind`: `Generates a branded profile for one existing Mind, identified by exact ID or fuzzy name. Markdown is returned inline by default; PDF, DOCX,…`
- `export_study`: `Starts an asynchronous export of Study results and returns an export job ID. Supports executive briefs and full reports in PDF, DOCX, PPTX,…`
- `get_audience_limits`: `**Call this before creating an Audience whenever a size is in play** — the user named a number, asked for "as many as possible", or you are…`
- `get_study_run`: `Returns durable progress or results for one confirmed multi-question run inside a Study, including its immutable confirmed plan, server-pre…`
- `get_study_status`: `Applicability: use only when the user asks to find, inspect, or check a Study or its export. For a deletion-only request, do not call this…`
- `get_study_summary`: `Returns or refreshes the semantic summary for a Study as Markdown plus flexible evidence blocks. Website, image, and video analyses retain…`
- `import_audience_sources`: `Imports supplied UTF-8 text, Markdown, CSV and JSON research files into account-owned storage. Accepts file contents rather than local path…`
- `list_audiences`: `Lists the authenticated user's Audiences, most recently updated first, one page at a time (limit, default 20, and offset; nextOffset contin…`
- `list_model_connections`: `Lists the authenticated team’s model connections with IDs, current revisions, endpoints, and verified text, structured-output, streaming, a…`
- `list_research_methods`: `Lists Minds research methods with availability, complexity, executable status, and fallback metadata. Results distinguish currently executa…`
- `list_studies`: `Applicability: use only when the user asks to find, inspect, or check a Study or its export. For a deletion-only request, do not call this…`
- `list_study_drafts`: `Lists durable unfinished study drafts, or returns the complete saved planning state for one exact draft ID. Draft records are distinct from…`
- `list_study_templates`: `List your own and team-shared Advanced Study templates, most used first, or read one exact template including its revision, research method…`
- `manage_study_template`: `Save, explicitly update, delete or use a Custom research template. Templates are private by default. Owners can set update.isSharedWithTeam…`
- `plan_study_questions`: `Creates or revises a non-executing draft for a multi-question plan inside an existing Study. Applicability: this is the setup operation for…`
- `run_study_questions`: `Executes the exact stored multi-question draft revision inside the target Study after explicit confirmation. One execution submits the ENTI…`
- `save_study_draft`: `Creates or checkpoints an unfinished Quick or Custom Study draft without starting research. It saves the objective, context, selected Audie…`
- `study_heatmap`: `Read or start a question asset heatmap, with the same behavior as Minds UI. For a specific video or image pass assetKey: its saved upload p…`

## Changes

- 2026-09-19: [description changed, field changed, schema changed](../../deltas/2026-09-19/4aa1efd007b57cd82e91.json): `81 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-09-18: [field changed](../../deltas/2026-09-18/4aa1efd007b57cd82e91.json): `9 field(s) changed`
- 2026-09-17: [field changed](../../deltas/2026-09-17/4aa1efd007b57cd82e91.json): `9 field(s) changed`
- 2026-09-16: [count changed, field changed, tool added](../../deltas/2026-09-16/4aa1efd007b57cd82e91.json): `2 tool(s) added; 12 field(s) changed`
- 2026-09-15: [annotation changed, description changed, field changed](../../deltas/2026-09-15/4aa1efd007b57cd82e91.json): `17 field(s) changed`
- 2026-09-14: [field changed, schema changed](../../deltas/2026-09-14/4aa1efd007b57cd82e91.json): `62 field(s) changed`
- 2026-09-11: [count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-09-11/4aa1efd007b57cd82e91.json): `3 tool(s) added; 67 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-09-10: [annotation changed, description changed, field changed, schema changed](../../deltas/2026-09-10/4aa1efd007b57cd82e91.json): `13 field(s) changed; signals: length_more_than_doubled, url_introduced`
- 2026-09-09: [description changed, schema changed](../../deltas/2026-09-09/4aa1efd007b57cd82e91.json): `27 field(s) changed`
- 2026-09-07: [annotation changed, description changed, schema changed](../../deltas/2026-09-07/4aa1efd007b57cd82e91.json): `70 field(s) changed; signals: imperative_language_introduced` **(notable)**
- 2026-09-05: [description changed, schema changed](../../deltas/2026-09-05/4aa1efd007b57cd82e91.json): `12 field(s) changed; signals: length_more_than_doubled`
- 2026-09-04: [count changed, schema changed, tool added](../../deltas/2026-09-04/4aa1efd007b57cd82e91.json): `1 tool(s) added; 7 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-09-03: [schema changed](../../deltas/2026-09-03/4aa1efd007b57cd82e91.json): `34 field(s) changed`
- 2026-09-02: [description changed, schema changed](../../deltas/2026-09-02/4aa1efd007b57cd82e91.json): `38 field(s) changed; signals: file_path_introduced`
- 2026-08-28: [description changed, schema changed, tool added, tool removed](../../deltas/2026-08-28/4aa1efd007b57cd82e91.json): `13 tool(s) added; 13 tool(s) removed; 15 field(s) changed; signals: file_path_introduced, length_more_than_doubled`
- 2026-08-26: [description changed, schema changed](../../deltas/2026-08-26/4aa1efd007b57cd82e91.json): `93 field(s) changed; signals: imperative_language_introduced` **(notable)**
- 2026-08-20: [annotation changed, description changed, schema changed](../../deltas/2026-08-20/4aa1efd007b57cd82e91.json): `14 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://getminds.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
