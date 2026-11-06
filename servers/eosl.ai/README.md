# eosl.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/eosl.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://eosl.ai/mcp` | 5 | [`46bb3fd530ed`](499d47ab37c2d9f8d153.json) | 2026-09-10 |

## Tools at `https://eosl.ai/mcp`

- `bulk_check`: `Check up to 200 part numbers in one call (read-only, no auth; for a single part use lookup_part). Returns a per-part row (status, EOSL date…`
- `get_family`: `Fetch the full source-backed record for one product family by slug (from search_models or lookup_part pageUrl): lifecycle dates per SKU gro…`
- `list_vendors`: `List all vendors tracked by EOSL.ai with family counts and vendor page URLs. Read-only, no parameters. Use this first to check whether a ve…`
- `lookup_part`: `Look up one hardware part number or model name in the EOSL.ai database (read-only, no auth; for many parts use bulk_check). Returns support…`
- `search_models`: `Search tracked product families by vendor, product line, or series name (case-insensitive substring, e.g. "nexus 9300"). Read-only. Returns…`

## Changes

- 2026-09-10: [schema changed](../../deltas/2026-09-10/499d47ab37c2d9f8d153.json): `1 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://eosl.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
