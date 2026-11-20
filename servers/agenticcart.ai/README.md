# agenticcart.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/agenticcart.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://agenticcart.ai/mcp` | 5 | [`93de7d3c5dd1`](d13e47321fee0fdc800c.json) | 2026-11-20 |

## Tools at `https://agenticcart.ai/mcp`

- `check_acp_feed`: `Grade a product feed against the Agentic Commerce Protocol (ACP) / OpenAI product feed specification, which governs whether a catalog can b…`
- `check_llms_txt`: `Fetch a website's /llms.txt and check it against the llmstxt.org format: the H1 title, the summary block, the link sections, whether the li…`
- `check_merchant_feed`: `Validate a product feed against the Google Merchant Center product specification. Takes the feed URL (XML or JSON) and returns a 0-100 scor…`
- `check_product`: `Audit a single product page for how well AI shopping assistants can read and recommend it. Takes the product page URL and returns a 0-100 s…`
- `check_store_readiness`: `Audit any public online store for AI and agent readiness. Takes the store homepage URL and returns a 0-100 score with concrete findings: wh…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://agenticcart.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
