# api.flowcastle.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.flowcastle.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.flowcastle.ai/api/mcp` | 51 | [`4e96d9180ba0`](7ab5e0161f25f4340969.json) | 2026-10-06 |

## Tools at `https://api.flowcastle.ai/api/mcp`

- `apply_actions`: `Validate and apply a batch of flow-builder actions — the single write path for editing flows, blocks, variables, broadcasts, sequences, and…`
- `create_application`: `Create a new application (workspace) owned by the caller. Requires a personal API key (usr_...) — application-scoped keys cannot create app…`
- `create_contact`: `Create a contact manually — for imports or externally-sourced audiences; contacts who message a bot are created automatically. Requires the…`
- `create_follow_up_task`: `Create a follow-up reminder for a person to get back to a contact. Creates persistent state and is NOT idempotent: calling it twice creates…`
- `deploy_application`: `Publish the workspace to its bots — the API equivalent of the dashboard's Deploy button. This is the step that makes edits live. apply_acti…`
- `execute_telegram_operation`: `Submit one supported read operation on the connected telegram_mtproto account. Call list_telegram_operations for the input schema. Returns…`
- `get_action_schema`: `Return the action-authoring contract that apply_actions batches are validated against. Read-only, needs no API key. Called with NO argument…`
- `get_application_context`: `Return the full application-level automation context in one read-only call: every flow (with folders), connected bots, variables, sequences…`
- `get_block_details`: `Return the complete contents of one block: block data, action configs, HTTP request bodies, custom-code files, triggers, menu payloads, and…`
- `get_broadcast_analytics`: `Return engagement analytics for a broadcast: delivery breakdown by status plus per-message-block sent and clicked counts for its flow, over…`
- `get_broadcast_details`: `Return full details for a single broadcast: status, schedule, recurrence rule, linked flow, and delivery breakdown by status. Read-only. Ca…`
- `get_contact`: `Return one contact's full profile plus every contact-variable value stored for them. Read-only. Values may hold personal data; variables of…`
- `get_contact_activity`: `Return one contact's engagement history: goals they achieved and buttons they clicked, newest first, plus all-time goal totals. Read-only.…`
- `get_design_guidelines`: `Return the flow-design rules that validation does NOT enforce: when to split a branch into its own flow, how navigation and menus must be w…`
- `get_flow_analytics`: `Measure how NAMED flows are actually used over the last 30 days: how many contacts entered each one, where inside it they stop (per block,…`
- `get_flow_context`: `Return one flow's graph topology: its blocks, how they link, and a short summary per block. Read-only. Deliberately omits block data and ac…`
- `get_flow_example`: `Return one reusable flow example by id, optionally with a complete action batch you can adapt and pass to apply_actions. Read-only, needs n…`
- `get_funnel_analytics`: `Return the measured conversion funnels of the workspace's ENTRY flows over the last 30 days, busiest first: how many new contacts entered,…`
- `get_module_catalog`: `Return a compact index of both installed and available marketplace modules, with each module's key, versions, description, actions, and tri…`
- `get_module_details`: `Return everything needed to use one module: action input fields and their types, trigger configuration, manual setup fields (credentials an…`
- `get_pulse_item`: `Return one Pulse item in full: the measured evidence, the ids of the conversations and execution-log rows behind it, and the change Apply w…`
- `get_survey_results`: `Read what customers ANSWERED in this workspace's surveys. A survey is any flow marked isSurvey: its choice questions record which option ea…`
- `get_telegram_operation`: `Read a Telegram operation status and result using its requestId and the same applicationId/botId used for submission. Requires manage_broad…`
- `get_variable_context`: `Search variable definitions by scope and keyword. Read-only. Returns { variables, total, returned, truncated } — compare returned against t…`
- `get_website_import`: `Status of a website import started by import_website_knowledge or an import_website_into_knowledge_base action: stage, progress, counters,…`
- `get_workspace_summary`: `Return a compact application, flow, sequence, operation, and bot summary — the cheapest way to orient in a workspace. Read-only, no side ef…`
- `import_website_knowledge`: `Crawl a website into a knowledge base so an AI_TOOL_ROUTER can answer from it. Creates a new base (named after the host) unless knowledgeBa…`
- `install_module`: `Install an exact marketplace module version into an application and create any missing installed-template actions. Requires the manage_auto…`
- `list_applications`: `List the applications this API key can access, with the caller role and the permissions it grants. Start here when using a personal API key…`
- `list_broadcasts`: `List broadcasts in the application with status, schedule, and delivery counts. Read-only. Filters combine as AND. Note that delivery counts…`
- `list_contact_tags`: `List the contact tags in use in the application (or one bot) with how many contacts carry each, most-used first. Read-only. This is the att…`
- `list_contacts`: `List and search contacts in the application, paginated, newest first. Read-only. Filters combine as AND; search matches name, username, ema…`
- `list_event_contacts`: `The reverse lookup: which contacts triggered one analytics event — achieved a goal (kind GOAL + goalKey), clicked a button (BUTTON_CLICK +…`
- `list_follow_up_tasks`: `List follow-up tasks — reminders for a person to get back to a contact. Read-only, ordered by due time so overdue work comes first. A follo…`
- `list_pulse_items`: `List Pulse items — the workspace attention queue. Two kinds: 'attention' is an observed problem a detector found (failing flows, a failed b…`
- `list_telegram_operations`: `Discover supported Telegram MTProto account operations, input schemas, permissions and limits. Requires manage_broadcasts. All current oper…`
- `list_watched_groups`: `List the group/channel chats a telegram_mtproto userbot monitors. Read-only. The watched list is the single source of truth for which chats…`
- `query_flow_logs`: `Read the bot execution log (flow_execution_log) — the record of what the runtime actually did, and the only place that separates "the actio…`
- `read_messages`: `Read the message transcript: what users sent the bot and what the bot sent back, newest first. Source is the runtime's own message ledger,…`
- `run_flow_autotest`: `Runs deterministic behavioural tests against flows that are ALREADY applied (compiles them to an AST and simulates a user). Call after appl…`
- `search_flow_examples`: `Search the library of reusable flow examples covering common business cases (lead capture, onboarding, payments, reminders). Read-only, nee…`
- `search_flows`: `Find every flow and block whose contents contain a keyword. Read-only. Searches message text and its translations, button labels and URLs,…`
- `send_flow_to_contacts`: `Run an EXISTING interactive flow for each listed contact right now, outside any trigger — as if each of them had just triggered it. Use it…`
- `send_message`: `Send a message to ONE contact right now, outside any flow. For reaching many contacts use a broadcast instead. Target the contact with cont…`
- `set_watched_groups`: `Replace a telegram_mtproto userbot's watched-groups list — the chats it monitors. Requires the manage_settings permission. SET semantics: s…`
- `sync_dialog_contacts`: `Import a telegram_mtproto userbot's existing chats as contacts — DM partners, groups, and channels — so everything the account already talk…`
- `update_application`: `Update application-level settings (name, active state, default language, language for everyone else, incoming-message behavior). Requires t…`
- `update_contact`: `Update a contact's profile fields and/or contact-variable values. Requires the manage_broadcasts permission. Only the fields you pass are c…`
- `update_follow_up_task`: `Close, reopen, snooze, or reschedule one follow-up task. Completing it records that a person handled the reminder — it does not message the…`
- `update_pulse_item`: `Change one Pulse item's state. Every action changes the queue for the WHOLE workspace — an item belongs to the workspace, not to whoever ca…`
- `validate_actions`: `Dry-run validation of a proposed batch of flow-builder actions. Mutates nothing and is safe to repeat. OPTIONAL: apply_actions runs this ex…`

## Changes

- 2026-10-06: [schema changed](../../deltas/2026-10-06/7ab5e0161f25f4340969.json): `1 field(s) changed`
- 2026-10-05: [description changed](../../deltas/2026-10-05/7ab5e0161f25f4340969.json): `1 field(s) changed`
- 2026-09-30: [description changed, schema changed](../../deltas/2026-09-30/7ab5e0161f25f4340969.json): `3 field(s) changed`
- 2026-09-29: [description changed, schema changed](../../deltas/2026-09-29/7ab5e0161f25f4340969.json): `14 field(s) changed; signals: url_introduced`
- 2026-09-24: [schema changed](../../deltas/2026-09-24/7ab5e0161f25f4340969.json): `19 field(s) changed`
- 2026-09-23: [count changed, tool added](../../deltas/2026-09-23/7ab5e0161f25f4340969.json): `1 tool(s) added`
- 2026-09-13: [schema changed](../../deltas/2026-09-13/7ab5e0161f25f4340969.json): `6 field(s) changed`
- 2026-09-11: [description changed, schema changed](../../deltas/2026-09-11/7ab5e0161f25f4340969.json): `10 field(s) changed`
- 2026-09-10: [count changed, schema changed, tool added](../../deltas/2026-09-10/7ab5e0161f25f4340969.json): `7 tool(s) added; 8 field(s) changed`
- 2026-09-08: [count changed, description changed, schema changed, tool added](../../deltas/2026-09-08/7ab5e0161f25f4340969.json): `1 tool(s) added; 7 field(s) changed`
- 2026-09-07: [count changed, description changed, schema changed, tool added](../../deltas/2026-09-07/7ab5e0161f25f4340969.json): `6 tool(s) added; 10 field(s) changed`
- 2026-09-04: [description changed, schema changed](../../deltas/2026-09-04/7ab5e0161f25f4340969.json): `15 field(s) changed; signals: url_introduced`
- 2026-09-03: [count changed, tool added](../../deltas/2026-09-03/7ab5e0161f25f4340969.json): `1 tool(s) added; signals: imperative_language_introduced` **(notable)**
- 2026-09-02: [count changed, description changed, schema changed, tool added](../../deltas/2026-09-02/7ab5e0161f25f4340969.json): `1 tool(s) added; 7 field(s) changed`
- 2026-09-01: [count changed, description changed, schema changed, tool added](../../deltas/2026-09-01/7ab5e0161f25f4340969.json): `3 tool(s) added; 25 field(s) changed`
- 2026-08-27: [count changed, tool added](../../deltas/2026-08-27/7ab5e0161f25f4340969.json): `3 tool(s) added`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.flowcastle.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
