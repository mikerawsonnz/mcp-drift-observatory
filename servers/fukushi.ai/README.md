# fukushi.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/fukushi.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://fukushi.ai/api/mcp` | 2 | [`98e9ba380940`](0bcf4c325cc520a3b5c1.json) | 2026-09-18 |

## Tools at `https://fukushi.ai/api/mcp`

- `get_article`: `fukushi.ai の公開記事を slug で指定して全文（Markdown）を取得する。search_articles の抜粋では手順や表の全体が掴めないときに使う。本文末の脚注に、その記事が根拠にした一次情報の出典が示されている。`
- `search_articles`: `障害福祉制度の解説サイト「障害福祉AI辞典」(fukushi.ai) の記事を検索し、該当箇所の抜粋と記事URLを返す。記事は厚生労働省の一次情報（報酬告示・留意事項通知・指定基準省令・サービスコード表）に接地して検証済みで、本文には出典が脚注として示されている。障害者総合支援…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://fukushi.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
