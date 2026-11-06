# api.bumblebox.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.bumblebox.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.bumblebox.ai/api/mcp` | 17 | [`4dca9509a89e`](9b5c6962987b04112709.json) | 2026-10-27 |

## Tools at `https://api.bumblebox.ai/api/mcp`

- `archive_email`: `Moves one inbox email to its mailbox's archive folder, on the mail server too. Undone by restore_to_inbox. Nothing is deleted.`
- `create_campaign_draft`: `Writes one draft inside an existing campaign, to one recipient (added to the campaign list if new), from the campaign's sender. Nothing is…`
- `draft_reply`: `Saves the text as the reply draft of a received email, from the address the email was written to (a brand address or the mailbox). needsIde…`
- `get_email`: `One email in full: sender, recipients, date, subject, plain-text body, attachment names, folder and BumbleBox classification.`
- `list_calendar_events`: `Events of the connected Google calendars between two dates (default: the next 7 days, at most 62 days).`
- `list_campaign_drafts`: `The drafts of one campaign that wait for the user to validate them in BumbleBox (recipient, subject, plain-text body, sender), newest first…`
- `list_folders`: `The folders of each connected mailbox, as last synced. Trash, spam, sent and drafts are left out.`
- `list_missions`: `The user's prospection campaigns (missions), most recently active first, with the number of drafts waiting, emails sent and prospects who r…`
- `list_replies_to_validate`: `Replies received on campaigns that still need the user: prepared reply drafts waiting for validation, and replies with no answer yet (with…`
- `list_to_answer`: `Received emails BumbleBox classified as needing a reply and still in the inbox, newest first.`
- `move_email`: `Moves one inbox email to an existing folder of the same mailbox (see list_folders), on the mail server too. No folder is created. Undone by…`
- `restore_to_inbox`: `Moves an archived, filed or trashed email back to the inbox, on the mail server too.`
- `search_contacts`: `Contacts BumbleBox knows from the mail history (name, address, organization domain, exchange counts, last exchanges, VIP mark, note), match…`
- `search_emails`: `Searches every connected mailbox (sender, subject, preview), newest first. Operators: from:, subject:, before:YYYY-MM-DD, after:YYYY-MM-DD,…`
- `send_reply`: `Replies to the sender of one received email, and only to them (no Cc, no Bcc, no attachment), from the address the email was written to. Wh…`
- `trash_email`: `Moves one inbox email to its mailbox's trash when BumbleBox certifies it as noise (spam, newsletter, promotion, with a unanimous safety vot…`
- `update_campaign_draft`: `Changes the subject, body or recipient of a draft that is still a draft. Nothing is sent, and a draft the user already validated cannot be…`

## Changes

- 2026-10-27: [description changed](../../deltas/2026-10-27/9b5c6962987b04112709.json): `3 field(s) changed`
- 2026-10-25: [schema changed](../../deltas/2026-10-25/9b5c6962987b04112709.json): `2 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.bumblebox.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
