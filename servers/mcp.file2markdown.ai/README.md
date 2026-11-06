# mcp.file2markdown.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.file2markdown.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.file2markdown.ai/mcp` | 4 | [`248523c62050`](d8374fa51a92d939b86f.json) | 2026-09-19 |

## Tools at `https://mcp.file2markdown.ai/mcp`

- `convert_base64`: `Convert base64-encoded file contents to Markdown. filename is required and drives format detection (e.g. "report.docx"). Intended for progr…`
- `convert_url`: `Fetch a URL (web page, PDF, Office doc, and more) and convert it to Markdown. Works on publicly accessible URLs. Web pages are converted fr…`
- `list_supported_formats`: `List supported input formats, per-tier limits, and which features need Pro. Single source of truth — do not claim capabilities beyond what…`
- `usage_status`: `Check your tier and remaining conversions before burning a call.`

## Changes

- 2026-09-19: [description changed, schema changed](../../deltas/2026-09-19/d8374fa51a92d939b86f.json): `8 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.file2markdown.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
