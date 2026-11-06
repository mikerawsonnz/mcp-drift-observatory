# freudly.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/freudly.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://freudly.ai/mcp` | 2 | [`03edc13ce99d`](b34e7d5b4d3fe06e55dc.json) | 2026-10-02 |

## Tools at `https://freudly.ai/mcp`

- `get_test_info`: `Details of one Freudly test by id: description, instructions, the scales it measures, authors and sources, limitations, what the user needs…`
- `search_tests`: `Search the Freudly catalogue of psychological self-assessment tests (personality, anxiety, depression, burnout, relationships, IQ and more)…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://freudly.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
