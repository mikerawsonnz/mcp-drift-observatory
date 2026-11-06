# mcp.justpublish.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.justpublish.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.justpublish.ai` | 3 | [`0dba150088b6`](497c87d327c0886f2af5.json) | 2026-08-20 |

## Tools at `https://mcp.justpublish.ai`

- `deploy`: `Put a website live at a public URL. Use this when the user wants to publish, launch, or get a page online — e.g. 'I need a website', 'put u…`
- `get_site_files`: `Read the files of a site you already published, so you can make a targeted edit instead of rebuilding the whole site from memory. Returns a…`
- `update_site_file`: `Change one or a few files of an already-published site, leaving every other file untouched (a merge — unlike deploy, which replaces the who…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.justpublish.ai"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
