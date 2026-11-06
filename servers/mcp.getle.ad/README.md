# mcp.getle.ad: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.getle.ad.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.getle.ad/mcp` | 35 | [`a678ba2f194f`](cbf2049430c50fa8f3ec.json) | 2026-09-27 |

## Tools at `https://mcp.getle.ad/mcp`

- `add_leads_to_list`: `Append leads to a list, at most 500 per call. Duplicates inside the list are skipped. Use this to save rows returned by search_b2b_leads or…`
- `check_deliverability`: `Inspect SPF, DKIM, DMARC and MX for a domain. Run it on your own sending domains before a campaign, or on a prospect's domain to judge whet…`
- `control_campaign`: `Change the run state of a campaign. 'stop' is permanent: a stopped campaign cannot be resumed, so confirm with the user before stopping.`
- `create_campaign`: `Queue a cold email campaign against a lead list. It starts sending as soon as the worker picks it up, so show the user the final subject, b…`
- `create_list`: `Create an empty lead list. Use add_leads_to_list to fill it.`
- `crm_leads`: `Leads in the CRM pipeline with their stage and value. Filter by stage to see what needs work. Requires a plan with CRM access.`
- `crm_update_lead`: `Change a CRM lead's pipeline stage, deal value or notes.`
- `delete_list`: `Permanently delete a list and every lead in it. Irreversible: ask the user first, then call again with confirm true.`
- `draft_reply`: `Ask Getlead to draft an answer to a lead using the conversation context. Returns plain text you can edit before sending with send_reply. No…`
- `email_templates`: `Read the workspace's saved email templates so a campaign can reuse proven copy.`
- `enrich_lead`: `Look up a person or company and enrich it with public profile and company data (role, company details, social profiles). Give a LinkedIn or…`
- `export_list_csv`: `Return list contents as CSV text, at most 1000 rows. Use it to hand the data to the user or another tool; do not use it to page through a l…`
- `find_email`: `Find a person's work email address from their first name, last name and company domain (e.g. Jane Doe at acme.com). Tries the common corpor…`
- `get_account`: `Plan, entitlements and remaining credits for the connected Getlead workspace. Call this first: it tells you how many B2B leads, scraped lea…`
- `get_campaign_analytics`: `Open, click, reply and bounce breakdown over time for one campaign. Requires a plan with campaign analytics.`
- `get_campaign_stats`: `Delivery and engagement counters for one campaign: sent, failed, opens, clicks, replies.`
- `get_inbox`: `Replies received across every connected mailbox, newest first. Use filter 'unread' for triage and 'opportunity' for the ones Getlead flagge…`
- `get_list_leads`: `Leads inside one list, at most 200 per call. Filter by verification status to see what a campaign would actually send to.`
- `get_thread`: `The full conversation with one lead: what was sent, what they replied, and the tracking events. Read this before drafting an answer. Lead-w…`
- `list_campaigns`: `Every campaign in the workspace with status and send counts.`
- `list_lists`: `Every lead list in the workspace with its id and lead count. Lists are what campaigns and bulk verification operate on.`
- `list_mailboxes`: `Connected sending mailboxes (SMTP, Gmail OAuth, API providers) with their id, from address and active flag. Use the id when creating a camp…`
- `list_opportunities`: `Replies Getlead classified as opportunities, with their status and estimated value.`
- `preview_b2b_leads`: `Find B2B leads, prospects or contacts for an ideal customer profile and see how many exist before spending anything: job titles, seniority,…`
- `scrape_job_leads`: `Leads produced by a finished scrape job, capped at 200 rows per call.`
- `scrape_job_status`: `Progress of a scrape job started with scrape_leads_start.`
- `scrape_leads_start`: `Queue a background scrape for fresh leads from the web and social platforms. Returns a job_id immediately; poll scrape_job_status and then…`
- `search_b2b_leads`: `Find B2B leads, prospects or decision makers with their work emails: search the contact database by job title, seniority, department, indus…`
- `send_reply`: `Send a real email to a lead from the mailbox that owns the conversation, threaded onto it. This reaches a real person immediately: show the…`
- `suppression`: `Read suppression stats or add addresses that must never be emailed again. Suppressed addresses are skipped by every campaign automatically.`
- `test_mailbox`: `Send Getlead's connection test for one mailbox to confirm it can authenticate and send. Use it before launching a campaign from a mailbox t…`
- `update_opportunity`: `Change the status, estimated value or notes of an opportunity.`
- `verify_email`: `Check whether an email address exists and is safe to send to, with a real SMTP handshake. Free. Returns valid, invalid, catchall, disposabl…`
- `verify_list_start`: `Start bulk verification for every address in a list. Returns immediately with a job; poll verify_list_status. Lead rows get their email_sta…`
- `verify_list_status`: `Progress and result breakdown (valid, invalid, catch-all, disposable, unknown) for a list verification job.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.getle.ad/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
