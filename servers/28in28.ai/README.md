# 28in28.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/28in28.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://28in28.ai/mcp` | 3 | [`7016fb5a880d`](075a4a6f7c4c1bd1119d.json) | 2026-11-07 |

## Tools at `https://28in28.ai/mcp`

- `checkDomain`: `Reads the public DNS of one domain and reports SPF, DKIM, DMARC, MX, MTA-STS and TLS-RPT findings, risks, unknowns and the exact DNS change…`
- `quoteFixVerify`: `Runs the email-authentication check of one domain and returns a machine-readable, NON-BINDING quote for Fix & Verify: price (EUR 99 net per…`
- `verifyFixVerify`: `Re-runs the check of the domain and compares it with the acceptance criteria and baseline of an earlier quoteFixVerify result: PASS when ev…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://28in28.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
