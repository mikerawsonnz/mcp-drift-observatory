# docs.bithuman.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/docs.bithuman.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://docs.bithuman.ai/docs-mcp` | 2 | [`e86e89384785`](27e9bd1338d47ebafd7d.json) | 2026-10-11 |

## Tools at `https://docs.bithuman.ai/docs-mcp`

- `fetch`: `Fetch one docs page as markdown by the id 'search' returned (a path such as /platforms/python), or by its full docs.bithuman.ai URL. Return…`
- `search`: `Search docs.bithuman.ai (bitHuman real-time avatar SDKs, the REST API, deployment options, models, pricing). Returns JSON {results: [{id, t…`

## Changes

- 2026-10-11: [description changed, schema changed](../../deltas/2026-10-11/27e9bd1338d47ebafd7d.json): `3 field(s) changed; signals: length_more_than_doubled, url_introduced`
- 2026-10-03: [description changed](../../deltas/2026-10-03/27e9bd1338d47ebafd7d.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://docs.bithuman.ai/docs-mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
