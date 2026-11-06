# creationloop.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/creationloop.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://creationloop.ai/api/mcp` | 4 | [`031f28dac7d9`](2babc902b804ee51dbc8.json) | 2026-08-20 |

## Tools at `https://creationloop.ai/api/mcp`

- `get_company_overview`: `What CreationLoop is, how an agent run becomes verified, exactly what the ledger proves, the registry, and the design-partner offer. Served…`
- `get_design_partner_offer`: `The current offer, which is the design partnership: what the ledger proves and how to apply. Served verbatim from the site's canonical copy.`
- `get_faq`: `Frequently asked questions about CreationLoop, with answers served verbatim from the site's canonical copy.`
- `submit_design_partner_application`: `Apply to become a CreationLoop design partner. Records the full application: email, website host, and any name, company, and message provid…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://creationloop.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
