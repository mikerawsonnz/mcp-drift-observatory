# tools.campaignpack.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/tools.campaignpack.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://tools.campaignpack.ai/mcp` | 13 | [`273f11e9dae2`](37dc2e3aa0d6d10fcb03.json) | 2026-11-08 |

## Tools at `https://tools.campaignpack.ai/mcp`

- `abort_campaign`: `Stop a running campaign.`
- `answer_approval`: `Answer a paused run that wants to send the user's data somewhere outside Campaign Pack. Ask the person; never decide for them.`
- `check_campaign`: `Progress of a running campaign: status, the tools it has just called, queue position, and whether it is waiting for a human approval. Poll…`
- `get_download_url`: `A link the person can open to get one file — the campaign PDF, a product still, a video. Works for any file in the workspace, including one…`
- `get_pack`: `Collect a finished campaign: the folder, its files, the written overview, and the path to the PDF.`
- `list_campaign_access`: `Who owns a campaign and who it is shared with.`
- `list_campaigns`: `Campaigns on this account, newest first, including ones shared with it. Start here when you do not already have an id — the ids from start_…`
- `list_workspace_files`: `List files and folders in the account's workspace — campaign folders, scripts, product stills, PDFs, uploads. Directories end in '/'.`
- `read_workspace_file`: `Contents of a text file in the workspace — a script, the plan, the creator brief, a transcript. Large files are truncated. For a PDF, image…`
- `share_campaign`: `Give a teammate access to a campaign by email address — including while it is still running. They see the same live run from their own AI c…`
- `start_campaign`: `Start a marketing campaign pack on Campaign Pack's own GPUs. Produces a campaign plan, ideas, ad and social scripts, a creator brief, and a…`
- `unshare_campaign`: `Revoke a collaborator's access. Takes effect on their next request.`
- `upload_product_photo`: `Put a product photo into the user's workspace so a campaign can edit stills from the real thing. Base64 of the image bytes.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://tools.campaignpack.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
