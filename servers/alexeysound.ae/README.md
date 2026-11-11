# alexeysound.ae: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/alexeysound.ae.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://alexeysound.ae/agent.php` | 3 | [`68bbb68aa825`](db4a249681730aaf931f.json) | 2026-11-11 |

## Tools at `https://alexeysound.ae/agent.php`

- `check_availability`: `Availability is not published. Returns how to ask for given dates.`
- `get_info`: `Everything about Alexey Sound, a production sound mixer / location sound recordist in Dubai: services, price (from AED 2,500/day), kit, FAQ…`
- `request_booking`: `Send a booking request to Alexey for the client. It is NOT a confirmation: Alexey replies to the client personally. Ask the client for ever…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://alexeysound.ae/agent.php"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
