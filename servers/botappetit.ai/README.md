# botappetit.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/botappetit.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://botappetit.ai/mcp` | 14 | [`d845e0362e86`](e19ce61dadbaa55281fe.json) | 2026-11-06 |

## Tools at `https://botappetit.ai/mcp`

- `explain_check`: `Explain one Bot Appétit check: what it looks at, why it matters for machines reading a page, and what good looks like. Use the id from list…`
- `get_report`: `Get a stored Bot Appétit report by scan id, the same report a person sees at botappetit.ai/r/<id>. Costs nothing and does not scan. Use it…`
- `leaderboard`: `The highest-scoring sites by category, from the latest Bot Appétit scan of each site's homepage: rank, host, score out of 100, grade and a…`
- `list_checks`: `List every check Bot Appétit runs on a page, grouped by category, with the id of each. Use the id with explain_check for what a check means…`
- `list_sites`: `List the sites the signed-in person follows in Bot Appétit, newest activity first, each with its latest site-scan score, the change since t…`
- `page_history`: `List every stored Bot Appétit scan of one exact page, newest first, with the score at the time and how it moved since the scan before. Cost…`
- `request_site_scan`: `A whole-site scan reads a representative sample of a site and needs a person with a Bot Appétit account, and an agent never creates one. Th…`
- `scan_page`: `Check one web page for AEO, SEO and performance: can a machine consume it? Returns the findings by check and the report link. If the exact…`
- `set_pins`: `Pin or unpin pages on one of the signed-in person's sites. Pinned pages are scanned in every site scan of that site and count toward its sc…`
- `set_rescan_settings`: `Turn the signed-in person's monthly re-scans of their sites on or off, and the email of each result on or off. Leave a field out to keep it…`
- `share_site_scan`: `Create or stop the unlisted share link for one of the signed-in person's site scans. Site scans are private by default; a link lets anyone…`
- `site_history`: `Read one of the signed-in person's sites over time: every site scan of it newest first with the score and the change since the previous sco…`
- `site_scan_status`: `Read one of the signed-in person's site scans: whether it is still running, and once it has finished the score, the checks that failed, the…`
- `start_site_scan`: `Start a whole-site scan for the signed-in person's account: Bot Appétit reads a representative sample of the site (not every page) and scor…`

## Changes

- 2026-11-06: [annotation changed, description changed, field changed](../../deltas/2026-11-06/e19ce61dadbaa55281fe.json): `85 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://botappetit.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
