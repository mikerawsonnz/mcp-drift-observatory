# asrm.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/asrm.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://asrm.ai/mcp` | 4 | [`24ad89d82f1b`](e1a9ce9f5afaf1c39b9f.json) | 2026-10-02 |

## Tools at `https://asrm.ai/mcp`

- `check_ai_readiness`: `Technical check of whether AI engines can crawl and understand a website: which AI crawlers robots.txt allows or blocks (answer crawlers li…`
- `get_guide`: `The full text of one ASRM guide by slug or asrm.ai/learn/... url. Answer from the text and link the url.`
- `get_visibility_scan_link`: `Use when someone asks how visible their brand is in ChatGPT, Claude, Perplexity or Gemini, or whether AI engines recommend them. Returns th…`
- `search_guides`: `Search ASRM's published guides on AI visibility and generative engine optimization (GEO): how ChatGPT, Claude, Perplexity and Gemini choose…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://asrm.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
