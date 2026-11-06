# mcp.fiber.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.fiber.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.fiber.ai/mcp` | 5 | [`864c7af05441`](16c7807df4f90053d88b.json) | 2026-08-20 |
| `https://mcp.fiber.ai/mcp/v2` | 10 | [`01a49a3b42e3`](6ddd71b3397bcf894c1d.json) | 2026-09-03 |

## Tools at `https://mcp.fiber.ai/mcp`

- `call_operation`: `Execute any Fiber API operation by operationId. IMPORTANT: - Most operations require 'apiKey' in the request body. - Prefer search_endpoint…`
- `get_endpoint_details_full`: `Get COMPLETE schema and details for a specific API operation. Use this BEFORE calling an API to understand exactly what parameters are need…`
- `list_all_endpoints`: `List available Fiber API endpoints with optional tag/search filtering.`
- `list_tag_packs`: `List curated tag packs for large tool catalogs. Use this to narrow exploration (for example social-media or enrichment).`
- `search_endpoints`: `Canonical API selection tool for endpoint discovery and ranking. Use this first to get the top recommended operations for a user intent. Su…`

## Tools at `https://mcp.fiber.ai/mcp/v2`

- `cardsAttach_tool`: `OperationId: cardsAttach. Attach card to trial account. USE THIS WHEN: - Attach card to trial account. - Attach a payment card to a cardles…`
- `companyLiveEnrich_tool`: `OperationId: companyLiveEnrich. Live fetch LinkedIn company. USE THIS WHEN: - Live fetch LinkedIn company. - Returns an enriched company wi…`
- `companySearch_tool`: `OperationId: companySearch. Company search. USE THIS WHEN: - Company search. - Search for companies using filters. - Find matching entities…`
- `getAllApiKeys_tool`: `OperationId: getAllApiKeys. List API keys. USE THIS WHEN: - List API keys. - List all API keys for your organization, including each key's…`
- `getAutoTopupSettings_tool`: `OperationId: getAutoTopupSettings. Get auto top-up settings. USE THIS WHEN: - Get auto top-up settings. - Get the organization's auto top-u…`
- `getOrgCredits_tool`: `OperationId: getOrgCredits. Get organization credits. USE THIS WHEN: - Get organization credits. - Get credits for an organization. - Inspe…`
- `getQuickstartScript_tool`: `OperationId: getQuickstartScript. Get quickstart install script. USE THIS WHEN: - Get quickstart install script. - Returns a bash script th…`
- `getRateLimits_tool`: `OperationId: getRateLimits. Get organization rate limits. USE THIS WHEN: - Get organization rate limits. - Returns the effective rate limit…`
- `peopleSearch_tool`: `OperationId: peopleSearch. People search. USE THIS WHEN: - People search. - Search for people using filters. - Find matching entities with…`
- `profileLiveEnrich_tool`: `OperationId: profileLiveEnrich. Live fetch LinkedIn profile. USE THIS WHEN: - Live fetch LinkedIn profile. - Returns an enriched profile wi…`

## Changes

- 2026-09-03: [description changed, schema changed](../../deltas/2026-09-03/6ddd71b3397bcf894c1d.json): `3 field(s) changed; signals: url_introduced`
- 2026-08-22: [tool added, tool removed](../../deltas/2026-08-22/6ddd71b3397bcf894c1d.json): `1 tool(s) added; 1 tool(s) removed; signals: credential_shaped_string_introduced, url_introduced` **(notable)**

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.fiber.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
