# app.annsa.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/app.annsa.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://app.annsa.ai/mcp` | 8 | [`9abd48353218`](59d41e60a9e6430b00b0.json) | 2026-11-06 |

## Tools at `https://app.annsa.ai/mcp`

- `annsa_ask`: `Find what customers said, what's on the board, or how Annsa works. 'about' picks the source: feedback (default), annsa (the docs, or a skil…`
- `annsa_board`: `Arrange the board. Some actions are a person's only. [production · app.annsa.ai · tools 8efe806f]`
- `annsa_decide`: `Record a person's decisions. Agents may list or propose principles. [production · app.annsa.ai · tools 8efe806f]`
- `annsa_file`: `Add feedback, a finding, a priority, a transcript, a page or a template. [production · app.annsa.ai · tools 8efe806f]`
- `annsa_priorities`: `List ranked priorities. Filter by stage, bet, person or topic, or get one by number. 'weekly' and 'view' return summaries. A read. [product…`
- `annsa_share`: `Tell the customers who asked that their priority shipped, by email or the widget. Needs a person's sign-in. [production · app.annsa.ai · to…`
- `annsa_spec`: `Read a priority's spec: Problem, What to build, Done When, open asks and principle titles. 'include_evidence' adds Evidence and direction a…`
- `annsa_work`: `Do the work on a priority, and settle routine asks with undo. [production · app.annsa.ai · tools 8efe806f]`

## Changes

- 2026-11-06: [description changed, schema changed](../../deltas/2026-11-06/59d41e60a9e6430b00b0.json): `72 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-11-05: [description changed, schema changed](../../deltas/2026-11-05/59d41e60a9e6430b00b0.json): `107 field(s) changed; signals: imperative_language_introduced` **(notable)**
- 2026-11-04: [description changed, schema changed](../../deltas/2026-11-04/59d41e60a9e6430b00b0.json): `9 field(s) changed`
- 2026-11-02: [description changed, schema changed](../../deltas/2026-11-02/59d41e60a9e6430b00b0.json): `14 field(s) changed`
- 2026-11-01: [description changed, schema changed](../../deltas/2026-11-01/59d41e60a9e6430b00b0.json): `28 field(s) changed`
- 2026-10-30: [description changed, schema changed](../../deltas/2026-10-30/59d41e60a9e6430b00b0.json): `21 field(s) changed`
- 2026-10-29: [description changed, schema changed](../../deltas/2026-10-29/59d41e60a9e6430b00b0.json): `13 field(s) changed`
- 2026-10-27: [description changed, schema changed](../../deltas/2026-10-27/59d41e60a9e6430b00b0.json): `163 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-10-21: [schema changed](../../deltas/2026-10-21/59d41e60a9e6430b00b0.json): `1 field(s) changed`
- 2026-10-20: [schema changed](../../deltas/2026-10-20/59d41e60a9e6430b00b0.json): `8 field(s) changed`
- 2026-10-19: [schema changed](../../deltas/2026-10-19/59d41e60a9e6430b00b0.json): `18 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://app.annsa.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
