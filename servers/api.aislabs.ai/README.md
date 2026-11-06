# api.aislabs.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.aislabs.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.aislabs.ai/mcp` | 3 | [`3429d8a1c95b`](c89254ace4cca834bb5a.json) | 2026-09-29 |
| `https://api.aislabs.ai/recorder/mcp` | 5 | [`b5988950db7b`](eca3f76420b2af2f3056.json) | 2026-09-02 |
| `https://api.aislabs.ai/cve/mcp` | 4 | [`e86895a576a2`](feb229ac0da36d41cb04.json) | 2026-09-29 |

## Tools at `https://api.aislabs.ai/mcp`

- `about_aislabs`: `FREE. The AIS front desk: what AIS sells (tested code libraries, CVE intelligence, the Agent Flight Recorder), which building serves what,…`
- `how_to_pay`: `FREE. The two payment doors — Gateway key (Authorization: Bearer; CVE key $19 / 30 days, Flight Recorder key $19 / 30 days, campus pass $29…`
- `list_buildings`: `FREE. The campus directory: every AIS MCP building (URL, tools, prices, free tier) and which key scope unlocks it, and what each key costs.…`

## Tools at `https://api.aislabs.ai/recorder/mcp`

- `delete_monitor`: `Agent Flight Recorder — remove a monitor (needs its secret or the owning key).`
- `fetch_capsule`: `Agent Flight Recorder (Gateway key) — get the last state capsule a monitored agent sent, to resume from where it died.`
- `fleet_status`: `Agent Flight Recorder (Gateway key) — every monitor you own: alive / late / dead, last heartbeat, capsule preview.`
- `heartbeat`: `Agent Flight Recorder — "still alive" ping for a registered monitor. Include capsule (any JSON ≤32KB: current step, done, next, ids) so a d…`
- `register_monitor`: `Agent Flight Recorder — FREE (1 monitor per alert target) / Gateway key (20 monitors + stored capsules + fleet view). Register an agent or…`

## Tools at `https://api.aislabs.ai/cve/mcp`

- `brief_teaser`: `FREE. Today's top-3 CVE priorities from the AIS daily ranking (no scores). Ranked by real exploitation — KEV + EPSS + KEV-recency — not CVS…`
- `cve_verdict`: `PAID — unlock with an AIS CVE key ($19 / 30 days) or campus pass (https://aislabs.ai/gateway/), or pay per call over x402 on the HTTP twin:…`
- `kev_fresh`: `PAID — unlock with an AIS CVE key ($19 / 30 days) or campus pass (https://aislabs.ai/gateway/), or pay per call over x402 on the HTTP twin:…`
- `top_cves_today`: `PAID — unlock with an AIS CVE key ($19 / 30 days) or campus pass (https://aislabs.ai/gateway/), or pay per call over x402 on the HTTP twin:…`

## Changes

- 2026-09-29: [description changed](../../deltas/2026-09-29/c89254ace4cca834bb5a.json): `3 field(s) changed`
- 2026-09-29: [description changed](../../deltas/2026-09-29/feb229ac0da36d41cb04.json): `3 field(s) changed; signals: url_introduced`
- 2026-09-02: [schema changed](../../deltas/2026-09-02/eca3f76420b2af2f3056.json): `1 field(s) changed; signals: length_more_than_doubled`
- 2026-09-01: [count changed, tool added, tool removed](../../deltas/2026-09-01/c89254ace4cca834bb5a.json): `2 tool(s) added; 9 tool(s) removed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.aislabs.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
