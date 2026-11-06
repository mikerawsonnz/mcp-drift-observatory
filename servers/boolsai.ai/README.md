# boolsai.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/boolsai.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://boolsai.ai/mcp` | 2 | [`fa48e1ac16d5`](ddae8585e697a057ec7d.json) | 2026-08-20 |

## Tools at `https://boolsai.ai/mcp`

- `boolsai_scan`: `Scan a public website. Returns its full tech stack — every external host the page talks to, every fetch/xhr/beacon endpoint, every inline-s…`
- `boolsai_scan_paths`: `Scan multiple paths on the same site in parallel and merge the external-host lists. Returns per-path host lists, a unified merged set, and…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://boolsai.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
