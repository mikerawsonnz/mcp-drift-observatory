# ase.academy: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/ase.academy.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://ase.academy/mcp` | 4 | [`2ae5f5f1c233`](f933d14374fb9035ae55.json) | 2026-10-23 |

## Tools at `https://ase.academy/mcp`

- `find_elements`: `Find elements of the table by words in their name, problem or test, by role (dev, lead, plat, qa, ...), by group (security, verification, .…`
- `get_element`: `One element in full: problem, observable test with its clauses and evidence kinds, when it applies, when it adds work without helping, acti…`
- `overview`: `The Agentic Engineering Periodic System: what it is, how to read it (rows, columns, judging and reading rules), the roles. Call this first.`
- `repository_checklist`: `What a repository can show for each test, clause by clause, what it cannot, and the judging rules. Use it to check the current project; rea…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://ase.academy/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
