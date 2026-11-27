# app.annsa.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/app.annsa.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://app.annsa.ai/mcp` | 8 | [`3df07fd279e1`](59d41e60a9e6430b00b0.json) | 2026-11-27 |

## Tools at `https://app.annsa.ai/mcp`

- `annsa_ask`: `Ask Annsa a question in plain words. Finds what customers said, what's on the board, or how Annsa works. about picks where to look: feedbac…`
- `annsa_board`: `Tidy the board. Use it to change a priority's stage or severity, merge duplicates, move priorities between groups, fix a title, place prior…`
- `annsa_decide`: `Record what a person decided. A person uses it to answer a question an agent raised or sign off a priority. As an agent you can list princi…`
- `annsa_file`: `Add something new to the board. Use it to file what a customer said, a bug or finding you found, or an idea. It attaches to the matching pr…`
- `annsa_priorities`: `Your ranked to-do list. Use it to see what to work on next: every open priority in rank order, with how many customers asked and why each o…`
- `annsa_share`: `Tell customers their request shipped. Use it after a priority ships to email or notify everyone who asked for it. Emails can't be unsent, s…`
- `annsa_spec`: `The plan for one priority. Use it before starting work: it gives you the Problem, What to build, and the Done When lines you'll have to pro…`
- `annsa_work`: `Do the work on a priority. Use it to claim a priority, write your part of the spec, leave notes, prove each Done When line with verify, and…`

## Changes

- 2026-11-27: [schema changed](../../deltas/2026-11-27/59d41e60a9e6430b00b0.json): `26 field(s) changed`
- 2026-11-25: [schema changed](../../deltas/2026-11-25/59d41e60a9e6430b00b0.json): `1 field(s) changed`
- 2026-11-23: [description changed, schema changed](../../deltas/2026-11-23/59d41e60a9e6430b00b0.json): `13 field(s) changed`
- 2026-11-20: [schema changed](../../deltas/2026-11-20/59d41e60a9e6430b00b0.json): `20 field(s) changed; signals: length_more_than_doubled`
- 2026-11-19: [schema changed](../../deltas/2026-11-19/59d41e60a9e6430b00b0.json): `7 field(s) changed`
- 2026-11-18: [schema changed](../../deltas/2026-11-18/59d41e60a9e6430b00b0.json): `28 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-11-17: [schema changed](../../deltas/2026-11-17/59d41e60a9e6430b00b0.json): `6 field(s) changed`
- 2026-11-16: [description changed, schema changed](../../deltas/2026-11-16/59d41e60a9e6430b00b0.json): `64 field(s) changed; signals: length_more_than_doubled`
- 2026-11-14: [field changed, schema changed](../../deltas/2026-11-14/59d41e60a9e6430b00b0.json): `17 field(s) changed`
- 2026-11-13: [schema changed](../../deltas/2026-11-13/59d41e60a9e6430b00b0.json): `25 field(s) changed`
- 2026-11-12: [schema changed](../../deltas/2026-11-12/59d41e60a9e6430b00b0.json): `10 field(s) changed`
- 2026-11-09: [description changed, schema changed](../../deltas/2026-11-09/59d41e60a9e6430b00b0.json): `248 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-11-06: [description changed, schema changed](../../deltas/2026-11-06/59d41e60a9e6430b00b0.json): `72 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-11-05: [description changed, schema changed](../../deltas/2026-11-05/59d41e60a9e6430b00b0.json): `107 field(s) changed; signals: imperative_language_introduced` **(notable)**
- 2026-11-04: [description changed, schema changed](../../deltas/2026-11-04/59d41e60a9e6430b00b0.json): `9 field(s) changed`
- 2026-11-02: [description changed, schema changed](../../deltas/2026-11-02/59d41e60a9e6430b00b0.json): `14 field(s) changed`
- 2026-11-01: [description changed, schema changed](../../deltas/2026-11-01/59d41e60a9e6430b00b0.json): `28 field(s) changed`
- 2026-10-30: [description changed, schema changed](../../deltas/2026-10-30/59d41e60a9e6430b00b0.json): `21 field(s) changed`
- 2026-10-29: [description changed, schema changed](../../deltas/2026-10-29/59d41e60a9e6430b00b0.json): `13 field(s) changed`
- 2026-10-27: [description changed, schema changed](../../deltas/2026-10-27/59d41e60a9e6430b00b0.json): `163 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://app.annsa.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
