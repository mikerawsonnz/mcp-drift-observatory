# api.inference.sh: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.inference.sh.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.inference.sh/mcp` | 25 | [`76025aa484dc`](47dcb336af169298b8e5.json) | 2026-08-20 |

## Tools at `https://api.inference.sh/mcp`

- `app_get`: `Get detailed app info including input/output schemas and version history`
- `app_list`: `Search and filter available apps on inference.sh`
- `app_run`: `Run an app on inference.sh. Creates a task that executes the app with the given input.`
- `knowledge_create`: `Create a new knowledge entry (concept, observation, preference, reference, etc.)`
- `knowledge_delete`: `Delete a knowledge entry by ID`
- `knowledge_get`: `Get detailed information about a knowledge entry by namespace/name or ID`
- `knowledge_list`: `List your knowledge entries, optionally filtered by type`
- `knowledge_search`: `Search your knowledge entries by query`
- `mcp_connect`: `Initiate a connection to an MCP server. For OAuth servers, returns an authorization URL to open in a browser.`
- `mcp_disconnect`: `Remove connection to an MCP server`
- `mcp_get`: `Get details about an MCP server including connection status`
- `mcp_list`: `Browse available MCP servers that can be connected to`
- `mcp_run`: `Call a tool on a connected MCP server. The server must be connected first via mcp_connect.`
- `mcp_search`: `Search available MCP servers by query`
- `mcp_tools`: `List available tools on a connected MCP server, or get details for a specific tool`
- `skill_files`: `List supplementary files for a skill (references, scripts, etc.)`
- `skill_search`: `Search the public skill store`
- `skill_store`: `Browse approved skills in the public skill store`
- `skill_upload`: `Create or update a skill with SKILL.md content and optional supporting files`
- `skill_use`: `Fetch a skill's assembled SKILL.md content. Tries the inference.sh store first, falls back to GitHub. Returns the full skill content for th…`
- `skill_view`: `View a specific supplementary file from a skill's manifest`
- `task_cancel`: `Cancel a running or queued task`
- `task_get`: `Get status and output of a task`
- `task_list`: `List your tasks on inference.sh`
- `task_logs`: `Get execution logs for a task`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.inference.sh/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
