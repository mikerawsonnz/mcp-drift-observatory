# afmr.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/afmr.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://afmr.ai/api/rpc` | 4 | [`9ff837136ef3`](204d8f6a7e3a70ebe2ed.json) | 2026-08-20 |
| `https://afmr.ai/mcp` | 4 | [`9ff837136ef3`](bef7b07757e77d976e14.json) | 2026-08-23 |

## Tools at `https://afmr.ai/api/rpc`

- `discover_afmr`: `Return canonical AFMR specifications, registries, schemas, endpoints, and scope boundaries.`
- `get_lift_evidence_contract`: `Return the stable configuration-scoped public-card schema and empty public index; no results are asserted.`
- `get_reputation_attestation_contract`: `Return the portable attestation, trust-profile, verifier-result, endpoint-registry, and lifecycle contracts.`
- `lookup_failure_mode`: `Find exact AFMR 1.0 failure-mode records by permanent ID or bounded text query.`

## Tools at `https://afmr.ai/mcp`

- `discover_afmr`: `Return canonical AFMR specifications, registries, schemas, endpoints, and scope boundaries.`
- `get_lift_evidence_contract`: `Return the stable configuration-scoped public-card schema and empty public index; no results are asserted.`
- `get_reputation_attestation_contract`: `Return the portable attestation, trust-profile, verifier-result, endpoint-registry, and lifecycle contracts.`
- `lookup_failure_mode`: `Find exact AFMR 1.0 failure-mode records by permanent ID or bounded text query.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://afmr.ai/api/rpc"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
