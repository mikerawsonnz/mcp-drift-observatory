# awardcast.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/awardcast.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://awardcast.ai/mcp` | 8 | [`191d066782f5`](f9898ec52cacb5cd2fb9.json) | 2026-08-20 |

## Tools at `https://awardcast.ai/mcp`

- `agency_profile`: `Buying profile of a US federal agency: how many contracts it awards, how much it obligates, what share is competed, the typical price per N…`
- `contractor_profile`: `Federal award history of a contractor: how many contracts it has won, total obligated, median win value, which agencies it sells to, its re…`
- `fetch`: `Open the full record behind an id returned by search: an agency profile with price by category and its top winners, a contractor's award hi…`
- `open_solicitations`: `US federal solicitations OPEN right now, from SAM.gov, each with the buying agency, the NAICS code and the place of performance. Call this…`
- `price_band`: `Historical closing-price range for an agency and NAICS category pair: the 10th percentile, median and 90th percentile of contracts already…`
- `search`: `Search AwardCast's US federal contracting record: buying agencies, federal contractors, and solicitations open right now. Call this first f…`
- `track_record`: `Accuracy scorecard for AwardCast's forecasts, scored against the real contract value once FPDS publishes it. Call this when the user asks w…`
- `upcoming_recompetes`: `US federal contracts nearing expiry that are likely to be recompeted, i.e. opportunities BEFORE they become a published solicitation. Each…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://awardcast.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
