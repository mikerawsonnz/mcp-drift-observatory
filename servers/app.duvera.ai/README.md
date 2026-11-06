# app.duvera.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/app.duvera.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://app.duvera.ai/mcp` | 52 | [`981b5eaeedf2`](00df3dd9874b4d8a29f0.json) | 2026-08-20 |

## Tools at `https://app.duvera.ai/mcp`

- `amazon__package_track`: `[amazon · risk:low] Look up the delivery status of an Amazon order (read-only)`
- `applehealth__heart_rate_read`: `[applehealth · risk:medium] Read heart-rate data from Apple Health`
- `applehealth__sleep_read`: `[applehealth · risk:medium] Read sleep-analysis data from Apple Health`
- `applehealth__steps_read`: `[applehealth · risk:medium] Read step-count data from Apple Health`
- `bluesky__trending_get`: `[bluesky · risk:low] Fetch the current trending topics on Bluesky. Returns topic names, display labels, and links to the topic feed. No acc…`
- `chase__balance_check`: `[chase · risk:low] Read the current balance of a Chase account (read-only)`
- `datadog__logs_view`: `[datadog · risk:low] Search and read logs from Datadog over a time range`
- `delta__boardingpass_show`: `[delta · risk:low] Pull up the boarding pass for a Delta flight`
- `duvera__dev_npm_package`: `[duvera · risk:low] Look up the latest version, description, license, and dependencies of an npm package. Works for scoped packages too (e.…`
- `duvera__dev_pypi_package`: `[duvera · risk:low] Look up the current version, summary, license, and homepage of a Python package on PyPI. No account required.`
- `duvera__dev_stackoverflow_search`: `[duvera · risk:low] Search Stack Overflow questions by keyword. Returns top 5 by relevance with title, link, score, and answer status. No a…`
- `duvera__finance_crypto_price`: `[duvera · risk:low] Current spot price for one or more cryptocurrencies (CoinGecko ids like "bitcoin,ethereum,solana") in a fiat currency (…`
- `duvera__finance_exchange_rates`: `[duvera · risk:low] Live USD exchange rates against major currencies. Read-only, no account required.`
- `duvera__food_recipe_search`: `[duvera · risk:low] Search recipes by dish name (e.g. "arrabiata", "pad thai"). Returns ingredients, instructions, category, and cuisine. N…`
- `duvera__food_restaurant_search`: `[duvera · risk:low] Search for restaurants and food places by name or location using OpenStreetMap. Read-only, no account required.`
- `duvera__geo_geocode`: `[duvera · risk:low] Convert a city or place name (e.g. "Berlin", "San Francisco") to latitude/longitude, country, timezone, and population.…`
- `duvera__github_latest_release`: `[duvera · risk:low] Get the latest published release (tag, name, notes, date) of a public GitHub repository. Returns 404 for repos that pub…`
- `duvera__github_read_file`: `[duvera · risk:low] Read a file from a public GitHub repository. Read-only.`
- `duvera__github_search_repos`: `[duvera · risk:low] Search public GitHub repositories by keyword. Returns top 5 results by stars. No auth required.`
- `duvera__news_search`: `[duvera · risk:low] Search Hacker News stories by keyword, ranked by relevance. Returns title, URL, points, author, and comment count. No a…`
- `duvera__news_top_stories`: `[duvera · risk:low] Top stories from Hacker News. Read-only, no account required.`
- `duvera__reference_dictionary`: `[duvera · risk:low] Definitions, phonetics, part of speech, and examples for an English word. No account required.`
- `duvera__reference_public_holidays`: `[duvera · risk:low] Public holidays for a given year and ISO country code (e.g. 2026 + "US"). Includes national and regional holidays with…`
- `duvera__time_now`: `[duvera · risk:low] Current date and time in an IANA timezone (e.g. "America/New_York", "Asia/Tokyo"). Includes day of week and DST status.…`
- `duvera__travel_flight_search`: `[duvera · risk:low] List aircraft currently airborne within a radius of a point (adsb.lol ADS-B data). Use geo.geocode to get a city's coor…`
- `duvera__weather_air_quality`: `[duvera · risk:low] Current air quality (US AQI, PM2.5, PM10, ozone) for a latitude/longitude. Use geo.geocode first if you only have a pla…`
- `duvera__weather_current`: `[duvera · risk:low] Current temperature, conditions, wind, and humidity for a latitude/longitude (Open-Meteo). Use geo.geocode first if you…`
- `duvera__wiki_search`: `[duvera · risk:low] Search Wikipedia articles by keyword. Returns matching page titles, keys, and excerpts. Pass a result's key to wiki.sum…`
- `duvera__wiki_summary`: `[duvera · risk:low] Get the lead summary of a Wikipedia article by title (e.g. "Zero_trust_architecture"). Use wiki.search first to find th…`
- `gmail__mail_read`: `[gmail · risk:low] Read recent emails from the Gmail inbox`
- `google_workspace__mail_search`: `[google-workspace · risk:low] Search Mail via Gmail, governed by Duvera.`
- `googlecalendar__availability_find`: `[googlecalendar · risk:low] Find open time slots within a date range in Google Calendar`
- `grubhub__order_track`: `[grubhub · risk:low] Check the live status and ETA of a Grubhub order`
- `hackernews__stories_top`: `[hackernews · risk:low] Fetch the current list of top-story ids on Hacker News. Returns an array of item ids (resolve details via the item…`
- `instacart__menu_search`: `[instacart · risk:low] Search for grocery items and stores in the Instacart app`
- `maps__eta_share`: `[maps · risk:low] Share your estimated time of arrival with a contact from Apple Maps`
- `microsoft365__calendar_list`: `[microsoft365 · risk:low] List Calendar via Outlook Calendar, governed by Duvera.`
- `microsoft365__mail_search`: `[microsoft365 · risk:low] Search Mail via Outlook / Exchange, governed by Duvera.`
- `notion__notes_search`: `[notion · risk:low] Search pages and notes in Notion by query`
- `obsidian__notes_search`: `[obsidian · risk:low] Search notes in an Obsidian vault by query`
- `open_meteo__weather_forecast`: `[open-meteo · risk:low] Current temperature, conditions, humidity, and wind for a latitude/longitude, from Open-Meteo.`
- `opensky__flights_live`: `[opensky · risk:low] List aircraft currently airborne within a latitude/longitude box, from OpenSky's live ADS-B feed.`
- `postgres__sql_read`: `[postgres · risk:low] Execute a read-only SQL query against a Postgres database`
- `shazam__audio_identify`: `[shazam · risk:low] Identify the song currently playing using Shazam`
- `slack__message_search`: `[slack · risk:low] Search recent messages across Slack channels`
- `southwest__flight_status`: `[southwest · risk:low] Check the status of a Southwest flight`
- `telegram__message_read`: `[telegram · risk:low] Read recent messages from a Telegram chat`
- `twitter__tweets_search`: `[twitter · risk:low] Search for recent tweets matching a keyword, hashtag, or phrase using the Twitter v2 API. Pass your Twitter Bearer Tok…`
- `uber__fare_estimate`: `[uber · risk:low] Estimate the fare for a trip in the Uber app`
- `united__flight_status`: `[united · risk:low] Check the status of a United flight`
- `venmo__payment_request`: `[venmo · risk:low] Request a payment from a contact via Venmo (no money leaves your account)`
- `wallet__boardingpass_show`: `[wallet · risk:low] Pull up a boarding pass stored in Apple Wallet`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://app.duvera.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
