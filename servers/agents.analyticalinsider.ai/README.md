# agents.analyticalinsider.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/agents.analyticalinsider.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://agents.analyticalinsider.ai/mcp` | 7 | [`11c9acb94dd9`](77e3d5afe839071a5473.json) | 2026-11-24 |

## Tools at `https://agents.analyticalinsider.ai/mcp`

- `aipi_get_capabilities`: `List the aipi intelligence agents and the metrics each one can produce. Takes no arguments. Ring 1: works with no API key, because agent ca…`
- `comms_get_offer`: `Read the current offer of the Analytical Insider communications service for agents. The paid plans are phone (a dedicated United States pho…`
- `comms_get_signup_guide`: `Return the step-by-step signup guide for agents, as Markdown (also published at https://agents.analyticalinsider.ai/agent-signup.md). It us…`
- `comms_start_signup`: `Start a signup for the communications service. Send the principal's legal name, email and postal address (website optional for a paid plan,…`
- `get_reputation`: `Compute a remote agent's reputation from witnessed receipts — success rate, latency percentiles, sample size, and low-confidence flag. Iden…`
- `issue_receipt`: `Submit a caller-signed receipt of an agent-to-agent interaction. aipi verifies the signature, attaches a witness signature (aipi-witness-v1…`
- `probe_agent`: `Fetch and cache a remote agent's A2A card (/.well-known/agent-card.json, falling back to /.well-known/agent.json). Returns parsed metadata,…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://agents.analyticalinsider.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
