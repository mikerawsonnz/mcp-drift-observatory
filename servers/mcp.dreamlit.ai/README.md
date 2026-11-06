# mcp.dreamlit.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.dreamlit.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.dreamlit.ai/mcp` | 12 | [`7fadefd35b78`](03165f6925de72d31cfe.json) | 2026-10-13 |

## Tools at `https://mcp.dreamlit.ai/mcp`

- `confirm_publish`: `Use only after explicit user confirmation and a prior prepare_publish result to publish or schedule a Dreamlit workflow. Side effect: insta…`
- `create_or_update_workflow`: `Creates a new Dreamlit workflow draft or updates an existing draft from an outcome-oriented natural-language prompt. Use after get_status;…`
- `get_analytics`: `Read-only. Use to query Dreamlit analytics for overview metrics, notification rows, recipient engagement, or workflow run rows with filters…`
- `get_status`: `Read-only. Use first when the agent needs Dreamlit product guidance, prompting guidance, approved workspace context, project setup, schema…`
- `get_workflow_and_preview_url`: `Read-only. Use before editing, verifying, or preparing publish for an existing workflow. Returns normalized draft and published workflow st…`
- `list_brand_styles`: `Read-only. Use when the user wants to inspect saved project brand styles for generated email drafts. Returns paginated project brand style…`
- `list_projects`: `Read-only. Use when the target project is unknown or the user names a project instead of providing an id. Returns accessible Dreamlit proje…`
- `list_workflows`: `Read-only. Use to find workflows in a project by name, description, or trigger type before inspection or editing. Trigger filters include d…`
- `prepare_publish`: `Read-only validation step before publishing. Use after the user asks to publish and after inspecting the workflow if needed. Returns valida…`
- `rename_workflow`: `Use when the user asks to rename an existing Dreamlit workflow. Side effect: changes only the workflow name; the draft, published version,…`
- `send_workflow_test`: `Side effect when confirmSend is true: sends one current draft email or Slack message for review, but does not publish, schedule, or edit th…`
- `unpublish_workflow`: `Use after explicit user intent to unpublish a Dreamlit workflow. Side effect: disables live triggers or schedules for that workflow and sto…`

## Changes

- 2026-10-13: [schema changed](../../deltas/2026-10-13/03165f6925de72d31cfe.json): `312 field(s) changed`
- 2026-10-10: [count changed, description changed, schema changed, tool added](../../deltas/2026-10-10/03165f6925de72d31cfe.json): `1 tool(s) added; 7 field(s) changed; signals: imperative_language_introduced` **(notable)**

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.dreamlit.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
