# mcp.helixar.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.helixar.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.helixar.ai/mcp` | 2 | [`4791f87507c6`](9f5f44afd0f7e032ba3e.json) | 2026-08-20 |

## Tools at `https://mcp.helixar.ai/mcp`

- `helixar_hdp_validate`: `Validate an HDP delegation chain against IETF draft-helixar-hdp-agentic-delegation-00. Surfaces scope escalations, depth violations, expire…`
- `helixar_inspect_mcp`: `Scan an MCP server (URL or raw manifest JSON) against Helixar's Sentinel detection rules. Returns risk score, findings, and a Claude-genera…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.helixar.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
