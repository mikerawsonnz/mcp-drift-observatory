# signals.boolsai.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/signals.boolsai.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://signals.boolsai.ai/mcp` | 12 | [`b0302306bdb2`](de30941bb61d4d084485.json) | 2026-08-20 |

## Tools at `https://signals.boolsai.ai/mcp`

- `domain_timeline`: `Week-by-week wayback diff timeline for one domain. Returns every detected stack change (additions / removals) with week date. Use this to s…`
- `event_dossier`: `Deep dive on a single event: full diff (added/removed values), surrounding price action (-3D to +14D), predicted vs actual α, links to wayb…`
- `farm_domain`: `Bulk-farm a domain's historical wayback snapshots into our index. Use this when you need backtest history on a domain we haven't already fa…`
- `find_signals`: `Automated pattern discovery — scans event_type × detector × diff_field × severity combinations and returns those with the strongest forward…`
- `recent_events`: `Live signal feed: events fired in the last N days (default 7). Returns each event with the predicted α range based on its event type's hist…`
- `scan_at_date`: `Scan a URL as it appeared on a historical date via the Wayback Machine. Uses intel.boolsai.ai against the wayback-wrapped URL. Returns the…`
- `signal_diff`: `Compare two signal patterns side-by-side. e.g. 'how does PRICING_TIERS_ADDED compare to VENDORS_DETECTED_CHANGED on the live dataset?' Retu…`
- `signal_landscape`: `ONE-SHOT cross-signal sweep. Computes α-vs-SPY stats simultaneously across event_type, detector, diff_field, severity, AND co_occurrence di…`
- `test_filter`: `Compute α stats for an arbitrary filter expression. Use this to test a specific hypothesis (e.g. 'tier_count_changed on enterprise-SaaS tic…`
- `ticker_history`: `All events fired on a single ticker, plus price action timeline. Use this to investigate one company's pattern (e.g. 'show me everything we…`
- `universe_summary`: `Orient the agent: total events, tickers, date range, top event types, top detectors, price coverage, SPY benchmark status. Call this FIRST…`
- `wayback_backtest`: `Run an SPY-benchmarked backtest on the WAYBACK historical event dataset (2+ years, 13K events) instead of the recent live event dataset (2…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://signals.boolsai.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
