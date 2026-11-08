# api.betslipdoctor.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.betslipdoctor.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.betslipdoctor.ai/api/mcp` | 94 | [`b0e0754fa889`](f29327f2a9147dd897c0.json) | 2026-11-08 |

## Tools at `https://api.betslipdoctor.ai/api/mcp`

- `account_settings`: `Read and change this account through its signed-in product routes. Change AI and model-training privacy settings in the app. Sportsbook act…`
- `add_doctor_parlay_to_slip`: `Put one of the Doctor’s posted parlays (key from get_doctor_parlays) on this account’s slip in one step, with a unique commandKey. Checks e…`
- `cancel_doctor_reply`: `Cancel an owned Doctor jobId under the app cancellation and reservation rules. Cannot undo a reply or provider work already completed. Reus…`
- `cancel_grade`: `Cancel an owned Grade jobId through the app service. Stops eligible work and releases its remaining reservation under the existing app rule…`
- `check_slip`: `The app slip’s rule for this conversation’s slip. Send legs (ids plus the oddsAmerican, line, observedAt and startsAt they were added with)…`
- `connect_sportsbook`: `Return a 10-minute betslipdoctor.ai link (linkUrl, expiresAt) for the customer to open and finish connecting a sportsbook. The app checks t…`
- `copy_tail_slip`: `After the customer reviews every current leg and confirms the exact stake/currency/settlement fields, save the app’s owned Tail/Fade ticket…`
- `create_api_key`: `After the customer asks to create a personal API key, send its name and requested scopes. The scopes must be a subset of this connection’s…`
- `create_tracked_slip`: `After the customer asks to save it, save one app ticket (the quote_grade ticket contract) to this account's saved slips through the app's P…`
- `disconnect_sportsbook`: `Disconnect an owned linked sportsbook accountId, the same as the app’s Disconnect: BSD imports for it stop at once and the link to your spo…`
- `doctor_actions`: `The Doctor actions beside the conversation, as the app does them. Record a decision only when the customer says what they did; change memor…`
- `doctor_conversation`: `Read or change a Doctor conversation with version bsd-agent-doctor-v1 and an action; the individual Doctor tools omit version and action. F…`
- `export_betting_history`: `Read one real CSV export page for the owned History filters. Returns complete/next, filename and CSV. Never call a partial page a full expo…`
- `fade_post`: `Preview actual supported opposite selections for a visible Tail post at the customer’s bookId and jurisdiction. Unavailable legs remain una…`
- `fix_grade_leg`: `The app’s Fix it on an owned saved Grade jobId whose get_grade_report says fixable.offered: the Doctor reprices, swaps or drops weak legs a…`
- `forget_doctor_note`: `Remove the exact owned note only after the customer explicitly asks to forget it. Requires current id/expectedRevision and confirmation for…`
- `get_betting_leaks`: `Read deterministic patterns from this account’s settled betting history, with coverage, sample sizes, thresholds and source ticket IDs.`
- `get_bettor_profile`: `Read this authenticated account’s bettor model, optionally filtered by topic: confirmed notes and revisions, separately attributed Honcho i…`
- `get_box_score`: `Read the in-play or final score and box score for one game (eventId from search_markets or the board), the same read as the app’s Live game…`
- `get_doctor_conversation`: `Read the owned threadId, saved user messages, Doctor answers and jobs; optional before pages older messages. Does not generate a new answer.`
- `get_doctor_events`: `Read saved events for the owned Doctor jobId, optionally after a sequence. Never starts a consult.`
- `get_doctor_job`: `Read the owned Doctor jobId, including its real saved answer when available. Never generates or restarts a reply.`
- `get_doctor_memory`: `Read this authenticated account’s confirmed notes, active status, current revisions and memory generation. Longer-term Honcho personalizati…`
- `get_doctor_parlays`: `Read the Doctor’s posted parlays for one league (e.g. LGUE_nfl): 2-3 legs on different games, each B+ or better when posted. Upcoming first…`
- `get_doctor_picks`: `Read today’s saved Doctor picks and recent settled WON/LOST/PUSH results. Each item carries league (first leg’s league id), sport (first le…`
- `get_doctor_quota`: `Read this account’s current app consult allowance, held and used amounts, and reset information. Does not reserve a consult.`
- `get_grade_catalog`: `Read this account’s Grade research options and available capabilities, including in-play eligibility when enabled. Does not start a Grade.`
- `get_grade_evidence`: `Return the evidence behind an owned completed Grade jobId: each claim checked (price, injury and lineup, matchup, form, line move, situatio…`
- `get_grade_groups`: `Read the owned Grade job’s group scores as they become available. Status is pending, partial or final; partial scores can change and are no…`
- `get_grade_job`: `Read the owned Grade jobId and its current durable status. Never starts or resumes work.`
- `get_grade_progress`: `Read saved progress for the owned Grade jobId, with optional after sequence and limit 1-100. Progress is not proof that a saved report is r…`
- `get_grade_report`: `Return the verified saved report for a completed Grade this account owns, by jobId. Returns unavailable until the saved report is readable;…`
- `get_history_summary`: `The authenticated account's app History summary (GET history/summary): record, stake and net over the chosen range, with its source, curren…`
- `get_league_order`: `Read BetSlip Doctor’s league order right now: the same leagues in the same order as the app’s league strip (its Home and Odds chips: games…`
- `get_plan`: `Read this account’s BetSlip Doctor plan exactly as the app shows it: the plan (free, starter, pro or elite), where it is paid (paymentSourc…`
- `get_player_research`: `Research a player and his prop the way the Doctor does: his last 5 and last 10 games against his season average and tonight’s line (overs,…`
- `get_saved_reports`: `Read the saved Grade jobs and reports behind list_grade_jobs, get_grade_job, get_grade_progress, get_grade_groups, get_grade_report, get_gr…`
- `get_tail_feed`: `Doctor ticket posts include result WON/LOST/PUSH when settled, null otherwise. Read the app Tail feed with its account-filtered community,…`
- `get_tail_post`: `Doctor ticket posts include result WON/LOST/PUSH when settled, null otherwise. Read one app Tail postId visible to this account under the s…`
- `get_todays_board`: `The app Live board (GET live/board): upcoming and in-play games, each with mainLines: its DraftKings game lines (slot, line, odds), optiona…`
- `get_tracked_slips`: `Read the authenticated account's saved-ticket library: the same list the app shows (GET tickets), newest first, with optional search, limit…`
- `grade_pickem_entry`: `Use action settlement with ticketId to read this owned entry’s result (history.read also required). Use bsd-pickem-grade-v2. check returns…`
- `grade_settings`: `Read or save this account’s Grade risk preference, analysis depth and unit size. Saving requires the exact confirmed settings, current revi…`
- `grade_slip`: `Combined form of quote_grade, start_grade and cancel_grade (same fields, same answers): version bsd-agent-grade-v1, action quote, start or…`
- `history_actions`: `Write this account's History as the app does. Record a bet only when the customer says they placed it. report_advice_response: POST history…`
- `list_api_keys`: `List your active personal BetSlip Doctor API keys (name, display prefix, scopes, created, last used). Secrets are never returned.`
- `list_connected_agents`: `List the agents (OAuth apps) connected to your BetSlip Doctor account: name, scopes, connected and last used.`
- `list_doctor_conversations`: `Read this account’s saved app Doctor threads. Does not generate an answer.`
- `list_grade_jobs`: `Read the authenticated account’s current Grade library, with optional limit 1-20 and account-bound cursor. Each row’s headline is its Rocky…`
- `list_linkable_sportsbooks`: `List the sportsbooks this account can link, the same list as the app’s Settings > Sportsbooks picker: each book (bookId, name, abbr) with t…`
- `list_sportsbooks`: `Read this account’s linked sportsbooks exactly as the app shows them: whether sportsbook linking is allowed, each account (accountId, book,…`
- `look_up_fact`: `Use the jobId of a Doctor consult already started after the customer accepted its quote. Send a planned fact, public subject names, league,…`
- `match_ticket_legs`: `For a betslip the customer showed you (screenshot, paste or their words): send each leg as printed (event, selection, market, period, line,…`
- `notifications`: `This account's notification inbox and settings, the same as the app's bell. feed: GET notifications/feed params {filter all/mentions/verifi…`
- `onboarding_preferences`: `Read the current league catalog and per-league team membership, or read/save your leagues and teams. Use original source-qualified IDs. Log…`
- `open_doctor_conversation`: `Persist an app Doctor thread, optionally attached to an owned ticket, report or history item. Does not start a reply or spend a consult all…`
- `prepare_sportsbook_handoff`: `Prepare the existing app’s fresh, vetted direct sportsbook link for an owned saved ticket. Choose the same sportsbook as the saved ticket a…`
- `preview_tail_post`: `Compute the exact app sharing preview and binding from an owned saved Grade report or Doctor exchange draft. Does not publish. Show the ret…`
- `preview_tail_slip`: `Show current supported prices for tailing or fading one visible public post at the customer’s chosen bookId and jurisdiction. Use original…`
- `price_shop_slip`: `Compare books on a saved slip, exactly the app's Compare books (POST tickets/compare-books): each leg's current price at up to 5 books (boo…`
- and 34 more in [f29327f2a9147dd897c0.json](f29327f2a9147dd897c0.json)

## Changes

- 2026-11-08: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-08/f29327f2a9147dd897c0.json): `2 tool(s) added; 2370 field(s) changed; signals: length_more_than_doubled, url_introduced`
- 2026-11-07: [description changed, schema changed](../../deltas/2026-11-07/f29327f2a9147dd897c0.json): `661 field(s) changed; signals: length_more_than_doubled, url_introduced`
- 2026-11-06: [annotation changed, description changed, field changed, schema changed](../../deltas/2026-11-06/f29327f2a9147dd897c0.json): `2136 field(s) changed; signals: length_more_than_doubled`
- 2026-11-03: [description changed](../../deltas/2026-11-03/f29327f2a9147dd897c0.json): `1 field(s) changed`
- 2026-11-01: [annotation changed, count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-11-01/f29327f2a9147dd897c0.json): `11 tool(s) added; 201 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-10-31: [description changed, schema changed](../../deltas/2026-10-31/f29327f2a9147dd897c0.json): `4 field(s) changed; signals: imperative_language_introduced` **(notable)**
- 2026-10-29: [description changed](../../deltas/2026-10-29/f29327f2a9147dd897c0.json): `1 field(s) changed`
- 2026-10-28: [description changed, schema changed](../../deltas/2026-10-28/f29327f2a9147dd897c0.json): `7 field(s) changed`
- 2026-10-26: [schema changed](../../deltas/2026-10-26/f29327f2a9147dd897c0.json): `4 field(s) changed`
- 2026-10-25: [description changed](../../deltas/2026-10-25/f29327f2a9147dd897c0.json): `1 field(s) changed`
- 2026-10-24: [description changed, schema changed](../../deltas/2026-10-24/f29327f2a9147dd897c0.json): `736 field(s) changed`
- 2026-10-23: [annotation changed, count changed, description changed, field changed, schema changed, tool added, tool removed](../../deltas/2026-10-23/f29327f2a9147dd897c0.json): `6 tool(s) added; 1 tool(s) removed; 1913 field(s) changed; signals: length_more_than_doubled`
- 2026-10-22: [count changed, description changed, schema changed, tool added, tool removed](../../deltas/2026-10-22/f29327f2a9147dd897c0.json): `21 tool(s) added; 7 tool(s) removed; 63 field(s) changed`
- 2026-10-19: [count changed, description changed, schema changed, tool added](../../deltas/2026-10-19/f29327f2a9147dd897c0.json): `6 tool(s) added; 71 field(s) changed`
- 2026-10-18: [count changed, description changed, schema changed, tool added](../../deltas/2026-10-18/f29327f2a9147dd897c0.json): `10 tool(s) added; 478 field(s) changed; signals: length_more_than_doubled, url_introduced`
- 2026-10-15: [annotation changed, description changed, field changed, schema changed](../../deltas/2026-10-15/f29327f2a9147dd897c0.json): `25 field(s) changed`
- 2026-10-13: [schema changed](../../deltas/2026-10-13/f29327f2a9147dd897c0.json): `20 field(s) changed`
- 2026-10-11: [annotation changed, description changed, schema changed](../../deltas/2026-10-11/f29327f2a9147dd897c0.json): `62 field(s) changed`
- 2026-10-10: [count changed, tool added](../../deltas/2026-10-10/f29327f2a9147dd897c0.json): `11 tool(s) added`
- 2026-10-09: [field changed](../../deltas/2026-10-09/f29327f2a9147dd897c0.json): `6 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.betslipdoctor.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
