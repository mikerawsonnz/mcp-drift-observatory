# api.bowmark.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.bowmark.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.bowmark.ai/mcp` | 35 | [`a6605af9fe7e`](5f2d24be930573ed8878.json) | 2026-11-08 |
| `https://api.bowmark.ai/mcp/registry` | 35 | [`a6605af9fe7e`](e742a173e323c903336e.json) | 2026-11-08 |

## Tools at `https://api.bowmark.ai/mcp`

- `add_connection`: `Get a sign-in link for one site, so the user can sign Bowmark in to it right now, before any run needs it. Pass the site as a domain ('yout…`
- `delete_connection`: `Start deleting a saved login by the 'id' 'list_connections' returned. **This does not delete anything by itself:** a delete cannot be undon…`
- `get_library`: `**Use this whenever a task touches a live website.** It answers whether Bowmark can already DO the thing: current prices, real availability…`
- `get_secret_link`: `Return the dashboard link for one stored secret this account holds, so you can answer "where is my Acme password?" with somewhere to go. **…`
- `get_usage`: `See the real cost of calls on this account, itemized by resource (provider calls, browser sessions, IP leases) and aggregated in dollars. P…`
- `jig_cache`: `Used by an open jig to save a call's last good result. You do not need to call this.`
- `jig_call`: `Used by an open jig to call the library. You do not need to call this — use 'run'.`
- `jig_get`: `Copy someone's published jig into THIS user's account, from its current version. The copy is the user's own: it runs as them with their log…`
- `jig_list`: `The jigs this user has, newest change first: id, slug, title, the built-in it started from, and when it last changed. A copy of someone's p…`
- `jig_look`: `See what an open jig is showing the user right now — the items on screen, which view they are on — plus what they just did on it (watched,…`
- `jig_open`: `Make the user a "jig": their own copy of a website, that you curate as they talk. Asked for "a jig of YouTube", build a page that LOOKS lik…`
- `jig_perf`: `Used by an open jig to report how fast it loaded. You do not need to call this.`
- `jig_publish`: `Publish the user's jig (name it by 'jigId' or your jig's 'jigSlug') as a listing others can get: it snapshots the page and state AS THEY AR…`
- `jig_pull_update`: `For a jig the user got from someone's listing ('jig_list' shows 'updateAvailable'): the three pages a merge needs. 'base' is the version th…`
- `jig_read`: `List a jig's files with their byte sizes, or with 'path' read one file's text. A page written as 'html' is one file, index.html. Read befor…`
- `jig_search`: `Search the public jigs other people published: "is there a jig for my Amazon orders?". Call it BEFORE building a page from scratch. Leave '…`
- `jig_seen`: `Used by an open jig to report what it shows. You do not need to call this.`
- `jig_set_handle`: `Claim the user's public handle: the @name in the links to pages they publish, bowmark.ai/jigs/@<handle>/<slug>. It is PUBLIC and PERMANENT:…`
- `jig_update`: `Change a page you opened with 'jig_open': merge 'state' into its state (a key set to null is removed), replace its 'html' or 'title', or ch…`
- `jig_view`: `Used by an open jig to pick up its latest state. You do not need to call this.`
- `lease_ip`: `Some sites (LinkedIn, marked 📍 in 'get_library') only accept a login from the address it signed in from. A dedicated IP is one address that…`
- `list_connections`: `List the saved logins this account already holds, one entry per login: its 'id' (name it in a signed-in call as '{ connection: id }'), the…`
- `list_secrets`: `List the stored secrets this account holds, by NAME. Returns name, type, which hosts each may be used against, when it expires and when it…`
- `llm_answer`: `Answers one job from llm_poll. 'answer' must be an object matching that job's inputSchema. A wrong shape is refused with the reason and the…`
- `llm_detach`: `Detaches this chat at once, so open Bowmark pages' AI calls go back to Bowmark's own model instead of waiting for this chat.`
- `llm_poll`: `Lets this chat answer the AI calls an open Bowmark page makes, so they cost nothing. Returns up to 5 pending jobs ({ jobId, system, prompt,…`
- `logout_connection`: `Sign a saved login out by the 'id' 'list_connections' returned. Bowmark drops the cookies it held, and where the site supports it ('siteLog…`
- `report`: `Record what was missing, wrong, or incomplete so Bowmark can build it. Call it yourself, in the same turn, without asking your user first:…`
- `request_secret`: `Create a named, empty slot for a secret and get back a link the user opens to fill it in. They type the value on a Bowmark page and choose…`
- `run`: `**Executes the task on the real websites** and returns the result. Call 'get_library' FIRST, then start with 'run({ script })' — never add…`
- `run_view`: `Used by the inline run view to draw a run's progress. You do not need to call this — 'run' returns the result.`
- `session_call`: `Runs ONE library function in a Bowmark session, so a flow that needs several calls in the SAME session can finish: a booking that texts the…`
- `session_close`: `Ends a session 'session_call' opened and frees what it held. Pass the 'sessionId'. Closing one that is already closed is harmless.`
- `support`: `Chat live with a Bowmark support agent about a problem you reported. Use it only after your user said yes to talking to support. Pass the '…`
- `wait_for_sign_in`: `Wait until the user finishes a sign-in link, so you know the moment they are done without asking them. Pass 'ref': 'meta.handoff.ref' from…`

## Tools at `https://api.bowmark.ai/mcp/registry`

- `add_connection`: `Get a sign-in link for one site, so the user can sign Bowmark in to it right now, before any run needs it. Pass the site as a domain ('yout…`
- `delete_connection`: `Start deleting a saved login by the 'id' 'list_connections' returned. **This does not delete anything by itself:** a delete cannot be undon…`
- `get_library`: `**Use this whenever a task touches a live website.** It answers whether Bowmark can already DO the thing: current prices, real availability…`
- `get_secret_link`: `Return the dashboard link for one stored secret this account holds, so you can answer "where is my Acme password?" with somewhere to go. **…`
- `get_usage`: `See the real cost of calls on this account, itemized by resource (provider calls, browser sessions, IP leases) and aggregated in dollars. P…`
- `jig_cache`: `Used by an open jig to save a call's last good result. You do not need to call this.`
- `jig_call`: `Used by an open jig to call the library. You do not need to call this — use 'run'.`
- `jig_get`: `Copy someone's published jig into THIS user's account, from its current version. The copy is the user's own: it runs as them with their log…`
- `jig_list`: `The jigs this user has, newest change first: id, slug, title, the built-in it started from, and when it last changed. A copy of someone's p…`
- `jig_look`: `See what an open jig is showing the user right now — the items on screen, which view they are on — plus what they just did on it (watched,…`
- `jig_open`: `Make the user a "jig": their own copy of a website, that you curate as they talk. Asked for "a jig of YouTube", build a page that LOOKS lik…`
- `jig_perf`: `Used by an open jig to report how fast it loaded. You do not need to call this.`
- `jig_publish`: `Publish the user's jig (name it by 'jigId' or your jig's 'jigSlug') as a listing others can get: it snapshots the page and state AS THEY AR…`
- `jig_pull_update`: `For a jig the user got from someone's listing ('jig_list' shows 'updateAvailable'): the three pages a merge needs. 'base' is the version th…`
- `jig_read`: `List a jig's files with their byte sizes, or with 'path' read one file's text. A page written as 'html' is one file, index.html. Read befor…`
- `jig_search`: `Search the public jigs other people published: "is there a jig for my Amazon orders?". Call it BEFORE building a page from scratch. Leave '…`
- `jig_seen`: `Used by an open jig to report what it shows. You do not need to call this.`
- `jig_set_handle`: `Claim the user's public handle: the @name in the links to pages they publish, bowmark.ai/jigs/@<handle>/<slug>. It is PUBLIC and PERMANENT:…`
- `jig_update`: `Change a page you opened with 'jig_open': merge 'state' into its state (a key set to null is removed), replace its 'html' or 'title', or ch…`
- `jig_view`: `Used by an open jig to pick up its latest state. You do not need to call this.`
- `lease_ip`: `Some sites (LinkedIn, marked 📍 in 'get_library') only accept a login from the address it signed in from. A dedicated IP is one address that…`
- `list_connections`: `List the saved logins this account already holds, one entry per login: its 'id' (name it in a signed-in call as '{ connection: id }'), the…`
- `list_secrets`: `List the stored secrets this account holds, by NAME. Returns name, type, which hosts each may be used against, when it expires and when it…`
- `llm_answer`: `Answers one job from llm_poll. 'answer' must be an object matching that job's inputSchema. A wrong shape is refused with the reason and the…`
- `llm_detach`: `Detaches this chat at once, so open Bowmark pages' AI calls go back to Bowmark's own model instead of waiting for this chat.`
- `llm_poll`: `Lets this chat answer the AI calls an open Bowmark page makes, so they cost nothing. Returns up to 5 pending jobs ({ jobId, system, prompt,…`
- `logout_connection`: `Sign a saved login out by the 'id' 'list_connections' returned. Bowmark drops the cookies it held, and where the site supports it ('siteLog…`
- `report`: `Record what was missing, wrong, or incomplete so Bowmark can build it. Call it yourself, in the same turn, without asking your user first:…`
- `request_secret`: `Create a named, empty slot for a secret and get back a link the user opens to fill it in. They type the value on a Bowmark page and choose…`
- `run`: `**Executes the task on the real websites** and returns the result. Call 'get_library' FIRST, then start with 'run({ script })' — never add…`
- `run_view`: `Used by the inline run view to draw a run's progress. You do not need to call this — 'run' returns the result.`
- `session_call`: `Runs ONE library function in a Bowmark session, so a flow that needs several calls in the SAME session can finish: a booking that texts the…`
- `session_close`: `Ends a session 'session_call' opened and frees what it held. Pass the 'sessionId'. Closing one that is already closed is harmless.`
- `support`: `Chat live with a Bowmark support agent about a problem you reported. Use it only after your user said yes to talking to support. Pass the '…`
- `wait_for_sign_in`: `Wait until the user finishes a sign-in link, so you know the moment they are done without asking them. Pass 'ref': 'meta.handoff.ref' from…`

## Changes

- 2026-11-08: [annotation changed, count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-11-08/e742a173e323c903336e.json): `1 tool(s) added; 22 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-11-08: [annotation changed, count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-11-08/5f2d24be930573ed8878.json): `1 tool(s) added; 22 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-11-07: [annotation changed, count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-11-07/5f2d24be930573ed8878.json): `1 tool(s) added; 51 field(s) changed`
- 2026-11-07: [annotation changed, count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-11-07/e742a173e323c903336e.json): `1 tool(s) added; 51 field(s) changed`
- 2026-11-06: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-06/e742a173e323c903336e.json): `7 tool(s) added; 10 field(s) changed; signals: imperative_language_introduced` **(notable)**
- 2026-11-06: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-06/5f2d24be930573ed8878.json): `7 tool(s) added; 10 field(s) changed; signals: imperative_language_introduced` **(notable)**
- 2026-11-04: [annotation changed, description changed, field changed, schema changed](../../deltas/2026-11-04/e742a173e323c903336e.json): `29 field(s) changed`
- 2026-11-04: [annotation changed, description changed, field changed, schema changed](../../deltas/2026-11-04/5f2d24be930573ed8878.json): `29 field(s) changed`
- 2026-11-03: [description changed, field changed, schema changed](../../deltas/2026-11-03/e742a173e323c903336e.json): `14 field(s) changed`
- 2026-11-03: [description changed, field changed, schema changed](../../deltas/2026-11-03/5f2d24be930573ed8878.json): `14 field(s) changed`
- 2026-11-02: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-02/e742a173e323c903336e.json): `2 tool(s) added; 24 field(s) changed; signals: imperative_language_introduced` **(notable)**
- 2026-11-02: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-02/5f2d24be930573ed8878.json): `2 tool(s) added; 24 field(s) changed; signals: imperative_language_introduced` **(notable)**
- 2026-11-01: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-01/e742a173e323c903336e.json): `1 tool(s) added; 27 field(s) changed`
- 2026-11-01: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-01/5f2d24be930573ed8878.json): `1 tool(s) added; 27 field(s) changed`
- 2026-10-31: [annotation changed, schema changed](../../deltas/2026-10-31/e742a173e323c903336e.json): `14 field(s) changed`
- 2026-10-31: [annotation changed, schema changed](../../deltas/2026-10-31/5f2d24be930573ed8878.json): `14 field(s) changed`
- 2026-10-30: [annotation changed, description changed](../../deltas/2026-10-30/5f2d24be930573ed8878.json): `18 field(s) changed`
- 2026-10-30: [annotation changed, description changed](../../deltas/2026-10-30/e742a173e323c903336e.json): `18 field(s) changed`
- 2026-10-29: [count changed, tool added](../../deltas/2026-10-29/5f2d24be930573ed8878.json): `7 tool(s) added; signals: imperative_language_introduced` **(notable)**
- 2026-10-29: [count changed, tool added](../../deltas/2026-10-29/e742a173e323c903336e.json): `7 tool(s) added; signals: imperative_language_introduced` **(notable)**

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.bowmark.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
