# mcp-server-295985738387.europe-west1.run.app: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp-server-295985738387.europe-west1.run.app.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp-server-295985738387.europe-west1.run.app/mcp` | 20 | [`015ec24721a8`](42e14eb37709960271b1.json) | 2026-08-20 |

## Tools at `https://mcp-server-295985738387.europe-west1.run.app/mcp`

- `bank_accounts`: `Retrieves bank account details and recent transaction history via a connected bank API integration. Returns a list of transactions for the…`
- `crypto_fx_rates`: `Converts an amount between any cryptocurrency and fiat currency pair, or between two cryptocurrencies, using real-time exchange rates sourc…`
- `crypto_price`: `Retrieves real-time price data for any cryptocurrency listed on CoinGecko. Returns the current price in any fiat currency, 24-hour percenta…`
- `crypto_price_lite`: `Retrieves the current spot price and 24-hour change for any cryptocurrency using the CoinGecko public API. Returns price, percentage change…`
- `currency_convert`: `Converts a monetary amount from one currency to another using live exchange rates sourced from the Frankfurter API (European Central Bank d…`
- `currency_convert_lite`: `Converts a monetary amount between any two fiat currencies using live exchange rates from the Frankfurter API (European Central Bank data).…`
- `currency_convert_open`: `Converts a monetary amount between two fiat currencies using live exchange rates from an open currency exchange API. Returns the converted…`
- `currency_fx_lite`: `Converts a foreign exchange (FX) amount between two fiat currencies using live mid-market rates. Returns the converted amount and the excha…`
- `currency_rates`: `Retrieves live and historical fiat currency exchange rates from the Frankfurter API (sourced from the European Central Bank). Supports both…`
- `financial_calculator`: `Performs precise financial calculations across six calculation types entirely locally with no external API dependency. compound_interest co…`
- `financial_calculator_lite`: `Performs common financial calculations locally with no external API dependency. Supports compound interest, loan repayment, return on inves…`
- `finnhub_stock_quote`: `Retrieves real-time stock price quotes and company information for any publicly traded company via the Finnhub API. Returns current price,…`
- `open_banking_transactions`: `Retrieves bank account balances and transaction history via PSD2 Open Banking (TrueLayer), covering 300+ UK and European banks. Returns the…`
- `platform_tool_finder`: `Discovers the most relevant tools available on this MCP server for a given task using local semantic search (MiniLM-L6-v2 embeddings). Acce…`
- `stock_price_lite`: `Retrieves the current trading price for a publicly listed stock by ticker symbol. Returns the current price as a single numeric value. This…`
- `stripe_payment_records`: `Retrieves payment and charge records from a Stripe merchant account. Returns a list of payment records filtered by the requested query type…`
- `stripe_payments`: `Retrieves live payment data from a Stripe account via the Stripe API. Supports four query types: recent_payments returns the latest payment…`
- `timezone_convert`: `Converts time between timezones. Useful for time conversion tasks. Use when you need to convert 3:45 PM EST to Pacific Time for a meeting s…`
- `web_news_headlines`: `Retrieves the latest real-time news headlines and article summaries from BBC News and The Guardian across nine topic categories. Returns st…`
- `web_url_reader`: `Fetches any public web page and returns clean, readable plain text stripped of HTML, navigation, scripts, advertisements, and boilerplate.…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp-server-295985738387.europe-west1.run.app/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
