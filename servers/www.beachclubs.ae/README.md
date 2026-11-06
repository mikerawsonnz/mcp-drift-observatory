# www.beachclubs.ae: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/www.beachclubs.ae.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://www.beachclubs.ae/mcp` | 4 | [`d19ddeb141a6`](342c8a5bf0901ef67c50.json) | 2026-11-05 |

## Tools at `https://www.beachclubs.ae/mcp`

- `get_beach_club`: `Returns public details for one beach club in the United Arab Emirates, looked up by id or by name (typo tolerant): BeachClubs.ae page and p…`
- `list_events`: `Lists published upcoming events at beach clubs in the United Arab Emirates (brunches, ladies' days, parties, live music) with Dubai local t…`
- `request_booking_enquiry`: `Sends a booking enquiry for a beach club in the United Arab Emirates to the BeachClubs.ae team, who reply to the guest by email. An enquiry…`
- `search_beach_clubs`: `Searches the BeachClubs.ae directory of beach clubs in the United Arab Emirates by name, hotel, area, emirate, family suitability, amenitie…`

## Changes

- 2026-11-05: [schema changed](../../deltas/2026-11-05/342c8a5bf0901ef67c50.json): `1 field(s) changed`
- 2026-10-24: [annotation changed, count changed, description changed, schema changed, tool added](../../deltas/2026-10-24/342c8a5bf0901ef67c50.json): `1 tool(s) added; 233 field(s) changed; signals: length_more_than_doubled, url_introduced`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://www.beachclubs.ae/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
