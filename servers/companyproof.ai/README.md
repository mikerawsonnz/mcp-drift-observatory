# companyproof.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/companyproof.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://companyproof.ai/v2/mcp` | 3 | [`ca1f93ee4033`](bf591ba60eea8d598f74.json) | 2026-10-07 |

## Tools at `https://companyproof.ai/v2/mcp`

- `get_company_profile`: `Retrieve a CompanyProof company profile and enrichment payload by the opaque company ID returned from search_companies. This read-only oper…`
- `search_companies`: `Find ranked CompanyProof company matches by name, registration number, VAT/tax identifier or ticker, optionally narrowed by subdivision and…`
- `verify_company_claims`: `Resolve a company, compare supported claims with current company evidence, preserve a proof record, and optionally monitor verified claims…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://companyproof.ai/v2/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
