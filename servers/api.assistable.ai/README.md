# api.assistable.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.assistable.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.assistable.ai/mcp` | 16 | [`7f0e88d1f283`](3fd8dc5dfbb162dc18d8.json) | 2026-10-31 |

## Tools at `https://api.assistable.ai/mcp`

- `appointments_list`: `List appointments in a subaccount within an optional date range.`
- `assistants_archive`: `Archive (soft-delete) an assistant.`
- `assistants_create`: `Create an assistant. Required: subAccountId, name. Optional config blocks (llmConfig, voiceConfig, chatConfig) mirror the dashboard create…`
- `assistants_get`: `Fetch an assistant's full configuration by ID. The response includes voice_settings (greeting mode, opening messages, voicemail) and platfo…`
- `assistants_list`: `List assistants in a subaccount (excludes archived by default). Note: voice_settings and platform_tools are returned only by assistants_get…`
- `assistants_update`: `Patch an assistant. Only supplied fields change; nested config blocks are upserted. voice_settings updates call greeting mode, opening mess…`
- `calls_get`: `Fetch a call (status, recording, transcript) by ID.`
- `contacts_get`: `Fetch a contact by ID.`
- `contacts_list`: `List contacts in a subaccount. meta.total is the number of matching contacts, so use it to answer how many contacts there are.`
- `conversations_list`: `List conversations in a subaccount.`
- `search_tools`: `Search Assistable's registered MCP tools by the task the user wants to do. Returns up to 5 exact tool definitions with JSON input schemas a…`
- `tools_create_custom`: `Create a custom tool (toolType=CUSTOM). Name must match /^[a-zA-Z0-9_-]+$/ and be unique in the subaccount.`
- `tools_delete`: `Soft-delete a custom tool.`
- `tools_get`: `Fetch a tool's full configuration.`
- `tools_list`: `List tools visible to a subaccount. Pass includePrebuilt=false for only custom tools.`
- `tools_update`: `Patch a custom tool. Supplying parameters/headers replaces those rows; omit to leave them.`

## Changes

- 2026-10-31: [count changed, tool removed](../../deltas/2026-10-31/3fd8dc5dfbb162dc18d8.json): `2 tool(s) removed`
- 2026-10-30: [count changed, tool removed](../../deltas/2026-10-30/3fd8dc5dfbb162dc18d8.json): `2 tool(s) removed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.assistable.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
