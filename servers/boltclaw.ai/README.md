# boltclaw.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/boltclaw.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://boltclaw.ai/docs/mcp-server` | 2 | [`be9b846f09b2`](d63a924fcbe09ea5ec53.json) | 2026-11-06 |

## Tools at `https://boltclaw.ai/docs/mcp-server`

- `fetch`: `Read one documentation page in full, as markdown. The id is what 'search' returns, which is the page's path without /docs/ - for example 'a…`
- `search`: `Find documentation pages about a subject. Returns an id, a title, a URL and a matching line for each hit, best first. Pass the id to 'fetch…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://boltclaw.ai/docs/mcp-server"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
