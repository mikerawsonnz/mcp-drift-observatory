# mcp.memoryrouter.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.memoryrouter.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.memoryrouter.ai/mcp` | 10 | [`6b11d59d1c67`](08cc448ffe4ce68bf7d6.json) | 2026-08-20 |

## Tools at `https://mcp.memoryrouter.ai/mcp`

- `commit_reflections`: `Use this to complete a consolidation started with consolidate_memories. Submits the reflection entries you wrote for the checked-out batch.…`
- `consolidate_memories`: `Use this when the user asks to consolidate, reflect on, or organize their memories, or when memory_status or a search result reports that c…`
- `date_search_memories`: `Use this to retrieve memories from a specific time window, for questions like 'what happened last week' or 'most important things this mont…`
- `delete_memories`: `Use this only when the user explicitly asks to delete specific memories and confirms after seeing what will be deleted. Permanently deletes…`
- `forget_all_memories`: `Use this only after the user explicitly requests a full-vault deletion, receives a permanent whole-vault warning, and provides the exact co…`
- `inspect_memory`: `Use this when the user asks why the assistant believes something, or wants to see the source memories behind a reflection. Given a memory i…`
- `memory_status`: `Use this when the user asks whether MemoryRouter is connected, which opaque vault binding is active, or how many memories/tokens the connec…`
- `search`: `Use this legacy compatibility alias when a client explicitly requests a tool named search. It searches the OAuth-selected MemoryRouter vaul…`
- `search_memories`: `Use this when the user asks about a prior decision, preference, person, project, or other fact that may be in their connected MemoryRouter…`
- `store_memory`: `Use this only when the user explicitly asks to remember something or confirms a proposed durable fact. Saves concise user-approved content…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.memoryrouter.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
