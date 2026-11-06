# advisorsai.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/advisorsai.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://advisorsai.ai/mcp` | 5 | [`3e5ddde0d7db`](528242ffe9b9a056287e.json) | 2026-10-15 |
| `https://advisorsai.ai/store-readiness-mcp` | 1 | [`92d8bde324f8`](d75b451c7d299bd2fa03.json) | 2026-08-25 |

## Tools at `https://advisorsai.ai/mcp`

- `advisors_catalog_get_service`: `Use after a service is identified and the user needs its published scope, limits, commercial packages, sample, and terms. Does not determin…`
- `advisors_catalog_list_services`: `Use when a user asks what Advisors AI offers. Returns exactly five public services; do not use it to infer fit or to create an order.`
- `advisors_catalog_match_service`: `Use when the user describes a business need but has not chosen a service. Returns at most two deterministic routing suggestions; it is not…`
- `advisors_order_prepare_link`: `Use only after the user explicitly selects a package returned by the service tool. Returns the ordinary login/request link; it does not cre…`
- `advisors_site_check_basics`: `Use only when a user asks to inspect a public website. Measures bounded page, robots, structured-data, sitemap, and experimental llms.txt s…`

## Tools at `https://advisorsai.ai/store-readiness-mcp`

- `advisors_store_readiness_check`: `Use only after the requester supplies a public page and asks for a read-only check. Returns at most one measured finding with a server-auth…`

## Changes

- 2026-10-15: [schema changed](../../deltas/2026-10-15/528242ffe9b9a056287e.json): `20 field(s) changed`
- 2026-08-25: [description changed, schema changed](../../deltas/2026-08-25/d75b451c7d299bd2fa03.json): `49 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://advisorsai.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
