# app.deepvalues.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/app.deepvalues.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://app.deepvalues.ai/api/mcp` | 25 | [`a8c78eb88594`](ddb6e3dcdf15351bd1ec.json) | 2026-10-10 |

## Tools at `https://app.deepvalues.ai/api/mcp`

- `account`: `Returns the calling key, its scopes, environment, and today's usage across all 3 buckets. Self-billing: counts as 1 metadata call. (GET htt…`
- `ai_context`: `Returns a system prompt + structured context block, scoped to one ticker. Drop it into OpenAI/Anthropic/any LLM SDK to ground your chatbot…`
- `companies_search`: `Company search (GET https://app.deepvalues.ai/api/v1/companies — 0.001 credits per call; works with no credentials up to 25 call(s)/day per…`
- `company_overview`: `Company overview (GET https://app.deepvalues.ai/api/v1/companies/{ticker}/overview — 0.001 credits per call; works with no credentials up t…`
- `credits_checkout`: `Creates a one-time Stripe Checkout Session for a credit pack, bound to the calling live key’s account. When the payment completes the credi…`
- `credits_packs`: `Lists the prepaid credit packs this key can buy (1 credit = $1.00). Free. (GET https://app.deepvalues.ai/api/v1/credits/checkout — free; ne…`
- `filings`: `SEC filings (10-K, 10-Q, 8-K, etc) (GET https://app.deepvalues.ai/api/v1/filings/{ticker} — 0.001 credits per call; works with no credentia…`
- `fundamentals`: `Income + balance + cashflow (GET https://app.deepvalues.ai/api/v1/fundamentals/{ticker} — 0.001 credits per call; works with no credentials…`
- `guru`: `One guru: bio + top holdings (GET https://app.deepvalues.ai/api/v1/gurus/{slug} — 0.005 credits per call; works with no credentials up to 2…`
- `guru_moves`: `The Follow the Pros feed. Every material 13F move — new position, full exit, a share count that moved by 25%, or a position of $100M or mor…`
- `guru_portfolio`: `One guru's full portfolio at a quarter (GET https://app.deepvalues.ai/api/v1/gurus/{slug}/portfolio — 0.005 credits per call; works with no…`
- `gurus`: `60 hand-picked institutional investors — every name a serious value investor would recognize. Filter by style. (GET https://app.deepvalues.…`
- `indicators_buffett`: `US corporate equities ÷ GDP, with zones (significantly undervalued through significantly overvalued) and historical percentile. (GET https:…`
- `indicators_shiller_pe`: `Shiller PE with historical percentile (GET https://app.deepvalues.ai/api/v1/indicators/shiller-pe — 0.001 credits per call; works with no c…`
- `intrinsic_value`: `DCF + Owner Earnings + Damodaran intrinsic value (GET https://app.deepvalues.ai/api/v1/intrinsic-value/{ticker} — 0.005 credits per call; w…`
- `keys_me`: `Returns the calling key, the exact balance of the ledger behind it (balanceMicro: integer micro-credits, 1 credit = $1.00 = 1,000,000), wha…`
- `mirror_brief`: `The same move as /verdict, flattened into a brief: what the investor did, when, at what price, against our value band, plus the verdict sen…`
- `news`: `Sentiment-scored news (GET https://app.deepvalues.ai/api/v1/news/{ticker} — 0.001 credits per call; works with no credentials up to 25 call…`
- `research`: `The differentiated endpoint: full briefing, bull case, bear case, valuation, investment plan, fair-value range. Bills against your ai_resea…`
- `sentiment`: `Value-investor sentiment rollup (not WSB noise) (GET https://app.deepvalues.ai/api/v1/sentiment/{ticker} — 0.001 credits per call; works wi…`
- `smart_money_changes`: `All 13F position changes meeting the materiality threshold (new positions, full exits, ≥25% share-count shifts, OR ≥$100M position size) ac…`
- `smart_money_holdings`: `Returns every guru from our 60-name roster who held the requested ticker as of the latest 13F-HR quarter (or a specific historical quarter)…`
- `theses`: `Public investment theses with structured metadata — sentiment, conviction, price target, anchored DVI run. Filter by ticker, conviction, or…`
- `verdict`: `One guru's disclosed move in one ticker, with the sentence Deep Values publishes about it and every number behind it: the company's legal n…`
- `webhooks_list`: `List webhook subscriptions (GET https://app.deepvalues.ai/api/v1/webhooks — free; needs a connected account or a dv_sk_ key)`

## Changes

- 2026-10-10: [description changed](../../deltas/2026-10-10/ddb6e3dcdf15351bd1ec.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://app.deepvalues.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
