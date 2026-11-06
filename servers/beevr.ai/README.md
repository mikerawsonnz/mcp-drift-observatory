# beevr.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/beevr.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://beevr.ai/mcp` | 8 | [`42cecbf9ff80`](794715dba82a6cd13760.json) | 2026-10-07 |

## Tools at `https://beevr.ai/mcp`

- `about_beevr`: `Who BeevR is, its AI capabilities (production agents, HIPAA AI, GraphRAG, Kite framework) and how to contact the team.`
- `get_article`: `Get one BeevR blog article as Markdown, by slug (from list_articles or search_beevr).`
- `get_case_study`: `Get the full write-up of one BeevR case study as Markdown, by slug (from list_case_studies).`
- `get_pricing`: `Get BeevR fixed-price packages (Pitch Demo, Investor MVP, Flagship Sprint) with price, duration and what is included.`
- `list_articles`: `List BeevR blog articles (newest first), optionally filtered by a keyword query.`
- `list_case_studies`: `List production systems BeevR has shipped (healthcare AI, security agent, AI B2B matchmaking, fintech payments, manufacturing) with key res…`
- `list_services`: `List BeevR services (AI agent development, AI development, MVP development, HIPAA and fintech MVPs, custom software, offshore development i…`
- `search_beevr`: `Search BeevR services, shipped case studies and articles (AI agents, MVP cost, HIPAA/PCI compliance, offshore development in Vietnam). Retu…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://beevr.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
