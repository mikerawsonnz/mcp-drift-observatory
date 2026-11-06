# capxule.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/capxule.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://capxule.ai/mcp` | 9 | [`7014a251fcaa`](6aef8eb99de229777343.json) | 2026-10-29 |

## Tools at `https://capxule.ai/mcp`

- `browse_journeys`: `Use when the user wants to look through the journeys, optionally within one category (a slug from list_journey_categories). Returns a page…`
- `create_takeaway`: `Use when the user asks for a summary to keep. Composes a markdown takeaway from this journey session: what the user asked, the key points a…`
- `find_journey`: `Use when the user wants a guided, step-by-step journey on a topic, a skill or an exam. Searches the published journeys and returns up to th…`
- `get_journey_progress`: `Use when the user asks where they are in a journey, how far they have come or how much is left. Returns the current stop, visited and remai…`
- `get_resume_link`: `Use when the user wants to continue the journey later, on the website or in another assistant. Returns a resume link and a short resume cod…`
- `list_journey_categories`: `Use when the user asks what kinds of journeys are available. Returns each category slug, a readable label, the number of journeys in it and…`
- `open_journey`: `Use when the user chooses a journey to start or continue. Opens it, or resumes the user's session for it, and returns the session contract:…`
- `restart_journey`: `Use only when the user explicitly asks to start a journey over, after confirming with them. Returns to the first step and clears the visite…`
- `take_journey_step`: `Use for every step after open_journey. Sends the user's choice and returns the next step: 'answer', 'statement', numbered 'options' with id…`

## Changes

- 2026-10-29: [annotation changed, count changed, description changed, field changed, schema changed, tool added, tool removed](../../deltas/2026-10-29/6aef8eb99de229777343.json): `7 tool(s) added; 10 tool(s) removed; 10 field(s) changed`
- 2026-10-27: [description changed](../../deltas/2026-10-27/6aef8eb99de229777343.json): `1 field(s) changed`
- 2026-10-26: [description changed](../../deltas/2026-10-26/6aef8eb99de229777343.json): `1 field(s) changed`
- 2026-10-25: [description changed](../../deltas/2026-10-25/6aef8eb99de229777343.json): `1 field(s) changed`
- 2026-10-24: [description changed](../../deltas/2026-10-24/6aef8eb99de229777343.json): `1 field(s) changed`
- 2026-10-22: [description changed](../../deltas/2026-10-22/6aef8eb99de229777343.json): `1 field(s) changed`
- 2026-10-20: [description changed](../../deltas/2026-10-20/6aef8eb99de229777343.json): `1 field(s) changed`
- 2026-10-18: [description changed](../../deltas/2026-10-18/6aef8eb99de229777343.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://capxule.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
