# www.edgechat.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/www.edgechat.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://www.edgechat.ai/mcp` | 5 | [`982bc84d381d`](f873093fd83495a35c76.json) | 2026-10-08 |

## Tools at `https://www.edgechat.ai/mcp`

- `connect`: `Find the shortest chain of in-text links from one Edgepedia article to another (at most 6 hops), with the sentence that makes each hop; pas…`
- `fetch`: `Read an encyclopedia article in full: one Edgepedia article as Markdown with its citations, by a 'search' result's id. Returns id, title, t…`
- `related`: `Find encyclopedia articles related to an Edgepedia article: its topic-mates, a few from each neighboring topic, and its geography neighbors…`
- `resolve`: `Find which encyclopedia article a name means: Edgepedia's best match for a person, place, thing, or concept named in a text, with a confide…`
- `search`: `Search an encyclopedia for facts about a person, place, thing, event, or concept: Edgepedia, over 300k articles with citations. Pass the su…`

## Changes

- 2026-10-08: [count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-10-08/f873093fd83495a35c76.json): `3 tool(s) added; 93 field(s) changed; signals: imperative_language_introduced, url_introduced` **(notable)**
- 2026-10-05: [description changed, schema changed](../../deltas/2026-10-05/f873093fd83495a35c76.json): `3 field(s) changed`
- 2026-09-30: [description changed, schema changed](../../deltas/2026-09-30/f873093fd83495a35c76.json): `6 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://www.edgechat.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
