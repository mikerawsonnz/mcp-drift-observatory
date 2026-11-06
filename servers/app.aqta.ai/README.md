# app.aqta.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/app.aqta.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://app.aqta.ai/api/mcp` | 10 | [`848f6080bd63`](93d7e519637ecfb275e1.json) | 2026-10-23 |

## Tools at `https://app.aqta.ai/api/mcp`

- `decode_receipt`: `Read a receipt field by field, with stated limits. Does not check the signature.`
- `explain_attestation_format`: `The receipt format: fields, outcomes, verification commands, and what a signature does not establish. Use before describing the format.`
- `get_public_key`: `Fetch the published Seal signing key.`
- `get_review_pack`: `The published sample evidence pack: fixed review question, bound receipts, disclosure.`
- `get_sample_receipt`: `A genuine signed receipt from the sample workspace (demo key), for trying verification.`
- `get_transparency_proof`: `Inclusion proof plus signed tree head for one of your receipts. Requires your aqta_ key.`
- `list_my_receipts`: `List your workspace receipts filtered by outcome, policy, model, or date range. Requires your aqta_ key as Bearer.`
- `verify_evidence_pack`: `Verify a review pack receipt by receipt. Each verdict comes from the signed envelope itself, never from stored state, and results are per-r…`
- `verify_receipt`: `Check that a record still says what was signed: the permitted or refused decision, unchanged, under Seal's published issuer keys or a key y…`
- `workspace_summary`: `Outcome, model and policy counts across your recent receipts. Requires your aqta_ key.`

## Changes

- 2026-10-23: [schema changed](../../deltas/2026-10-23/93d7e519637ecfb275e1.json): `2 field(s) changed`
- 2026-10-10: [description changed, schema changed](../../deltas/2026-10-10/93d7e519637ecfb275e1.json): `3 field(s) changed`
- 2026-08-25: [description changed, schema changed](../../deltas/2026-08-25/93d7e519637ecfb275e1.json): `3 field(s) changed; signals: length_more_than_doubled`
- 2026-08-24: [description changed, schema changed](../../deltas/2026-08-24/93d7e519637ecfb275e1.json): `5 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://app.aqta.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
