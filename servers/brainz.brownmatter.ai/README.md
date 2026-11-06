# brainz.brownmatter.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/brainz.brownmatter.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://brainz.brownmatter.ai/mcp` | 17 | [`2f79e2404db8`](6e08d69177df4991706a.json) | 2026-11-01 |

## Tools at `https://brainz.brownmatter.ai/mcp`

- `complete_task`: `Mark a task done. Sets taskStatus=done + doneAt and appends 'outcome' to the task body as an Outcome section. The result carries a one-line…`
- `create_task`: `Turn a finding into first-class work: creates a 'task'-type concept with taskStatus=open and the given relations — part_of a domain, 'reali…`
- `create_vault`: `Create a new, empty vault owned by you and add it to this connection. Returns the new vault and the vaults this connection can now use. Onc…`
- `delete_concept`: `Remove a concept from the vault and all of its outgoing edges. Use to clear a note that is wrong, obsolete, or junk (e.g. a probe or test n…`
- `dream`: `Dreaming: a scheduled consolidation sweep over this vault. Light stages what changed since the last dream (near-duplicate concepts, finishe…`
- `get_concept`: `Fetch one concept by exact id: full markdown body, metadata, and its direct graph neighbors (each with the relation that connects it). Use…`
- `get_context`: `Assemble a markdown briefing of the concepts most relevant to a query and/or explicit ids, expanded through the graph and trimmed to a toke…`
- `get_related`: `Walk the knowledge graph outward from a concept and return everything within 'depth' hops, with distance and the edge path that reached it.…`
- `link_concepts`: `Add a typed, directed edge between two existing concepts by editing the 'from' note's frontmatter (e.g. lead-scoring depends_on contact-mod…`
- `list_concepts`: `Enumerate concept metadata (no bodies), optionally filtered by product, type, or a single tag. Use to get the lay of the land in an unfamil…`
- `list_tasks`: `List the vault's work pile: 'task'-type concepts with their lifecycle (open/taken/done), oldest first, including who has taken each one (ta…`
- `onboard`: `Index an existing product's codebase into this vault. {action: "start"} returns the onboarding playbook: a method for surveying the codebas…`
- `search_concepts`: `Search the product knowledge vault by free-text query. Useful when you need product knowledge but don't yet know which concept ids exist. R…`
- `sync`: `Re-index an onboarded vault after the code changes (drift). {action: "start"} returns the sync playbook: the vault's last_synced_at, a cove…`
- `take_task`: `Claim a task and get its briefing in one call. Pass an 'id' to claim a specific task, or omit it to claim the next open task (oldest open b…`
- `upsert_concept`: `Write a concept note into the vault (creates or overwrites the markdown file, then reindexes it). Use to capture new product knowledge disc…`
- `vault_stats`: `Summarize the vault: counts of concepts and edges, the products and tags in use, a breakdown by concept type, and whether semantic search i…`

## Changes

- 2026-11-01: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-01/6e08d69177df4991706a.json): `1 tool(s) added; 73 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://brainz.brownmatter.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
