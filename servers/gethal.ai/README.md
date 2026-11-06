# gethal.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/gethal.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://gethal.ai/mcp` | 7 | [`5710de51001b`](2556ed675e69d9cab919.json) | 2026-08-20 |

## Tools at `https://gethal.ai/mcp`

- `book_demo`: `Submits a demo request. The prospect receives a confirmation email and must click the link in it before the request reaches a human at A Cl…`
- `describe_hal`: `Explains how the HAL autonomous sales agent works: the six-stage pipeline (find → research → qualify → quality control → draft → send) and…`
- `get_company_info`: `Returns the company name, operator, contact email, homepage, and a short description of gethal.ai.`
- `get_customer_profile`: `Returns the target customer profile for gethal.ai (industries, team sizes, regions, representative use cases) and any public reference cust…`
- `get_features`: `Returns the six core features of gethal.ai with one-line descriptions.`
- `get_pricing`: `Returns the gethal.ai pricing plans (Solo, Team, Enterprise) with both monthly and yearly rates plus included features.`
- `get_use_cases`: `Returns representative B2B sales use cases (outbound prospecting, market expansion, partner-channel sales) with example prompts.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://gethal.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
