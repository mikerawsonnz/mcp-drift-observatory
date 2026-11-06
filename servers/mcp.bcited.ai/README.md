# mcp.bcited.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.bcited.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.bcited.ai/public` | 6 | [`267795e4c6b9`](443aa011af344d4baaa1.json) | 2026-11-02 |

## Tools at `https://mcp.bcited.ai/public`

- `get_domain_readiness`: `Look up one domain on b/cited's public AEO readiness leaderboard: its rank, grade, overall and AEO scores in every category it appears in,…`
- `get_leaderboard`: `Return one category of b/cited's public AEO readiness leaderboard: every curated domain ranked by overall readiness score (0–100) with its…`
- `get_prompt_citations`: `For one leaderboard category, which sites ChatGPT, Claude and Perplexity cited when asked b/cited's fixed set of buyer prompts, for one ISO…`
- `list_leaderboard_categories`: `List the 12 industry categories of b/cited's public AEO readiness leaderboard (slug, name, description).`
- `lookup_glossary`: `Define a term the way b/cited's glossary defines it — AEO, citation, brand rank, visibility score, authority score, topical cluster, covera…`
- `scan_site`: `Run b/cited's Site Readiness scan on one public URL: a rule-based audit (not model-judged) of 30+ observable signals across nine categories…`

## Changes

- 2026-11-02: [annotation changed, description changed, schema changed](../../deltas/2026-11-02/443aa011af344d4baaa1.json): `13 field(s) changed`
- 2026-10-20: [description changed](../../deltas/2026-10-20/443aa011af344d4baaa1.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.bcited.ai/public"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
