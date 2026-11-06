# maxcv.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/maxcv.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://maxcv.ai/mcp` | 2 | [`e34c116a5329`](e09868b6c0094ff38665.json) | 2026-08-20 |

## Tools at `https://maxcv.ai/mcp`

- `score_cv`: `Score how well a CV/resume matches a specific job posting. Fast and cheap — returns the original match score and the score after tailoring,…`
- `tailor_cv`: `Tailor a CV/resume to a specific job posting: rewrites the CV with the posting's ATS keywords (never fabricating skills not already present…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://maxcv.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
