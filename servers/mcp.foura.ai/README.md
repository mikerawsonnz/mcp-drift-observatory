# mcp.foura.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.foura.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.foura.ai/mcp` | 4 | [`2b016af7646b`](b3a044fd8cccae7febc9.json) | 2026-09-23 |

## Tools at `https://mcp.foura.ai/mcp`

- `foura_auto`: `Give it a public URL and get the content back. Use it when only the content matters and not how it is fetched: it escalates from a direct r…`
- `foura_browser`: `Load a public URL in a full browser session. JavaScript runs, the DOM renders, and cookies come back with the response. Use it for single-p…`
- `foura_proxy`: `Route an HTTP request through rotating proxies, retrying on another exit until one delivers. Use it when foura_single is blocked, and whene…`
- `foura_single`: `Send one HTTP request and return the response. Use it for static pages, JSON APIs, and server-rendered HTML, with your own headers, body an…`

## Changes

- 2026-09-23: [schema changed](../../deltas/2026-09-23/b3a044fd8cccae7febc9.json): `20 field(s) changed`
- 2026-09-17: [description changed, schema changed](../../deltas/2026-09-17/b3a044fd8cccae7febc9.json): `89 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.foura.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
