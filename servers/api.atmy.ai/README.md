# api.atmy.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.atmy.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.atmy.ai/mcp` | 12 | [`67e215fb5694`](5f23f4a4f55342a166a0.json) | 2026-11-14 |

## Tools at `https://api.atmy.ai/mcp`

- `find_sensors`: `Single sensors with their latest reading (PM1, PM2.5, PM10, temperature, humidity, pressure), network and quality check: status, rating 0–1…`
- `get_air_quality`: `PM2.5 now in a city (mean of the latest reading of each eligible sensor, at most 60 minutes old; a government station hour up to 3 hours ol…`
- `get_air_quality_history`: `Daily PM2.5 of a city from the Atmy Data Hub (UTC days, sensors after the quality check) with the day's weather from 2026-01-19 (mean, lowe…`
- `get_air_quality_monthly`: `The whole measurement history of a city from the Atmy Data Hub: PM2.5 per month with the month's weather from 2026-01, yearly means (comple…`
- `get_city_forecast`: `The next hours of a city: temperature, wind, humidity, precipitation and the pollution accumulation index 0–100 (how strongly the weather k…`
- `get_country_ranking`: `Cities of a country ranked by daily PM2.5 for the last completed day (Atmy Data Hub), most polluted or cleanest first.`
- `get_home_environment`: `Greenery and emission sources around a point (a home): tree canopy share within 300 m, green land share and summer NDVI within 500 m with a…`
- `get_sensor`: `One sensor by its id: location, network, license, quality check with rating and reasons, and the latest reading.`
- `get_sensor_readings`: `Readings of one sensor: raw (the last 31 days, at most 7 days a call), 5-minute means (the same windows), hourly means (the last 366 days,…`
- `get_sensors_average`: `The mean of up to 100 sensors per 5 minutes, hour or UTC day, each sensor counted once per bucket, with the number of sensors in each bucke…`
- `list_sensor_networks`: `The sensor networks in Atmy (Sensor.Community, AirGradient, Atmy, and government stations of official networks) with their number of sensor…`
- `search_cities`: `Find the cities with an Atmy air-quality summary by name (any language) or country. Returns slugs to pass to the other tools.`

## Changes

- 2026-11-14: [count changed, tool added](../../deltas/2026-11-14/5f23f4a4f55342a166a0.json): `1 tool(s) added`
- 2026-11-09: [description changed, schema changed](../../deltas/2026-11-09/5f23f4a4f55342a166a0.json): `2 field(s) changed`
- 2026-11-07: [description changed](../../deltas/2026-11-07/5f23f4a4f55342a166a0.json): `1 field(s) changed`
- 2026-11-01: [schema changed](../../deltas/2026-11-01/5f23f4a4f55342a166a0.json): `1 field(s) changed`
- 2026-10-28: [count changed, tool added](../../deltas/2026-10-28/5f23f4a4f55342a166a0.json): `5 tool(s) added`
- 2026-10-25: [count changed, description changed, schema changed, tool added](../../deltas/2026-10-25/5f23f4a4f55342a166a0.json): `1 tool(s) added; 9 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.atmy.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
