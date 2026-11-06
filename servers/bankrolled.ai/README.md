# bankrolled.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/bankrolled.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://bankrolled.ai/mcp` | 5 | [`cb171d8ae69d`](5cc2518d652f586b7ba6.json) | 2026-10-29 |

## Tools at `https://bankrolled.ai/mcp`

- `cross_border_check`: `Answer cross-border money questions: deposit protection for non-residents, which schemes cover accounts held across borders. Returns source…`
- `health_check`: `Liveness check. Returns ok and version. Free, no key.`
- `money_fact`: `Get an official, dated personal-finance limit: deposit insurance (FDIC, FSCS, CDIC, AU FCS, NZ DCS) or contribution limits and allowances (…`
- `pricing_list`: `List everything this server covers: every money_fact fact_key with an example question, and every scheme_lookup country. Free (nothing on t…`
- `scheme_lookup`: `Identify a country's deposit-insurance scheme and its headline coverage (US FDIC, UK FSCS, CA CDIC, AU FCS, NZ DCS) with the regulator's UR…`

## Changes

- 2026-10-29: [annotation changed, field changed](../../deltas/2026-10-29/5cc2518d652f586b7ba6.json): `10 field(s) changed`
- 2026-10-24: [count changed, tool added](../../deltas/2026-10-24/5cc2518d652f586b7ba6.json): `1 tool(s) added`
- 2026-10-20: [description changed, schema changed](../../deltas/2026-10-20/5cc2518d652f586b7ba6.json): `5 field(s) changed`
- 2026-10-15: [description changed, schema changed](../../deltas/2026-10-15/5cc2518d652f586b7ba6.json): `41 field(s) changed; signals: imperative_language_introduced` **(notable)**

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://bankrolled.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
