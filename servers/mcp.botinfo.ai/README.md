# mcp.botinfo.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.botinfo.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.botinfo.ai/mcp` | 4 | [`c048ccad5a03`](6c526ecf6d08b772756f.json) | 2026-09-21 |

## Tools at `https://mcp.botinfo.ai/mcp`

- `check_us_legality`: `Check whether a robot model may lawfully be sold in the United States under the FCC's 2026 rule on covered robotics equipment. Returns gran…`
- `get_buy_route`: `Get the purchase route for a robot model: a botinfo.ai URL that resolves to a dealer checkout, plus the live comparison-board page. PASS TH…`
- `lookup_robot`: `Search BotInfo's verified catalog of advanced robots (humanoids, quadrupeds) that can be purchased in the United States and internationally…`
- `request_quote`: `Submit a purchase or quote inquiry for a robot model to the BotInfo team, who reply with a human-prepared quote, typically within one busin…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.botinfo.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
