# mcp.airshelf.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.airshelf.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.airshelf.ai/mcp` | 8 | [`029bb8f16ee3`](bcd6b8dd84c17aeab22b.json) | 2026-11-02 |

## Tools at `https://mcp.airshelf.ai/mcp`

- `compare_products`: `Compare 2-10 catalog products side-by-side on their datasheet specs. Slugs come from search_catalog and are case-insensitive and dash-toler…`
- `explain_product`: `Explain the evidence behind a catalog row. Returns stored processing stages when available and always returns a golden-record field summary…`
- `find_products`: `Discover candidate products for a buyer need. Takes a need in natural language (e.g. "best value home espresso machine", market "TH"), Unle…`
- `get_product`: `Get the full golden record (AirShelf's verified product record) and latest price for one catalog product by slug ("<manufacturer>-<model>")…`
- `list_merchants`: `List public AirShelf merchants that have an assigned slug and at least one active product. Every listed merchant has an account with AirShe…`
- `request_quote`: `Send a quote request for catalog products to a merchant's sales team on behalf of a named buyer. This is a two-step, double opt-in flow. Th…`
- `research_shopping`: `research_shopping is the full verified-research job; find_products is the quick candidate-list tool. It runs as a background job and return…`
- `search_catalog`: `Search the AirShelf cross-vendor product catalog by natural-language query. The catalog covers industrial-automation, wiring-devices, digit…`

## Changes

- 2026-11-02: [description changed](../../deltas/2026-11-02/bcd6b8dd84c17aeab22b.json): `5 field(s) changed`
- 2026-10-24: [description changed, schema changed](../../deltas/2026-10-24/bcd6b8dd84c17aeab22b.json): `2 field(s) changed`
- 2026-10-06: [schema changed](../../deltas/2026-10-06/bcd6b8dd84c17aeab22b.json): `7 field(s) changed; signals: length_more_than_doubled`
- 2026-09-24: [description changed, schema changed](../../deltas/2026-09-24/bcd6b8dd84c17aeab22b.json): `103 field(s) changed; signals: imperative_language_introduced` **(notable)**
- 2026-09-22: [schema changed](../../deltas/2026-09-22/bcd6b8dd84c17aeab22b.json): `2 field(s) changed`
- 2026-09-08: [description changed](../../deltas/2026-09-08/bcd6b8dd84c17aeab22b.json): `2 field(s) changed; signals: length_more_than_doubled`
- 2026-08-23: [annotation changed, schema changed](../../deltas/2026-08-23/bcd6b8dd84c17aeab22b.json): `14 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.airshelf.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
