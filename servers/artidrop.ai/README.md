# artidrop.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/artidrop.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://artidrop.ai/mcp` | 4 | [`e36a4ff68b66`](c2c055447e4e8f5a62d4.json) | 2026-08-20 |

## Tools at `https://artidrop.ai/mcp`

- `get`: `Get artifact metadata. Set include_content to true to also return the full HTML content.`
- `publish`: `Publish HTML or Markdown content as a shareable URL. Pass 'content' byte-for-byte from the source — do not retype, reformat, minify, summar…`
- `publish_site`: `Publish a multi-file HTML site from a base64-encoded ZIP file. The ZIP must contain an index.html at its root. For sites larger than ~10MB…`
- `versions`: `List version history of an artifact`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://artidrop.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
