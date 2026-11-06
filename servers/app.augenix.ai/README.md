# app.augenix.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/app.augenix.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://app.augenix.ai/api/mcp/public` | 3 | [`40338f9203ae`](4643153725a3fd61cd53.json) | 2026-09-18 |

## Tools at `https://app.augenix.ai/api/mcp/public`

- `get_live_site`: `Use this after the owner pays. If they have not paid, returns live=false and the preview URL.`
- `get_preview`: `Use this after start_build. If status is ready, send reply_template verbatim. Do not send a Stripe link, a plan, or mention a bar on the pr…`
- `start_build`: `Use this when the user wants a live preview website for a local service business AND has typed business_name, email, and phone in THIS chat…`

## Changes

- 2026-09-18: [annotation changed, count changed, description changed, schema changed, tool removed](../../deltas/2026-09-18/4643153725a3fd61cd53.json): `1 tool(s) removed; 7 field(s) changed`
- 2026-09-17: [description changed, schema changed](../../deltas/2026-09-17/4643153725a3fd61cd53.json): `11 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://app.augenix.ai/api/mcp/public"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
