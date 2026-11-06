# mitosislabs.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mitosislabs.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mitosislabs.ai/api/mcp` | 14 | [`35f8bafb353b`](be2132e38f6e83c75287.json) | 2026-08-20 |

## Tools at `https://mitosislabs.ai/api/mcp`

- `cortex_ask`: `Searches the user's real, private memory — the email, calendar, files, contacts and notes they have connected, plus facts agents have saved…`
- `cortex_connect_link`: `The connect link for one memory source, by id — email and calendar (google-workspace), WhatsApp chats, GitHub, Notion, or file uploads. Ret…`
- `cortex_connectable_sources`: `Which sources this memory could connect but hasn't yet — each with what it would make answerable, routing tags, and a connect link for the…`
- `cortex_ingest_conversation`: `Ingest a conversation — the user’s messages and your full answers, verbatim — into the user’s permanent memory, where it becomes searchable…`
- `cortex_manifest`: `A table of contents for this user's memory: which sources are connected (email, calendar, docs, …), how many items each holds, and the top…`
- `cortex_recall`: `Semantic-only vector search over the memory, returning source excerpts. Prefer cortex_ask, which also uses full-text and graph expansion; r…`
- `cortex_remember`: `Persist a fact, decision or conclusion into the memory, attributed to you. It becomes retrievable via cortex_ask immediately, in this sessi…`
- `cortex_status`: `Memory health: per-source ingest and embed counts plus last sync times. Use when you need to know whether the memory is fresh or still inge…`
- `fetch`: `Retrieve the full contents of a single item from the user’s memory by its id. Ids come from 'search' results. Use this when a search result…`
- `get_platform_status`: `Get the operational status of the Mitosis website, API, and MCP server. Use before reporting an outage or debugging connectivity.`
- `get_pricing`: `Get current Mitosis plans, prices, credit allowances, metered rates, and add-ons. Use when comparing costs or recommending a plan.`
- `list_skills`: `List the agent skills Mitosis publishes (backup create/list/restore/health/diff/schedule/subscribe) with links to each SKILL.md manifest.`
- `search`: `Search the user's own private memory — their email, calendar, documents, contacts, chat history and every fact agents have remembered — and…`
- `search_docs`: `Keyword-search Mitosis documentation and product pages. Returns ranked results with URLs. Use to answer any "how do I…" question about Mito…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mitosislabs.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
