# moonlings.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/moonlings.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://moonlings.ai/api/mcp` | 8 | [`31de97dbcdbc`](e1c9a180ad5de8ea2b32.json) | 2026-08-20 |

## Tools at `https://moonlings.ai/api/mcp`

- `check_facts`: `Find what AI assistants get WRONG about a local business. Asks ChatGPT and Perplexity live (with web search) about the business's hours, ad…`
- `check_report_status`: `Poll a deep research report by slug. Free. Returns status (generating / ready / failed); a failed report triggers the automatic refund of i…`
- `check_visibility`: `Ask ChatGPT and Perplexity live (with web search) who they'd recommend in a business's category and city, and report whether THIS business…`
- `get_report_result`: `Fetch a completed deep research report by slug. Free. Returns the long-form report (markdown), a structured-findings JSON block, the action…`
- `ping`: `Returns server status, the price list, and (when authenticated) your credit balance. Free — call it to check connectivity and see what this…`
- `review_gap`: `Compare a local business's Google rating and review count against the top same-category rivals nearby, with the gap math done: who leads, t…`
- `run_scan`: `A live competitor scan: a research agent finds the business's strongest same-category rival nearby and scouts it (offer, pricing signals, r…`
- `start_deep_report`: `Launch a full overnight-grade research report on a local business: an autonomous research crew maps the competitive landscape, reads the bu…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://moonlings.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
