# www.foliora.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/www.foliora.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://www.foliora.ai/mcp` | 12 | [`3571263f7997`](ff6df35762f4a3ff78f0.json) | 2026-09-16 |

## Tools at `https://www.foliora.ai/mcp`

- `approve_change`: `Approve one drafted change set by its exact canonical hash. Call this only after the customer has read the operations from get_page_job and…`
- `create_preview_link`: `Build a Foliora /preview URL for a public website. Does not crawl, does not take credentials, and does not change the site. Send the human…`
- `get_approved_change`: `Return an already-approved canonical hash and its ordered typed operations. Apply exactly these values; do not reinterpret or regenerate th…`
- `get_page_job`: `One proposed page change: why Foliora proposes it, the brief, the objectives it addresses, the drafted change set with every operation's ex…`
- `get_product`: `Return Foliora product facts: brand, per-site plans, canonical URLs, and product boundaries. Use when the user asks what Foliora is, how mu…`
- `get_snapshot`: `Fetch a Foliora preview snapshot the human already started. Requires the 32-character hex token from /preview/{token}. Returns public findi…`
- `list_findings`: `List the crawl findings still open on a site: SEO and AI-readiness plumbing such as missing descriptions, blocked AI crawlers, missing llms…`
- `list_page_jobs`: `The page changes Foliora proposes for one owned site, highest impact first — the same list the customer's dashboard shows. Each row carries…`
- `list_sites`: `List sites owned by the authenticated Foliora account with crawl and finding status. Requires OAuth or a Foliora API key with read scope.`
- `reject_change`: `Close one drafted change set without approving it. Call this only when the customer says so. The job stays proposed and can be drafted agai…`
- `report_finding_fix`: `After the agent fixes a finding on the site (a meta description, a robots rule, llms.txt), mark it fix_reported with a short note. It shows…`
- `report_publication`: `Record proof that the customer's agent applied every operation from an already-approved canonical hash. Foliora verifies the live page from…`

## Changes

- 2026-09-16: [count changed, description changed, schema changed, tool removed](../../deltas/2026-09-16/ff6df35762f4a3ff78f0.json): `5 tool(s) removed; 14 field(s) changed`
- 2026-09-08: [count changed, tool added](../../deltas/2026-09-08/ff6df35762f4a3ff78f0.json): `4 tool(s) added`
- 2026-09-07: [count changed, description changed, tool added](../../deltas/2026-09-07/ff6df35762f4a3ff78f0.json): `4 tool(s) added; 1 field(s) changed`
- 2026-09-02: [annotation changed, count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-09-02/ff6df35762f4a3ff78f0.json): `6 tool(s) added; 124 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://www.foliora.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
