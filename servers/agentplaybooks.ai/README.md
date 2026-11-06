# agentplaybooks.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/agentplaybooks.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://agentplaybooks.ai/api/mcp/manage` | 50 | [`b35f62fac3b8`](009e0bf3c8a619f8ac0a.json) | 2026-09-12 |

## Tools at `https://agentplaybooks.ai/api/mcp/manage`

- `archive_memories`: `Hide matching memories from normal search and context, retaining them in the longterm tier. Search scope='archived' to find them or read_me…`
- `call_connected_tool`: `Call a tool on one of this playbook's connected MCP or OpenAPI servers. Arguments are forwarded as-is and the result mirrors the connected…`
- `consolidate_memories`: `Consolidate related memories under a new parent memory with a summary. Child rows stay readable; by default they are archived to the longte…`
- `create_mcp_server`: `Connect an MCP or OpenAPI server to this playbook by storing its transport configuration. This writes playbook state; it does not by itself…`
- `create_persona`: `Set the playbook's singleton persona name and system prompt. This does not add a second persona; it is a backward-compatible alias that ove…`
- `create_playbook`: `Create a new playbook container for a singleton persona, skills, and memory. Each call inserts a new playbook; it does not upsert by name.…`
- `create_run`: `Create a workflow run so this playbook can be applied immediately with isolated context and canvas artifacts. Requires canvas:write or full…`
- `create_skill`: `Create a new skill for this playbook. Use this to expand capabilities. Requires full or skills:write permission. Use update_skill to change…`
- `create_task_graph`: `Create a hierarchical task plan in one call: a parent plan memory plus a child node per subtask. Upserts by key, so repeating the same plan…`
- `delete_mcp_server`: `Disconnect an MCP or OpenAPI server from this playbook. The remote server is not shut down; only this playbook's connection record is remov…`
- `delete_memory`: `Permanently delete a memory and its saved history. Requires memory:write or full permission. To hide an entry while retaining its content,…`
- `delete_persona`: `Reset the playbook's singleton persona to the default Assistant name and system prompt. Despite the delete_* name, this is not a hard delet…`
- `delete_playbook`: `Permanently delete a playbook and all of its contents (persona, skills, memory, API keys, canvas, and secrets). This cannot be undone. Requ…`
- `delete_run`: `Permanently delete a workflow run and its isolated canvas artifacts. This cannot be undone. Requires canvas:write or full permission. Use u…`
- `delete_secret`: `Permanently delete a secret. Cannot be undone. Requires secrets:write or full permission. Use rotate_secret to replace the value without re…`
- `delete_skill`: `Permanently delete a skill from this playbook. This cannot be undone except by recreating the skill. Requires full or skills:write permissi…`
- `find_tools`: `Search this playbook's complete tool catalog by keyword: the built-in playbook tools (memory, skills, canvas, workflow runs, secrets) and e…`
- `get_canvas_toc`: `Get the table of contents for a canvas document. Returns section IDs, headings, and levels for navigation and patch_canvas_section. Read-on…`
- `get_memory_context`: `Get a context-optimized view of memories: full working memory, summaries for contextual, and keys only for longterm. Read-only. Use this to…`
- `get_memory_history`: `Read previous versions of a memory by its current key, including original memory_at and saved contents. History is excluded from normal sea…`
- `get_memory_tree`: `Get a hierarchical tree of memories showing parent-child relationships and per-node status. Read-only. Use this to visualize task graphs; u…`
- `get_playbook`: `Get a playbook with its singleton persona, skills, connected MCP servers, and memory. This is the only persona retrieval tool; there is no…`
- `get_skill`: `Return the full definition of one skill in this playbook, including name, description, content, priority, and attachments. Identify the ski…`
- `list_canvas`: `List canvas documents in a workflow run. Canvas documents are collaborative markdown files that multiple agents can edit in parallel. Omit…`
- `list_mcp_servers`: `List the MCP and OpenAPI servers connected to this playbook, including transport metadata and discovered capability counts. Read-only. Ther…`
- `list_playbooks`: `List playbooks owned by or shared with the authenticated user, including access role and content counts. Read-only; it does not create or m…`
- `list_runs`: `List workflow runs for this playbook. Runs isolate canvas artifacts and execution context. Read-only. There is no get_run; this list return…`
- `list_secrets`: `List all secret names and metadata in this playbook. Does not return values — secret values are never exposed to agents. Requires secrets:r…`
- `list_skill_versions`: `List historical versions of a skill for auditing or rollback. Read-only. Use this before rollback_skill; use get_skill for the current defi…`
- `list_skills`: `List every skill currently attached to this playbook, returning id, name, description, content, licence, and priority ordered by priority d…`
- `lock_canvas_section`: `Lock a section for exclusive editing so other agents cannot modify it. Requires canvas:write or full permission. Always unlock_canvas_secti…`
- `patch_canvas_section`: `Edit a specific section of a canvas document. Parallel-safe: only the targeted section is updated. Requires canvas:write or full permission…`
- `promote_memory`: `Restore a memory's visibility, promote it to a higher tier or boost its priority for active use. This tool cannot demote; use archive_memor…`
- `read_canvas`: `Read a canvas document. Returns full content, sections structure, and metadata. Optionally read a specific section by ID. Read-only. Use ge…`
- `read_memory`: `Read one memory entry by key and return its value, tags, tier, summary, and metadata. This is not a pure read: it increments access_count a…`
- `rollback_skill`: `Rollback a skill to a previous version recorded by list_skill_versions. The current definition is replaced and cannot be recovered except b…`
- `rotate_secret`: `Rotate an existing secret with a new value. The old value is permanently replaced and cannot be recovered. Requires secrets:write or full p…`
- `search_memory`: `Search memory keys, JSON values, descriptions and summaries. Defaults to current, non-archived memories. scope='archived' searches archived…`
- `store_secret`: `Store a new encrypted secret. The value is encrypted with AES-256-GCM using a per-user derived key and never stored or returned in plaintex…`
- `unlock_canvas_section`: `Unlock a previously locked canvas section so other agents can edit it. Requires canvas:write or full permission. Use lock_canvas_section to…`
- `update_mcp_server`: `Update a connected MCP or OpenAPI server's stored name, description, tools, resources, or transport. Requires playbooks:write or full permi…`
- `update_persona`: `Update the singleton persona's name, system prompt, or metadata without resetting to defaults. persona_id must equal playbook_id because th…`
- `update_playbook`: `Update this playbook's name, description, visibility, tags, config, singleton persona fields, or always-on project instructions. Replacemen…`
- `update_run`: `Update a workflow run's name, status, or context. Requires canvas:write or full permission. Use list_runs to find run_id (there is no get_r…`
- `update_skill`: `Update an existing skill in this playbook. Requires full or skills:write permission. Use create_skill to add a skill, list_skill_versions b…`
- `update_task_status`: `Update the status of a task node in a hierarchical plan. When all children of a parent are completed, the parent is auto-updated. Returns t…`
- `use_secret`: `Send a GET or HEAD request with a secret injected as a header, and return the response. The secret value is never returned to the agent — i…`
- `use_secret_write`: `Send a POST, PUT, PATCH or DELETE request with a secret injected as a header, and return the response. The secret value is never returned t…`
- `write_canvas`: `Create or fully replace a canvas document. Markdown headings are auto-parsed into sections for parallel editing. A replace overwrites prior…`
- `write_memory`: `Create or update a memory by key; previous contents are saved automatically and readable with get_memory_history. memory_at is optional and…`

## Changes

- 2026-09-12: [count changed, description changed, schema changed, tool added](../../deltas/2026-09-12/009e0bf3c8a619f8ac0a.json): `1 tool(s) added; 35 field(s) changed`
- 2026-08-22: [annotation changed, count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-08-22/009e0bf3c8a619f8ac0a.json): `2 tool(s) added; 411 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://agentplaybooks.ai/api/mcp/manage"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
