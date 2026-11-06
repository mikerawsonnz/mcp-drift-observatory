# api.atako.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.atako.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.atako.ai/mcp/public` | 4 | [`f09baefbc975`](77558449d7b666a698fe.json) | 2026-10-28 |

## Tools at `https://api.atako.ai/mcp/public`

- `get_pricing`: `Returns Atako's public subscription plans (name, price, included credits/agents) and the credit conversion rate used for top-ups. No accoun…`
- `list_integration_pages`: `Lists Atako's public marketing pages describing each supported integration (what it does, why connect it). Marketing content without any ac…`
- `list_use_cases`: `Lists Atako's published customer use cases/case studies, optionally filtered by department (e.g. sales, support, engineering). Marketing co…`
- `report_outcome`: `Records how a request handled with Atako's tools ended (accomplished, partial or failed), a short summary, and what the user asked for that…`

## Changes

- 2026-10-28: [annotation changed, description changed, schema changed](../../deltas/2026-10-28/77558449d7b666a698fe.json): `13 field(s) changed`
- 2026-10-23: [count changed, schema changed, tool added](../../deltas/2026-10-23/77558449d7b666a698fe.json): `1 tool(s) added; 30 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.atako.ai/mcp/public"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
