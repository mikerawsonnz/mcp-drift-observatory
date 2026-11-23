# avioverse.aero: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/avioverse.aero.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://avioverse.aero/mcp` | 5 | [`471d34ab782a`](48ecc3ac830d366c3cdb.json) | 2026-11-23 |

## Tools at `https://avioverse.aero/mcp`

- `fetch`: `Return the full text of one library page as Markdown. 'id' is the 'id' (site path) or 'url' of a result from 'search'.`
- `get_rule`: `Return an EASA rule by its reference (for example 145.A.30(e), CAMO.A.305, ORO.GEN.200, FCL.010) with its text, AMC and GM, the regulation,…`
- `list_regulations`: `List the EASA regulations in the library with their official reference, the EAR revision date the text reproduces, and the 'regulation' val…`
- `lookup_term`: `Return how EASA defines a term, quoted verbatim with the regulation and article it comes from, plus the entry from the general aviation glo…`
- `search`: `Search EASA rules, EASA definitions, implementation guides, articles and the Metis manual by reference or by words. Returns matching pages…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://avioverse.aero/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
