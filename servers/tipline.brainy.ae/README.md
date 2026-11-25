# tipline.brainy.ae: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/tipline.brainy.ae.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://tipline.brainy.ae/mcp` | 6 | [`1ed85c1b3663`](ada4fe2bb40413d8a9b6.json) | 2026-11-25 |

## Tools at `https://tipline.brainy.ae/mcp`

- `get_gta6_cheats`: `Confirmed Grand Theft Auto VI story-mode cheat codes: name, how to unlock it, and the D-pad sequence (PS5 and Xbox Series X/S), with the so…`
- `get_gta6_entry`: `Get the full text (markdown) of one Tipline entry by id, with its sources.`
- `get_gta6_safe_codes`: `Known Grand Theft Auto VI safe combinations: code, location and how to find it, each with its entry URL and sources.`
- `gta6_release_times`: `When Grand Theft Auto VI unlocks in each country (UTC and local time), the rules behind it, and sources.`
- `list_gta6_entries`: `List Tipline entries (id, title, summary, url), optionally filtered by type.`
- `search_gta6_guide`: `Search Tipline's sourced notes about Grand Theft Auto VI (characters, places, vehicles, weapons, activities, systems, release info; mission…`

## Changes

- 2026-11-25: [count changed, tool added](../../deltas/2026-11-25/ada4fe2bb40413d8a9b6.json): `2 tool(s) added`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://tipline.brainy.ae/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
