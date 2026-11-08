# artemisgtm.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/artemisgtm.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://artemisgtm.ai/mcp` | 5 | [`0cd2ae062b5b`](05201622ddbc4614d3f7.json) | 2026-11-08 |

## Tools at `https://artemisgtm.ai/mcp`

- `book_evaluation`: `The evaluation booking link for Artemis GTM and what happens on the call: Tom Regan walks the motion, names the biggest leak visible from t…`
- `describe_firm`: `What Artemis GTM is: an AI GTM engineering firm for seed to Series C B2B startups, who founded it, what it builds, how it builds (its propr…`
- `get_resources`: `The free guides on artemisgtm.ai, by topic (speed to lead, lead scoring and handoff, visitor identification, ICP, outbound, data and report…`
- `list_systems`: `The GTM systems Artemis GTM builds inside a client's own CRM and tools, each with the problem it fixes, what gets built and the related fre…`
- `recommend_engagement`: `Given a B2B go-to-market problem in plain language (for example "leads sit for two days before anyone calls them", "most of our website tra…`

## Changes

- 2026-11-08: [description changed](../../deltas/2026-11-08/05201622ddbc4614d3f7.json): `2 field(s) changed; signals: url_introduced`
- 2026-11-07: [description changed](../../deltas/2026-11-07/05201622ddbc4614d3f7.json): `1 field(s) changed; signals: url_introduced`
- 2026-10-25: [tool added, tool removed](../../deltas/2026-10-25/05201622ddbc4614d3f7.json): `5 tool(s) added; 5 tool(s) removed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://artemisgtm.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
