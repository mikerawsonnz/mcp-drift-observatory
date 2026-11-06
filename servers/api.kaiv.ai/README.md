# api.kaiv.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.kaiv.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.kaiv.ai/api/bridge/mcp/dns-check-e159a722` | 1 | [`af612a8b53ec`](71e216e04bfe9cc97b90.json) | 2026-08-23 |
| `https://api.kaiv.ai/api/bridge/mcp/version-truth-ca7b5b8c` | 3 | [`5176af0f6b52`](8e9639f7aa0dad5a9d4b.json) | 2026-08-22 |
| `https://api.kaiv.ai/api/bridge/mcp/dependency-trust-f1aaf06d` | 5 | [`6336e8a91696`](bd5778e9e04910374e00.json) | 2026-08-22 |
| `https://api.kaiv.ai/api/bridge/mcp/can-i-use-5446c68b` | 3 | [`a581976cf743`](c6ba5b1494e8c1056708.json) | 2026-09-05 |
| `https://api.kaiv.ai/api/bridge/mcp/email-check-b6ab5250` | 4 | [`28dd65207054`](d4251f86d38836fc36be.json) | 2026-08-23 |

## Tools at `https://api.kaiv.ai/api/bridge/mcp/dns-check-e159a722`

- `resolve_dns`: `Resolve any DNS record live via Google Public DNS. Answers: is DNS propagated? What are the MX/TXT/SPF/DKIM records? Where does this CNAME…`

## Tools at `https://api.kaiv.ai/api/bridge/mcp/version-truth-ca7b5b8c`

- `get_cycle`: `One release cycle of a product: its latest patch version, release date, LTS/support/EOL dates and whether extended support exists. Use when…`
- `get_product`: `All release cycles for a product, newest first: latest patch version, release date, LTS status/date, end-of-life date, and end of active su…`
- `list_products`: `List every product slug tracked (nodejs, python, react, postgresql, ubuntu, …). Call this first when unsure of the exact product slug to pa…`

## Tools at `https://api.kaiv.ai/api/bridge/mcp/dependency-trust-f1aaf06d`

- `get_advisory`: `Get a security advisory (vulnerability) by its key. Returns a security advisory by key — e.g. a GHSA id taken from a version's advisoryKeys…`
- `get_dependencies`: `Get the resolved dependency graph for one package version. Returns the full resolved dependency graph (direct and indirect) for a version —…`
- `get_package`: `List every version of a package and whether each is deprecated. Returns all published versions of a package with publish date, the default-…`
- `get_package_version`: `Get license, security advisories, and source links for one package version. Returns detailed metadata for a single version: SPDX licenses,…`
- `get_project_health`: `Get a project's OpenSSF Scorecard security posture and maintenance signals. THE trust check. Returns supply-chain trust signals for a packa…`

## Tools at `https://api.kaiv.ai/api/bridge/mcp/can-i-use-5446c68b`

- `check_feature_support`: `Can I use this feature, and from which browser version? Accepts a loose name (":has()", "container queries", "css-grid") and resolves it to…`
- `get_feature_by_id`: `Support table for an exact caniuse feature id. Use when the id is already known, for example from a previous search. No fuzzy matching is a…`
- `search_features`: `Find the caniuse feature id for a loose query. Use when a query is ambiguous and you want to choose between candidates before checking supp…`

## Tools at `https://api.kaiv.ai/api/bridge/mcp/email-check-b6ab5250`

- `check_email_domain`: `Full email posture for a domain: can it receive mail, and can it be spoofed? Runs MX, SPF and DMARC lookups together and returns a plain-la…`
- `get_dmarc_record`: `DMARC record, policy, and whether it actually protects. Returns the DMARC TXT record at _dmarc.<domain>, its policy (none / quarantine / re…`
- `get_mx_records`: `Mail exchanger records for a domain. Returns the MX hosts in priority order and whether any exist. A domain with no MX records cannot recei…`
- `get_spf_record`: `SPF record and how strict it is. Returns the SPF TXT record, the qualifier on its 'all' mechanism (fail / softfail / neutral / pass) and wh…`

## Changes

- 2026-08-23: [schema changed](../../deltas/2026-08-23/d4251f86d38836fc36be.json): `118 field(s) changed`
- 2026-08-23: [schema changed](../../deltas/2026-08-23/71e216e04bfe9cc97b90.json): `11 field(s) changed`
- 2026-08-22: [annotation changed, field changed](../../deltas/2026-08-22/8e9639f7aa0dad5a9d4b.json): `18 field(s) changed`
- 2026-08-22: [annotation changed, description changed, field changed, schema changed](../../deltas/2026-08-22/bd5778e9e04910374e00.json): `56 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.kaiv.ai/api/bridge/mcp/dns-check-e159a722"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
