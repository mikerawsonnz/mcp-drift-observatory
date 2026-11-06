# scan.agenticplug.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/scan.agenticplug.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://scan.agenticplug.ai/mcp` | 2 | [`f13d7ca92d9f`](9401a81874daab05fd72.json) | 2026-10-10 |

## Tools at `https://scan.agenticplug.ai/mcp`

- `explain_check`: `Explain one agent-readiness check in depth: what it is, why it matters for AI agents and AI search, exactly how the scanner tests it, what…`
- `scan_website`: `Scan a public website and report how ready it is for AI agents and AI search: which checks pass, which are missing, and what each check is,…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://scan.agenticplug.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
