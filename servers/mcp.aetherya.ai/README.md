# mcp.aetherya.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.aetherya.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.aetherya.ai/mcp` | 26 | [`1c6a54a7db7e`](0ec8f666c7c4e4781c4d.json) | 2026-11-21 |

## Tools at `https://mcp.aetherya.ai/mcp`

- `thesia_ask_audience`: `SECONDARY TOOL. Pose a question to a SINGLE synthetic persona and get one predicted, in-character response — good for an open-ended 'would…`
- `thesia_audit_site`: `Run a behavioral simulation of one page: simulated visitors from a simulated audience tour the page and report where they hesitate, get con…`
- `thesia_cancel`: `Stop a study, instant read, plan, audit or post simulation that is still running. Use it when the user changes their mind or a run was star…`
- `thesia_compare_creatives`: `Compare 2+ image creatives (thumbnails, display banners, social images) against a simulated audience. Creates the experiment, uploads the i…`
- `thesia_confirm_study`: `Respond to a plan from thesia_plan_study. Use action 'confirm' with accept_sessions to approve the quoted cost and start the run — this is…`
- `thesia_create_audience`: `Create synthetic-audience personas to simulate against. Describe who you want to model and get back personas (with ids) you can then target…`
- `thesia_create_intake_link`: `Create a secret upload link to send a client so they can drop creative files (images, video) for pretesting. Returns the url and expiry; tr…`
- `thesia_estimate`: `Quote how many simulation sessions a run would cost, and roughly what share of your plan it would consume, before committing to it. Free —…`
- `thesia_get_audit_result`: `Fetch the result of an audit started by thesia_audit_site, using its job_id. Returns the full simulated behavioral findings once complete,…`
- `thesia_get_brief`: `Turn a finished study, audit, read or post simulation into a short decision brief: the question, a direct answer, the reasoning with suppor…`
- `thesia_get_result`: `Fetch the findings of a run started by thesia_run_study, thesia_test_copy, thesia_audit_site, thesia_plan_study, thesia_read, thesia_simula…`
- `thesia_list_audiences`: `List the simulated audiences (simulated personas) in this workspace: their overall shape (where they are, what they do, how much is actuall…`
- `thesia_list_capabilities`: `List the research methods this workspace can run — with the exact stimulus fields each one requires — plus remaining plan headroom and simu…`
- `thesia_list_intake_files`: `List the files a client uploaded through an intake link (name, type, size, status, set label, a short-lived download url). The feature must…`
- `thesia_list_runs`: `List the workspace's recent simulations across studies, instant reads, plans, audits and post simulations, newest first, with the kind and…`
- `thesia_plan_study`: `Give Thesia a decision you need to make, in plain English, and it designs the study, picks or builds the audience, prices it, and runs it —…`
- `thesia_pretest_report`: `Assemble a markdown pretest report (how we worked, one section per set, what the results mean, sealed predictions appendix) from finished s…`
- `thesia_pretest_video`: `Pretest a short video (mp4, mov, webm; max 512 MB, 10 minutes) against a simulated audience: hook score, attention curve, drop-off points.…`
- `thesia_read`: `Myrias instant read. Reads 2-5 variants against a census-weighted synthetic population for a market, in seconds, and returns each variant's…`
- `thesia_record_outcome`: `Attach what actually happened to a sealed prediction (append-only) and get the evaluation. creative_comparison actual: {metric:'ctr', value…`
- `thesia_run_study`: `Run a Research Lab study — pricing sensitivity, message testing, concept testing, focus groups — against a simulated audience and get a str…`
- `thesia_seal_prediction`: `Lock a prediction (a creative comparison ranking, a video analysis, a study or a manual payload) with a SHA-256 hash and timestamp, so it c…`
- `thesia_share_result`: `Mint a shareable URL for a completed study, audit or creative comparison so someone without an Thesia account can read the findings. Use it…`
- `thesia_simulate_post`: `Run a post (X, LinkedIn, Instagram, Facebook) or email through a simulated audience and get predicted engagement, sentiment and representat…`
- `thesia_test_copy`: `Compare 2-5 copy variants — headlines, value propositions, ad or email copy — against a simulated audience, and get a ranked verdict with p…`
- `thesia_verify_prediction`: `Recompute the hash of a sealed prediction and report whether it still matches the stored one.`

## Changes

- 2026-11-21: [count changed, tool added, tool removed](../../deltas/2026-11-21/0ec8f666c7c4e4781c4d.json): `26 tool(s) added; 27 tool(s) removed; signals: imperative_language_introduced` **(notable)**

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.aetherya.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
