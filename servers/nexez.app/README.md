# nexez.app: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/nexez.app.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://nexez.app/mcp` | 5 | [`69207e51377e`](7b52bc128caafcb0213d.json) | 2026-08-26 |

## Tools at `https://nexez.app/mcp`

- `nexez_directory`: `Browse the cross-merchant Nexez directory (optionally filtered by category, query, minimum readiness, or location).`
- `nexez_get_page`: `Fetch a listing's full structured agent manifest (seller profile, offers, actions) by slug.`
- `nexez_search`: `Search across all Nexez merchants for services/products matching a buyer request. Returns ranked listings with offers + agent.json URLs.`
- `nexez_validate_checkout`: `Dry-run a checkout for an offer BEFORE paying - validates the offer, currency, and payment readiness. Never charges.`
- `nexez_validate_negotiation`: `Dry-run a negotiation proposal against the seller’s rules BEFORE submitting. Returns the rules evaluation. Never writes.`

## Changes

- 2026-08-26: [schema changed](../../deltas/2026-08-26/7b52bc128caafcb0213d.json): `4 field(s) changed`
- 2026-08-24: [description changed](../../deltas/2026-08-24/7b52bc128caafcb0213d.json): `1 field(s) changed`
- 2026-08-23: [schema changed](../../deltas/2026-08-23/7b52bc128caafcb0213d.json): `3 field(s) changed`
- 2026-08-22: [schema changed](../../deltas/2026-08-22/7b52bc128caafcb0213d.json): `4 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://nexez.app/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
