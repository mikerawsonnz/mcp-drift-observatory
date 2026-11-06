# mcp.normhyra.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.normhyra.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.normhyra.ai` | 5 | [`80572b3e750b`](e7e1a6cbb10257c02572.json) | 2026-08-28 |

## Tools at `https://mcp.normhyra.ai`

- `calculate_actual_rent`: `Räkna om en normhyra (kr/m²/år) till faktisk årshyra i kronor för en given lägenhetstyp, yta och eventuella korrigeringspoäng. Returnerar å…`
- `calculate_normhyra`: `Räkna om en faktisk hyra till normhyra (kr/m²/år) för referenslägenheten 3 rok, 77 m². Hyran kan anges som årshyra (yearlyRent) ELLER månad…`
- `calculate_rent_roll`: `Konvertera en hel hyreslista (flera lägenheter) till normhyra i ett anrop. Varje lägenhet räknas om till normhyra (kr/m²/år) för norm -78,…`
- `export_rent_roll_pdf`: `Konvertera en hyreslista till normhyra OCH generera en PDF-sammanställning – samma layout som PDF-exporten på normhyra.ai (liggande A4, tab…`
- `list_apartment_types`: `Returnera alla lägenhetstyper som normhyra.ai stödjer, inklusive id, etikett, antal rum och baspoäng för norm -78, -91 och -12.`

## Changes

- 2026-08-28: [description changed, schema changed](../../deltas/2026-08-28/e7e1a6cbb10257c02572.json): `12 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.normhyra.ai"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
