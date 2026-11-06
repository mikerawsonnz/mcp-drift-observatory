# property.bluebed.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/property.bluebed.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://property.bluebed.ai/mcp` | 11 | [`61989e35fba7`](e7c3f93ddafd851a0a0d.json) | 2026-11-04 |

## Tools at `https://property.bluebed.ai/mcp`

- `about`: `Says who runs this service, the agent's CEA registration and agency licence, how the service is paid for, and how to reach the agent.`
- `book_call`: `Booking a call through your assistant is not open yet. Calling this holds nothing and takes no details: it returns a WhatsApp link to the a…`
- `cancel_booking`: `Booking a call through your assistant is not open yet. Calling this holds nothing and takes no details: it returns a WhatsApp link to the a…`
- `check_booking`: `Booking a call through your assistant is not open yet. Calling this holds nothing and takes no details: it returns a WhatsApp link to the a…`
- `confirm_booking`: `Booking a call through your assistant is not open yet. Calling this holds nothing and takes no details: it returns a WhatsApp link to the a…`
- `get_area`: `Returns the reviewed area details of a launch by slug: address, tenure, nearby amenities with straight-line distances, schools within two k…`
- `get_launch`: `Returns one launch by slug: its property type (condo or ec, which adds a notice on executive condominiums), its reviewed facts with source…`
- `get_unit_type`: `Returns one unit type of a launch by slug and type name: size, bathrooms, powder rooms and WCs, stacks (stacks_note explains an asterisk),…`
- `list_launches`: `Lists the new launches this service covers: name, property type (condo or ec, an executive condominium), district, street, number of units,…`
- `rules_for_buyer`: `Quotes the Singapore property rules that apply to a buyer, exactly as published, with the authority, source link, effective date and the da…`
- `search_floor_plans`: `Searches floor plans across the reviewed launches, a selection during the trial. Filter by property type (condo or ec), bedrooms, size in s…`

## Changes

- 2026-11-04: [description changed, schema changed](../../deltas/2026-11-04/e7c3f93ddafd851a0a0d.json): `10 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://property.bluebed.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
