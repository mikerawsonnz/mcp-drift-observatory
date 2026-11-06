# api.odei.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.odei.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.odei.ai/mcp` | 7 | [`c8dfe3fe0988`](c8e87c72ac0a7848c91d.json) | 2026-08-20 |

## Tools at `https://api.odei.ai/mcp`

- `odei_connect_handshake`: `Verify an app.odei.ai pairing code and open an ODEI Connect session.`
- `odei_connect_plan`: `Return the ordered local ODEI install plan and reporting contract.`
- `odei_connect_report_step`: `Record evidence that a Connect ceremony step has completed.`
- `odei_connect_status`: `Return current ODEI Connect ceremony progress.`
- `odei_connect_talk`: `Answer from ODEI Connect session state without invoking a model API.`
- `wm_recall`: `Read facts back from your ODEI-hosted operator memory. Simple substring + recency match (v1) — no semantic search yet.`
- `wm_remember`: `Write one fact to your operator memory in ODEI — the World Model grows from it. Server-side (ODEI-hosted) memory for the paired operator; n…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.odei.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
