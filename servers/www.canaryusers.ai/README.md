# www.canaryusers.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/www.canaryusers.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://www.canaryusers.ai/api/mcp` | 3 | [`712877eb9ed3`](4721c244195e2e540b69.json) | 2026-08-20 |

## Tools at `https://www.canaryusers.ai/api/mcp`

- `canary_scan`: `Run a CanaryUsers UX scan on a DEPLOYED URL (your live or preview app — not source code). A flock of AI personas evaluates the page and rep…`
- `get_report_markdown`: `Get one scan's full report as AI-ready markdown: the findings ranked by severity, why each matters, and how to fix it. Pass a scanId from l…`
- `list_recent_scans`: `List the most recent CanaryUsers UX scans for your account (id, URL, CanaryScore, grade, status, date). Use this to find a scan to dig into.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://www.canaryusers.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
