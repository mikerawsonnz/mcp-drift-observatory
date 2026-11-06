# councilof.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/councilof.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://councilof.ai/mcp/free` | 14 | [`2f12c471e26f`](646cc9386b69a5727a2b.json) | 2026-10-08 |
| `https://councilof.ai/mcp` | 19 | [`2389b7c430d2`](72b229b0a72f686b6a58.json) | 2026-10-15 |

## Tools at `https://councilof.ai/mcp/free`

- `board_totals`: `Live GSPC board totals from https://councilof.ai/api/gspc. Returns the slot count and the measured count as two labelled numbers WITH their…`
- `evidence_bundle_preview`: `For ONE obligation (article-50, article-53 GPAI transparency, dora or cra) and an optional subject: the obligation record, its counsel-gate…`
- `get_axis`: `One axis row from the live GSPC board at https://councilof.ai/api/gspc — every axis the board carries, behavioural and financial families a…`
- `get_card`: `GET one public-root card-v0 leaf by sha256 (64 hex) from https://councilof.ai/cards/{sha16}.json. UNMEASURED cells stay visible. States: VA…`
- `get_root`: `GET the permissionless public-root at https://councilof.ai/root.json. Returns merkle_root, card_count, as_of, and UNMEASURED notes. Separat…`
- `list_cards`: `The published signed-card index (https://councilof.ai/signed/card_index.json): what the index declares (n_cards) and how many rows it actua…`
- `mcp_trust`: `GET the latest MCP handshake trust snapshot (https://councilof.ai/interop/mcp-trust/latest.json): counts of how many internet-facing MCP se…`
- `measurement_index`: `Read the latest signed measurement-capsule index published at https://councilof.ai/measurement-capsules/latest.json: the index root over ev…`
- `route`: `GSPC Route (free, decide-only). Applies YOUR policy and the fixed GSPC floor to a candidate set and returns the chosen candidate, the basis…`
- `server_evidence`: `Trust per server, not totals: every published measurement capsule about ONE endpoint URL across all batches — MCP contract-parity dimension…`
- `verify_capsule`: `Verify one measurement capsule. Pass capsule_json as the capsule's JSON TEXT (exact: number lexemes are kept) or as an object. Recomputes c…`
- `verify_card`: `Verify a signed gspc.measurement-card under the published rule (https://councilof.ai/signed/HOW-TO-VERIFY.md): recompute the id from the ca…`
- `verify_inclusion`: `Check a sha256 against the live public-root merkle via GET /api/proof?sha=. Three states only: VALID (included), INVALID (not a leaf), UNCH…`
- `x402_trust`: `GET the latest x402 catalog trust snapshot: counts of how many catalogued x402 resources open a correct 402 challenge vs how many are phant…`

## Tools at `https://councilof.ai/mcp`

- `art50_marking_evidence`: `PAID (x402 or CSOAI LTD invoice). Article 50 marking-evidence pack via https://councilof.ai/api/art50/marking-evidence: which machine-reada…`
- `board_totals`: `Live GSPC board totals from https://councilof.ai/api/gspc. Returns the slot count and the measured count as two labelled numbers WITH their…`
- `commission_card`: `PAID (x402). Commission one signed card-v0 receipt (surface ras.commission) for a named subject on the frozen bank via https://councilof.ai…`
- `evidence_bundle`: `PAID (x402). For ONE obligation (article-50, article-53 GPAI transparency, dora or cra) and an optional subject via https://councilof.ai/ap…`
- `evidence_bundle_preview`: `For ONE obligation (article-50, article-53 GPAI transparency, dora or cra) and an optional subject: the obligation record, its counsel-gate…`
- `get_axis`: `One axis row from the live GSPC board at https://councilof.ai/api/gspc — every axis the board carries, behavioural and financial families a…`
- `get_card`: `GET one public-root card-v0 leaf by sha256 (64 hex) from https://councilof.ai/cards/{sha16}.json. UNMEASURED cells stay visible. States: VA…`
- `get_root`: `GET the permissionless public-root at https://councilof.ai/root.json. Returns merkle_root, card_count, as_of, and UNMEASURED notes. Separat…`
- `list_cards`: `The published signed-card index (https://councilof.ai/signed/card_index.json): what the index declares (n_cards) and how many rows it actua…`
- `mcp_trust`: `GET the latest MCP handshake trust snapshot (https://councilof.ai/interop/mcp-trust/latest.json): counts of how many internet-facing MCP se…`
- `measurement_index`: `Read the latest signed measurement-capsule index published at https://councilof.ai/measurement-capsules/latest.json: the index root over ev…`
- `receipts_batch`: `PAID (x402 or CSOAI LTD invoice). A historical batch of the estate's measurement receipts via https://councilof.ai/api/receipts/batch: ever…`
- `route`: `GSPC Route (free, decide-only). Applies YOUR policy and the fixed GSPC floor to a candidate set and returns the chosen candidate, the basis…`
- `rwa_evidence`: `PAID (x402). Per-request signed evidence card of ONE XRPL issued asset's deterministic on-ledger state via https://councilof.ai/api/rwa/evi…`
- `server_evidence`: `Trust per server, not totals: every published measurement capsule about ONE endpoint URL across all batches — MCP contract-parity dimension…`
- `verify_capsule`: `Verify one measurement capsule. Pass capsule_json as the capsule's JSON TEXT (exact: number lexemes are kept) or as an object. Recomputes c…`
- `verify_card`: `Verify a signed gspc.measurement-card under the published rule (https://councilof.ai/signed/HOW-TO-VERIFY.md): recompute the id from the ca…`
- `verify_inclusion`: `Check a sha256 against the live public-root merkle via GET /api/proof?sha=. Three states only: VALID (included), INVALID (not a leaf), UNCH…`
- `x402_trust`: `GET the latest x402 catalog trust snapshot: counts of how many catalogued x402 resources open a correct 402 challenge vs how many are phant…`

## Changes

- 2026-10-15: [description changed, field changed](../../deltas/2026-10-15/72b229b0a72f686b6a58.json): `4 field(s) changed; signals: length_more_than_doubled`
- 2026-10-08: [description changed, schema changed](../../deltas/2026-10-08/72b229b0a72f686b6a58.json): `5 field(s) changed`
- 2026-10-08: [description changed, schema changed](../../deltas/2026-10-08/646cc9386b69a5727a2b.json): `4 field(s) changed`
- 2026-10-07: [description changed, schema changed](../../deltas/2026-10-07/646cc9386b69a5727a2b.json): `5 field(s) changed; signals: url_introduced`
- 2026-10-07: [description changed, field changed, schema changed](../../deltas/2026-10-07/72b229b0a72f686b6a58.json): `14 field(s) changed; signals: url_introduced`
- 2026-10-06: [description changed, schema changed](../../deltas/2026-10-06/72b229b0a72f686b6a58.json): `9 field(s) changed; signals: url_introduced`
- 2026-10-06: [description changed, schema changed](../../deltas/2026-10-06/646cc9386b69a5727a2b.json): `5 field(s) changed; signals: url_introduced`
- 2026-10-03: [description changed, schema changed](../../deltas/2026-10-03/72b229b0a72f686b6a58.json): `9 field(s) changed; signals: url_introduced`
- 2026-10-03: [description changed, schema changed](../../deltas/2026-10-03/646cc9386b69a5727a2b.json): `5 field(s) changed; signals: url_introduced`
- 2026-10-01: [count changed, tool added](../../deltas/2026-10-01/646cc9386b69a5727a2b.json): `2 tool(s) added; signals: url_introduced`
- 2026-10-01: [count changed, tool added](../../deltas/2026-10-01/72b229b0a72f686b6a58.json): `3 tool(s) added; signals: url_introduced`
- 2026-09-30: [description changed, schema changed](../../deltas/2026-09-30/72b229b0a72f686b6a58.json): `24 field(s) changed; signals: url_introduced`
- 2026-09-29: [description changed](../../deltas/2026-09-29/72b229b0a72f686b6a58.json): `1 field(s) changed`
- 2026-09-28: [description changed, schema changed](../../deltas/2026-09-28/72b229b0a72f686b6a58.json): `8 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://councilof.ai/mcp/free"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
