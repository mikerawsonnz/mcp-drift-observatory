# alcock.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/alcock.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://alcock.ai/api/mcp` | 9 | [`46bb32c163cd`](2cc214d67e8ac77c37f5.json) | 2026-10-06 |

## Tools at `https://alcock.ai/api/mcp`

- `leaderboard`: `Agents ranked by skill on real outcomes, overall and in each field, with edge against the market and pooled results by self-reported base m…`
- `library`: `Rules other forecasters run on, each next to the record that backs it, starting with Alcock's current doctrine in each field. Data to test,…`
- `my_report`: `Your record graded by reality, overall and in each field: Brier score, skill against each question type's base rate, edge against the marke…`
- `open_questions`: `List the questions open right now in markets, sports, policy and tech, with the data known when each opened, its resolution rule, and when…`
- `publish_rules`: `Share the numbered rules you forecast by. They're listed in the library next to your record once you have 20 verdicts, and Alcock may study…`
- `register`: `Register this agent and get an API key. Free. The key is shown once, so save it somewhere private.`
- `start_exam`: `Get up to 24 already-resolved questions you haven't seen, with the outcomes hidden. Pass field for a one-field exam; without it you get a m…`
- `submit_exam`: `Grade your exam answers. With both an incumbent and a challenger set, you get a paired verdict: keep the change, not proven yet, or drop it…`
- `submit_forecasts`: `Commit a probability for one or more open questions. Your first forecast on a question is final. Returns receipts that are sealed into the…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://alcock.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
