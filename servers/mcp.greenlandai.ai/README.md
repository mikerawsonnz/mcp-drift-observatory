# mcp.greenlandai.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.greenlandai.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.greenlandai.ai/mcp` | 37 | [`6ff484a97acb`](5b0efbe1bdd6887ddbf2.json) | 2026-09-25 |

## Tools at `https://mcp.greenlandai.ai/mcp`

- `balance_proof`: `Cryptographic inclusion proof for YOUR wallet balance in the latest hourly transparency attestation (GET /wallet/balance-proof): leaf hash,…`
- `billing_attempts`: `YOUR OWN CHARGE RECORD — what this wallet was charged for, attempt by attempt, so you can verify your bill without asking us (relays GET /a…`
- `billing_quote`: `The exact per-caller price of a metered call BEFORE you make it — free, no website, an MCP tool you can actually invoke (relays GET /api/v1…`
- `bridge_proof`: `Cryptographic inclusion proofs for YOUR Bridge Ledger rows — contribution/fee events — in the balance-proof shape (GET /programme/bridge/pr…`
- `company`: `One company's record and graph neighbourhood by id; the response carries 'charged_joules' — the all-in PRICE of THIS call (one key on every…`
- `contribute_receipts`: `Your OWN append-only contribution receipts (forward your enabled gai_ key as X-API-Key) — the proof of what you submitted, with the canonic…`
- `contribute_relations`: `Submit evidenced graph relationships to the GreenlandAI contributor door (TEN programme). Auth: your OWN GreenlandAI key in X-API-Key — an…`
- `contribute_stats`: `Your OWN contributor standing (forward your enabled gai_ key as X-API-Key; the door derives identity from the key). Returns totals (submitt…`
- `contribute_submissions`: `Your OWN per-item submission outcomes (forward your enabled gai_ key as X-API-Key). Each item: id, kind, name, outcome (pending_review / ac…`
- `deposit`: `One resource deposit's record by numeric id (relays GET /api/v1/deposits/{id}), including its 'commodities[]' ({name, role: primary/byprodu…`
- `deposit_status`: `YOUR OWN USDC-on-Base deposit state (relays GET /api/v1/wallet/deposit-status; own wallet only, derived from your credential, never a param…`
- `deposits`: `Search resource deposits (relays GET /api/v1/deposits). Filters: 'commodity', 'resource_type', 'country', 'status', 'owner_country', 'max_p…`
- `funding_prepare`: `The in-band funding step for a joule shortfall — NEVER a website to visit (operator lock). USDC on Base is the live agent-fundable rail: de…`
- `hops`: `DEPRECATED alias for 'relationships' — kept working, to be removed at a future major. Use 'relationships'. Reason (operator ruling 2026-09-…`
- `joules_balance`: `Your own wallet balance — a FREE read either way (checking costs nothing). A GreenlandAI AGENT key ('gai_'/'gqa_') reads its OWN wallet via…`
- `joules_deficit`: `Given a planned 'cost', read a balance and return {needed, have, shortfall, tool_to_call_next} so an agent can decide in-band whether it ca…`
- `ledger_verify`: `Recent public ledger anchors with their on-chain transaction ids and the exact credit supply at each anchor — public, no auth. Independentl…`
- `look_at`: `Satellite still of a place — a Sentinel-2 ARCHIVE image (the screen as a picture). Pose = lat/lng OR entity_type+id (anchor); same pose fam…`
- `look_from`: `Map lane: pins near a point (lat/lng + radius_km). 'entity_type' (deposit / infrastructure / company / project) behaves two ways (backend,…`
- `map_viewport`: `Map lane: everything inside a bounding box — THE SCREEN (relays GET /api/v1/map.viewport). Typed params: min_lat/min_lng/max_lat/max_lng (t…`
- `mapdata`: `CLOSED — do NOT call. '/api/v1/mapdata' (the bulk map-layers surface) is TEMPORARILY closed to ALL callers, agent AND human: the backend re…`
- `market_accept`: `Accept a delivery on a match (POST /match/{id}/accept) — releases escrow to the provider. You must be the buyer party; backend enforces it.`
- `market_listings`: `Browse the RAREEAI marketplace: kind="providers" (listings) or "oracles". Typed query params for the providers browse (GET /providers): fro…`
- `market_match`: `Read one marketplace match by id, including its 'escrow_terms' and this trade's typed fee/timeout fields. You must be a party to the match.…`
- `market_provide`: `Create/update a marketplace listing (POST /provide). Requires marketplace:write (verified account) — an unverified/under-scoped token gets…`
- `market_quote`: `Read one marketplace REQUEST by id (GET /request/{id}; you must own it). Returns the request as the route actually declares it: id, wallet_…`
- `market_request`: `Post a marketplace BUY request (POST /request) — you want to buy a resource; providers match against it and your escrow is debited on match…`
- `nearby`: `Entities near a location (the primitive 'look_from' builds on). Typed query params (GET /nearby): lat + lng (required), radius_km (default…`
- `oracle_assess`: `Post your verdict on a delivery you were assigned (POST /oracle/assess/{match_id}). Body: {verdict ('valid' or 'invalid'), quality_score (a…`
- `oracle_assignments`: `List YOUR oracle assignments — the deliveries you have been assigned to assess (GET /oracle/assignments). The backend scopes this to your o…`
- `oracle_deregister`: `Deregister as an oracle and unstake (POST /oracle/deregister?wallet_id=...). Returns your staked joules from escrow (less any amount alread…`
- `oracle_register`: `Register as a RAREEAI oracle by staking joules (POST /oracle/register). INVITE-ONLY at launch (Phase 1 — the oracle pool is operator-run):…`
- `relationships`: `Graph lane: labelled relationship EDGES between companies/entities (ownership, operates, supplies, …) — the PRODUCT (edges with tiers + pro…`
- `trade_settlement`: `YOUR OWN trade's settlement — every leg of a marketplace trade you were the BUYER or SELLER of (relays GET /api/v1/wallet/trade/{match_id}/…`
- `transparency_latest`: `The latest hourly PUBLIC transparency attestation (GET /transparency/latest — no auth): a Merkle root over every wallet balance, the verifi…`
- `verify_proof`: `Look up one identifier (chunk_id, proof_id, match_id, transfer id, or a BSV txid) in ENYAL's public verify lookup — no auth. The backend's…`
- `wallet_transfer`: `Direct wallet-to-wallet transfer (POST /wallet/transfer). Requires wallet:transfer scope. WHO CAN SEND (the backend as it runs, 2026-09-03)…`

## Changes

- 2026-09-25: [description changed, schema changed](../../deltas/2026-09-25/5b0efbe1bdd6887ddbf2.json): `11 field(s) changed; signals: length_more_than_doubled, url_introduced`
- 2026-09-24: [description changed, schema changed](../../deltas/2026-09-24/5b0efbe1bdd6887ddbf2.json): `18 field(s) changed`
- 2026-09-23: [count changed, description changed, schema changed, tool added](../../deltas/2026-09-23/5b0efbe1bdd6887ddbf2.json): `4 tool(s) added; 10 field(s) changed; signals: length_more_than_doubled`
- 2026-09-21: [count changed, description changed, schema changed, tool added](../../deltas/2026-09-21/5b0efbe1bdd6887ddbf2.json): `1 tool(s) added; 388 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.greenlandai.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
