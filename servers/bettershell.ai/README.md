# bettershell.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/bettershell.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://bettershell.ai/mcp` | 13 | [`ffc8c2b70071`](68243e6e3554c247bb83.json) | 2026-11-27 |

## Tools at `https://bettershell.ai/mcp`

- `add_to_profile`: `Saves what the person tells you to save to their BetterShell profile, in their own words: lines under a job, project or activity, a new ent…`
- `check_fit`: `Checks a job posting against the person's saved profile, measured the way BetterShell makes the page: whether there is a full page of mater…`
- `connect_bettershell_account`: `Connects the person's BetterShell account, so the résumés BetterShell makes in this chat are made on that account and saved there, where th…`
- `edit_resume`: `Changes lines, the summary or the look of a résumé BetterShell made, fits it back to its page and redraws it, with a new PDF. Use it when t…`
- `get_profile`: `Returns the person's saved BetterShell profile: every job, project and activity with its lines, and their skills, in their own words. Use i…`
- `interview_prep`: `For one application, returns the page that was sent, the person's own lines that page left off, and the posting, to prepare them for that i…`
- `list_applications`: `Shows the person's applications in BetterShell and the stage each reached, with how many got a phone screen or an interview, which have wai…`
- `make_cover_letter`: `Prints a cover letter you wrote as the pair of a résumé BetterShell made: the same header, type and colours, fitted to one page, with a PDF…`
- `read_job_posting`: `Reads the job posting at a link and returns its title, company and text, so you can see what the job asks for before tailoring the person's…`
- `read_resume`: `Returns the text of a résumé BetterShell made, line by line with ids, as it prints. Use it to talk about the résumé, write or change a line…`
- `review_resume`: `Measures the person's résumé the way BetterShell lays out a page and returns the facts for a review: how much of a page it fills, which job…`
- `tailor_resume`: `BetterShell's resume builder. Makes the person a finished, tailored one-page résumé PDF from their own résumé or CV: it picks their stronge…`
- `update_application`: `Records news on one of the person's applications when they tell you: they applied, had a phone screen or an interview round, got an offer o…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://bettershell.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
