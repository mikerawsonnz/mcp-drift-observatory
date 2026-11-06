# dynamicfeed.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/dynamicfeed.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://dynamicfeed.ai/mcp` | 94 | [`926644e49af2`](8b77937413ae91f87c33.json) | 2026-08-20 |

## Tools at `https://dynamicfeed.ai/mcp`

- `ai_models`: `Current & trending AI MODELS from the open-model ecosystem (Hugging Face) — name, org, task, popularity (likes/downloads) and release date.…`
- `ai_provider_latency`: `Measured latency & uptime for each major AI provider's API (OpenAI, Anthropic, Google, Mistral, Groq, DeepSeek, xAI) — Dynamic Feed's own m…`
- `air_quality`: `Current air quality for a city or lat/lon — PM2.5, PM10, US & European AQI, ozone, NO2, with a category (Good/Moderate/Unhealthy...). Use f…`
- `air_quality_fusion`: `Cross-validated air quality — TWO independent networks reading the same sky: the Open-Meteo CAMS model (the existing air_quality source) vs…`
- `airport_delays`: `Live FAA airport delays, ground stops, closures & ground-delay programs (US NAS, keyless). 'airport' = 3-letter code (LGA, LAX…) or blank f…`
- `au_economy`: `Official AUSTRALIAN economic indicators from the Australian Bureau of Statistics Data API (SDMX) — STATISTICS ONLY, NO prices. 'indicator'…`
- `au_water`: `Australian river heights + gauge rainfall near any AU location — live CC-BY-licensed gauge observations from the Bureau of Meteorology's Wa…`
- `aviation_weather`: `Live aviation weather — decoded METAR observations + TAF forecasts for any ICAO airport (NOAA Aviation Weather Center, public domain, keyle…`
- `bitcoin_network`: `Live Bitcoin NETWORK telemetry — infrastructure metrics only, NO price data. 'metric' = "overview" (default, full digest) / "fees" (recomme…`
- `carbon_intensity`: `Great Britain grid carbon intensity right now (gCO2/kWh + index) + the live fuel mix + the cleanest upcoming half-hour from the 24h forecas…`
- `cert_check`: `Live TLS/SSL certificate check for any domain — measured by a direct handshake RIGHT NOW: issuer, validity window, days to expiry, expiring…`
- `check_vulnerability`: `Is this exact package (and version) vulnerable? FULL historical lookup across the entire OSV.dev corpus (Google) — every matching advisory…`
- `china_data`: `Returns current World Bank macro series for China, including GDP, growth, CPI, trade, M2, unemployment, and FDI, with source and observatio…`
- `cite`: `Get a fresh, CITEABLE source + timestamp for a current datapoint — so you can cite it, not guess. Pass ANY tool, source, or topic (earthqua…`
- `climate_enso`: `Current EL NIÑO / LA NIÑA state — latest ONI anomaly + phase, official episode check, recent seasons, and NOAA CPC's alert-system status (e…`
- `clinical_trials`: `Live clinical-trial registrations and status updates from ClinicalTrials.gov (US NIH/NLM registry). Returns the most-recently-updated trial…`
- `company_lookup`: `Resolve a company name (or exact 20-char LEI) to its authoritative global Legal Entity Identifier + canonical legal name, address, status a…`
- `convert`: `Convert an amount between currencies at the LIVE rate (not a stale training-era rate). CURRENTLY LIVE: fiat (USD/EUR/GBP/JPY/CNY/AUD/...).…`
- `countdown`: `Time until a LIVE event you can't compute without a clock: a market open/close (NYSE, NASDAQ, LSE, TSE, HKEX, SSE, ASX, XETRA) or the next…`
- `current_time`: `The current date & time anywhere — an LLM has no internal clock, so use this instead of guessing "today" or "now". tz is an IANA timezone (…`
- `current_weather`: `Current weather anywhere — by city name or lat/lon. Returns temperature, feels-like, wind, humidity, precipitation and conditions, live. Us…`
- `detect_drift`: `DRIFT DETECTION — audit a batch of AI-stated facts against live ground-truth in one call. Pass 'claims' (a list of statements an LLM produc…`
- `dns_lookup`: `Live DNS records for a domain via Cloudflare DNS-over-HTTPS (keyless): A / AAAA / MX / TXT / NS / CNAME / SOA / CAA. Resolve a domain to wh…`
- `drought`: `US drought severity — % of area in each D0-D4 class by week (U.S. Drought Monitor, keyless). 'area' = 'total' (US national) or a state FIPS…`
- `drug_shortages`: `US drug shortages from the FDA (openFDA, keyless). 'query' = drug/generic name (amoxicillin…) or blank for the most recently updated. Is dr…`
- `earthquakes`: `Recent earthquakes worldwide from USGS — magnitude, depth, location, PAGER impact alert (green→ red, distinct from raw magnitude), tsunami…`
- `econ_calendar`: `What is SCHEDULED to move markets — upcoming US Treasury auctions (type, term, size, date) and FOMC meeting dates incl. the next meeting. P…`
- `emissions`: `National greenhouse-gas emissions for a country (ISO-3 code, e.g. USA/CHN/IND) + year, from Climate TRACE (CC BY 4.0, keyless): CO2/CH4/N2O…`
- `energy_grid`: `Live US electricity grid data by region/operator (US EIA, public domain). region = US48 (national) or a grid operator: CAISO · PJM · MISO ·…`
- `ephemeris`: `Solar & lunar timing for a place + day — sunrise/sunset, the full twilight set (civil/nautical/ astronomical), moonrise/moonset, moon phase…`
- `exploited_vulnerabilities`: `Vulnerabilities CONFIRMED exploited in the wild — the CISA Known Exploited Vulnerabilities (KEV) catalog, each enriched with its EPSS explo…`
- `fda_recalls`: `Recent FDA-regulated RECALLS & enforcement actions via openFDA — regulatory facts, NO prices. 'category' = "drug" (default) / "food" / "dev…`
- `federal_register`: `Recent US Federal Register documents — rules, proposed rules, notices, executive orders (keyless). 'doc_type' = RULE / PRORULE / NOTICE / P…`
- `flood_forecast`: `5-day river-discharge FORECAST near an Australian location — Copernicus CEMS Global Flood Awareness System (GloFAS, operational LISFLOOD co…`
- `github_releases`: `Latest releases for a GitHub repo (owner/name) — version, date, author, link — via the public releases atom feed (keyless, no rate limit).…`
- `global_disasters`: `Active worldwide disaster alerts (GDACS) — ONE cross-hazard feed across earthquakes, tropical cyclones, floods, droughts and volcanoes, eac…`
- `global_indicator`: `A flagship development statistic from Our World in Data: the latest value for a country plus a short multi-year trend, with full source att…`
- `global_macro`: `Worldwide macro indicators for ANY country (World Bank Open Data, CC-BY). country = an ISO code (US, GB, DE, IN, BR, JP, CN, ZA…) or name.…`
- `gov_contracts`: `US federal contract & assistance awards from USAspending.gov (keyless, US public domain). Who was awarded what, by which agency, for how mu…`
- `gps_interference`: `Probable GPS/GNSS interference (jamming/spoofing) over an area, MEASURED from live ADS-B navigation integrity (the GPSJam method) — unique…`
- `grid_carbon`: `Live grid carbon intensity (gCO2/kWh): current value, trend vs ~3 hours ago, and the live generation mix by fuel. 'region' = "au" (Australi…`
- `hacker_news`: `Live Hacker News stories (keyless) — the tech/AI attention layer right now. kind = top / new / best; optional case-insensitive title filter…`
- `health_surveillance`: `US public-health surveillance signals from the CDC — the current level + week-over-week direction of circulating illness, not individual ca…`
- `hurricanes`: `Active tropical cyclones from the NOAA National Hurricane Center (NHC) — tropical depressions, tropical storms, and hurricanes. Per storm:…`
- `interest_rates`: `Live US benchmark interest rates — Effective Fed Funds Rate, SOFR, OBFR, etc. from the New York Fed. Use instead of guessing the current Fe…`
- `internet_outages`: `Live BGP routing health for a network resource — an ASN (e.g. "AS3215"), an IP ("8.8.8.8"), or a prefix ("193.0.0.0/22") — from RIPEstat (R…`
- `lightning_network`: `Bitcoin LIGHTNING NETWORK aggregate statistics — network infrastructure metrics only, NO price data. Returns node count, public channel cou…`
- `live_flights`: `Live aircraft positions right now — real-time flight tracking from open ADS-B (adsb.lol, CC0). Answers "what's flying over X?" and "where i…`
- `marine_forecast`: `Marine / surf forecast for a coastal point — current sea state + next-24-hour outlook. Returns total significant wave height / period / dir…`
- `market_hours`: `Returns current open/closed status and next open/close times for major exchanges, crypto (24/7), and forex (24/5). Appropriate when a user…`
- `natural_events`: `Active natural events worldwide from NASA EONET — wildfires, severe storms (hurricanes/typhoons), volcanoes, floods, sea/lake ice. Use for…`
- `ocean_buoys`: `Live marine observations from NOAA NDBC ocean buoys — significant wave height & period, wave direction, wind speed/direction/gust, barometr…`
- `orbital_data_centers`: `DATA CENTERS IN SPACE — curated registry of compute/AI spacecraft in orbit (Starcloud's NVIDIA H100 GPU, ESA Φsat-2 AI edge, D-Orbit in-orb…`
- `ots_calendar_health`: `Live health of the public OpenTimestamps (OTS) timestamp-anchoring calendar servers — the aggregation-and-anchoring infrastructure behind t…`
- `package_health`: `Health & security posture of a software package (npm / PyPI / Go / Maven / Cargo / NuGet / RubyGems) from deps.dev (Google Open Source Insi…`
- `pollen_forecast`: `Airborne pollen / allergen forecast — six pollen types (alder, birch, grass, mugwort, olive, ragweed) in grains/m³, each with a plain-Engli…`
- `product_recalls`: `US product recalls — food, drug & medical-device enforcement reports (openFDA, keyless, CC0). 'category' = all / food / drug / device; 'que…`
- `public_holidays`: `Public / statutory holidays for a country (and optional state/province/region) in a given year — computed in-house, NOT scraped, so it's ex…`
- `reality_check`: `Fact-check a statement against LIVE data — the anti-hallucination tool. Pass any claim about the current world ("the latest Python is 3.12"…`
- `research_papers`: `Latest scholarly preprints from arXiv — newest-first — by category and/or keyword. Returns up to 15 papers, each with: title, authors, trun…`
- and 34 more in [8b77937413ae91f87c33.json](8b77937413ae91f87c33.json)

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://dynamicfeed.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
