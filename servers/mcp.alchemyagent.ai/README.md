# mcp.alchemyagent.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.alchemyagent.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.alchemyagent.ai/mcp` | 12 | [`c277db14212b`](1a01a7699d9657164c06.json) | 2026-11-27 |

## Tools at `https://mcp.alchemyagent.ai/mcp`

- `agent_readiness`: `Check how ready a site is for AI agents: llms.txt (validated against the llmstxt.org format, with broken-link check) and llms-full.txt, Mar…`
- `ai_crawler_check`: `Check whether AI and search crawlers (GPTBot, OAI-SearchBot, ChatGPT-User, ClaudeBot, PerplexityBot, Googlebot, Google-Extended, Bingbot, C…`
- `ai_render_check`: `Show what AI crawlers that don't run JavaScript (GPTBot, ClaudeBot, PerplexityBot, CCBot) actually see on a page: readable words in the raw…`
- `authority_check`: `Compare up to 10 domains (a site and its competitors) by Tranco popularity rank (top 1M sites). A free stand-in for domain authority. Uses…`
- `cwv_trend`: `Show how a site's real-user Core Web Vitals (LCP, INP, CLS, FCP, TTFB) changed over the last ~40 weeks, from the Chrome UX Report History A…`
- `data_connections`: `Explain how to connect the user's own Google Search Console, GA4 and Bing Webmaster Tools data to AlchemyAgent. This free connector has no…`
- `entity_check`: `Check how a brand appears in Wikidata, the open knowledge base that Google's Knowledge Graph and AI assistants draw brand facts from. Finds…`
- `gsc_query_classifier`: `Classify a Google Search Console queries export to find AI-assistant traffic: conversational prompts, follow-up pivots, AI-visibility track…`
- `pagespeed_check`: `Run Google PageSpeed Insights on a public URL. Returns real-user Core Web Vitals (LCP, INP, CLS from the Chrome UX Report), the Lighthouse…`
- `schema_check`: `Check a page's JSON-LD structured data against Google's rich-result requirements for common types (Organization, LocalBusiness, Product, Ar…`
- `security_headers`: `Grade a site's security headers with Mozilla HTTP Observatory and list exactly which headers are missing or weak (HSTS, Content-Security-Po…`
- `wikipedia_presence`: `Find Wikipedia articles (in the 10 largest language editions) that link to a domain, and the brand's own Wikipedia article page views over…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.alchemyagent.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
