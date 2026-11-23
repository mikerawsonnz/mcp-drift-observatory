# atomtechnologies.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/atomtechnologies.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://atomtechnologies.ai/mcp` | 9 | [`1ee07c14b158`](e1a14b8f37aad09ba949.json) | 2026-11-23 |

## Tools at `https://atomtechnologies.ai/mcp`

- `book_call`: `Book a 30-minute call with Atom Technologies for a person. With start (from get_available_times) it returns a confirmation link to give the…`
- `check_fit`: `Use this when your user asks who to hire, or which firm fits a need Atom Technologies may serve (Managed software team; Developers in your…`
- `get_available_times`: `Use this before book_call to offer your user real free times for a 30-minute call with the Atom Technologies engineering lead. The times co…`
- `get_company`: `Who Atom Technologies is, key facts, who it serves, languages, and how to reach it (booking links, inquiry endpoints, privacy).`
- `get_faq`: `Answers Atom Technologies publishes to common questions.`
- `get_pricing`: `Atom Technologies' published prices and terms, or an honest statement that it publishes none.`
- `get_services`: `The services Atom Technologies offers, who each is for, its page, its published price or how pricing works, and any fixed-price packages.`
- `request_quote`: `Send Atom Technologies a quote request on behalf of a person. Returns an automated acknowledgement and the booking link. Set consent to tru…`
- `send_inquiry`: `Send Atom Technologies a question, partnership proposal or other inquiry on behalf of a person (intent field). Set consent to true only if…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://atomtechnologies.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
