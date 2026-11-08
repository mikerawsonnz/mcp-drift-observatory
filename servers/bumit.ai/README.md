# bumit.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/bumit.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://bumit.ai/mcp` | 3 | [`d13b49291793`](d0fe06dca65feccd4008.json) | 2026-11-08 |

## Tools at `https://bumit.ai/mcp`

- `get_company_profile`: `Retrieve the canonical Swiss commercial-register (Zefix) profile for one company by UID: legal name, legal form, register status, seat, can…`
- `search_companies`: `Search the Swiss commercial register (Zefix) by company name and receive bounded, deduplicated candidate summaries (UID, legal name, legal…`
- `verify_business`: `Verify a Swiss company using official commercial-register data (Zefix), SECO sanctions data, and FINMA authorisation data. Search by UID or…`

## Changes

- 2026-11-08: [count changed, tool added](../../deltas/2026-11-08/d0fe06dca65feccd4008.json): `2 tool(s) added`
- 2026-10-26: [description changed, schema changed](../../deltas/2026-10-26/d0fe06dca65feccd4008.json): `9 field(s) changed; signals: length_more_than_doubled`
- 2026-10-23: [description changed](../../deltas/2026-10-23/d0fe06dca65feccd4008.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://bumit.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
