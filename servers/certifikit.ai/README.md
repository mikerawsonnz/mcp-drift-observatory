# certifikit.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/certifikit.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://certifikit.ai/mcp` | 4 | [`195adc3fbfe7`](d45eb9be114050bb87df.json) | 2026-10-20 |

## Tools at `https://certifikit.ai/mcp`

- `build_insurance_requirements`: `Recommends the insurance a general contractor should require of a subcontractor, or a property manager or HOA of a vendor: general liabilit…`
- `check_certificate`: `Checks a certificate of insurance (ACORD 25) against insurance requirements with CertifiKit's deterministic rules engine: coverage present,…`
- `find_coi_guides`: `Searches CertifiKit's plain-English guides on certificates of insurance: reading an ACORD 25, additional insured endorsements (CG 20 10), w…`
- `list_requirement_presets`: `The ready-made insurance requirement sets check_certificate accepts as preset: a standard construction subcontractor and a property / HOA v…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://certifikit.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
