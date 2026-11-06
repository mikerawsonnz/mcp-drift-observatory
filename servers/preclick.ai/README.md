# preclick.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/preclick.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://preclick.ai/mcp` | 6 | [`37d1e402e4ff`](1a44b2e75208b490636a.json) | 2026-08-20 |

## Tools at `https://preclick.ai/mcp`

- `url_scanner_async_scan`: `Submit a URL for asynchronous security analysis. Returns immediately with a task_id. Poll with url_scanner_async_task_status to check progr…`
- `url_scanner_async_scan_with_intent`: `Submit a URL with optional user intent for asynchronous security analysis. Returns immediately with a task_id. Poll with url_scanner_async_…`
- `url_scanner_async_task_result`: `Retrieve the result of an asynchronous scan task. If completed, returns the full scan result (risk_score, confidence, agent_access_directiv…`
- `url_scanner_async_task_status`: `Check the status of an asynchronous scan task. Returns the current task status using native MCP task semantics (working, completed, failed,…`
- `url_scanner_scan`: `Analyze a URL for security threats (synchronous, blocks until complete or timeout). Returns risk score, confidence, agent access guidance,…`
- `url_scanner_scan_with_intent`: `Analyze a URL for security threats with optional user intent context (synchronous, blocks until complete or timeout). Returns risk score, c…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://preclick.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
