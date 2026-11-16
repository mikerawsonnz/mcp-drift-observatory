# aeoengine.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/aeoengine.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://aeoengine.ai/mcp` | 4 | [`ab40a7b301c8`](b4551d53f9e6ab4923f1.json) | 2026-11-16 |

## Tools at `https://aeoengine.ai/mcp`

- `get_aeo_report_status`: `Poll a previously submitted AEO report job once. status is queued, preparing, needs_review or running (keep polling) or complete, partial o…`
- `run_aeo_report`: `Run the free AI-visibility report for a website (ChatGPT, Perplexity, Gemini, Claude coverage, competitor gaps, prioritized fixes). Require…`
- `site_audit_get`: `Read a site audit started with site_audit_start. format json (the default) returns the status and the report JSON. format md returns the Ma…`
- `site_audit_start`: `Start a site audit for one public page. Returns audit_id; poll it with site_audit_get. Requires an agency key (the same key as run_aeo_repo…`

## Changes

- 2026-11-16: [count changed, tool added](../../deltas/2026-11-16/b4551d53f9e6ab4923f1.json): `2 tool(s) added`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://aeoengine.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
