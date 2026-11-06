# celestio.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/celestio.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://celestio.ai/mcp` | 7 | [`18effaa8abad`](5a10e65fdbb6102578c7.json) | 2026-11-06 |

## Tools at `https://celestio.ai/mcp`

- `compare_birth_charts`: `Compatibility between two people (partners, crushes, friends, family) from their names, birth dates, places and, if known, times. No accoun…`
- `compute_birth_chart`: `Calculates a birth chart (planets, signs, houses, rising sign, aspects) for anyone from their name, birth date, place and, if known, time.…`
- `get_birth_reading`: `Writes (or returns the already written) free personal birth chart reading for someone, saved in the connected Celestio account. Pass person…`
- `get_reading`: `Returns one reading from the connected Celestio account by readingId: its sections and a link to it on celestio.ai. Status "writing" means…`
- `list_my_readings`: `Lists the readings saved in the connected Celestio account, newest first (birth readings and compatibility reports and Transit reports with…`
- `preview_compatibility`: `Free compatibility preview for two people: saves both charts in the connected Celestio account and returns the strongest connections betwee…`
- `preview_transits`: `Calculates a free personal 30-day Transit preview for exactly one chartId OR person (birth details). Requires createReadings and may save a…`

## Changes

- 2026-11-06: [schema changed](../../deltas/2026-11-06/5a10e65fdbb6102578c7.json): `14 field(s) changed`
- 2026-10-27: [schema changed](../../deltas/2026-10-27/5a10e65fdbb6102578c7.json): `96 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://celestio.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
