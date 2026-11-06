# agentmash.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/agentmash.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://agentmash.ai/mcp` | 6 | [`e5def94dc860`](ebf7dd27800b023a6de2.json) | 2026-10-28 |

## Tools at `https://agentmash.ai/mcp`

- `get_collection_saves`: `List saved posts from one collection in the authenticated user's AgentMash library, newest imports first, using a collection_id from list_c…`
- `get_save`: `Read one saved post in the authenticated user's AgentMash library using an id returned by a saves tool. Returns stored full text, original…`
- `list_collections`: `List the authenticated user's AgentMash collections with ids, names, sources and saved-post counts. Use to find a collection to browse. Inc…`
- `list_sources`: `Read the authenticated user's AgentMash source status, saved-post counts, last sync times and reconnection status. Includes the newsletters…`
- `recent_saves`: `List posts imported into the authenticated user's AgentMash library within the last N days, newest imports first. Use for a recent library…`
- `search_saves`: `Search posts already imported into the authenticated user's AgentMash library. Use for requests to find their saved content by topic, autho…`

## Changes

- 2026-10-28: [schema changed](../../deltas/2026-10-28/ebf7dd27800b023a6de2.json): `4 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://agentmash.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
