# events.aero: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/events.aero.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://events.aero/mcp/events` | 5 | [`20963c3b870e`](0ab3287c5fc33c6e22e5.json) | 2026-10-11 |

## Tools at `https://events.aero/mcp/events`

- `featured-events`: `The events Events.Aero is featuring right now, the same selection as the lead row of the home page, optionally for one country. Each includ…`
- `get-event`: `Get one public event by its sqid or slug (from search-events or featured-events): dates, venue, price, how to book or RSVP, organiser conta…`
- `list-countries`: `The countries Events.Aero lists events in, with the code to pass to other tools and each country's public home and events pages.`
- `list-event-types`: `The kinds of aviation event on Events.Aero (airshow, fly-in, workshop and so on), with the value to pass to search-events and the public pa…`
- `search-events`: `Search upcoming public aviation events on Events.Aero (airshows, fly-ins, workshops and more). Filter by free text, event type, country, da…`

## Changes

- 2026-10-11: [schema changed](../../deltas/2026-10-11/0ab3287c5fc33c6e22e5.json): `4 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://events.aero/mcp/events"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
