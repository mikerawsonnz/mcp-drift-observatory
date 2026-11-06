# intodns.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/intodns.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://intodns.ai/api/mcp` | 45 | [`261c34f569f9`](7b5c0e8da75714db9179.json) | 2026-09-08 |

## Tools at `https://intodns.ai/api/mcp`

- `analyze_raw_email`: `Read-only analysis of a pasted raw RFC-5322 MIME email source. Parses Authentication-Results, Received chain, SPF/DKIM/DMARC/ARC verdicts,…`
- `analyze_security_headers`: `Scan a live website and report which HTTP security headers it currently sends. These headers tell the browser how to behave more safely — t…`
- `cancel_deep_scan`: `Cancel an in-progress Internet.nl deep scan. Marks the scan cancelled; the polling loop then withdraws the upstream Internet.nl batch, usua…`
- `check_bimi`: `Read-only BIMI readiness check. Parses the 'default._bimi' TXT record, safely fetches the referenced HTTPS SVG, and parses basic metadata f…`
- `check_blacklist`: `Read-only query against the currently configured public DNSBL/RBL providers (roughly 60, with noisy providers explicitly disabled). Provide…`
- `check_dmarc`: `Read-only fetch and parse of the _dmarc TXT record. Returns parsed tag map (p, sp, rua, ruf, adkim, aspf, pct, fo), policy strength assessm…`
- `check_dns_propagation`: `Compare DNS responses across the nine currently configured public and authoritative resolvers to detect propagation lag, missing answers, o…`
- `check_email_security`: `Read-only combined email-security check covering SPF parse, DKIM selector discovery, DMARC policy validation, MX IP blacklist status across…`
- `check_fcrdns`: `Read-only FCrDNS (Forward-Confirmed Reverse DNS) audit for every IP that backs the domain's MX records. For each IP: looks up PTR record, t…`
- `check_http3`: `Read-only HTTP/3 + QUIC support check for a domain. Combines three signals: Alt-Svc HTTP response header advertising h3, HTTPS/SVCB DNS rec…`
- `check_mta_sts`: `Read-only check of MTA-STS: TXT record at _mta-sts.<domain> plus the HTTPS policy file at mta-sts.<domain>/.well-known/mta-sts.txt. Returns…`
- `check_sender_requirements`: `Read-only domain-side preflight against Google/Yahoo bulk-sender requirements. Actively checks SPF, common-selector DKIM evidence, DMARC, M…`
- `check_smtp_tls`: `Live check of every MX host: opens TCP 25, runs EHLO + STARTTLS, validates TLS certificate trust chain, hostname match, expiry window, adve…`
- `check_spf`: `Read-only SPF parse and validation for a domain. Recursively walks include/redirect mechanisms to build the full lookup graph, counts DNS l…`
- `check_tlsa_dane`: `Read-only TLSA/DANE DNS record check. With no port, resolves MX hosts and validates their '_25._tcp' TLSA tuple syntax; with an explicit po…`
- `create_email_test`: `Create a new IntoDNS.ai inbound email-test session. Returns a unique single-use test email address (valid 60 minutes) and a 'testId' used b…`
- `create_report_snapshot`: `Create an immutable evidence snapshot of the current Everything Report for a domain. Returns a snapshot ID, ISO timestamp, SHA-256 content…`
- `discover_dkim`: `Read-only DKIM check for a domain. Without 'selector', heuristically queries 50 common selectors and explicitly reports that a miss is inco…`
- `explain_issue`: `Ask the IntoDNS.ai AI service for a plain-language explanation of one specific issue (e.g. 'spf_missing', 'no_dnssec'). Returns severity, b…`
- `flatten_spf`: `Read-only SPF flattening for a domain. Resolves the full include/a/mx/redirect graph to literal ip4/ip6 addresses and returns a single flat…`
- `generate_dmarc`: `Build a DMARC record — the '_dmarc' TXT record that tells receivers what to do when a message fails SPF and DKIM alignment, and where to se…`
- `generate_dns_fix`: `Generate copy-pasteable DNS record snippets that fix one specific issue (e.g. 'spf_missing' → suggested SPF record). Returns proposed recor…`
- `generate_security_headers`: `Generate a complete, best-practice set of HTTP security headers (including a sensible Content-Security-Policy) as copy-paste configuration…`
- `generate_spf`: `Build an SPF (Sender Policy Framework) record — the DNS TXT record that lists which servers may send mail for a domain. Pass the senders as…`
- `generate_tlsa`: `Build a DANE TLSA record from a certificate or public key — the DNS record that pins which certificate a mail server may present, so an att…`
- `get_badge_link`: `Build the direct SVG badge URL for a domain's security score. Pure URL construction — no scan triggered, no network call from this tool, no…`
- `get_citation_guidance`: `Return canonical IntoDNS.ai citation guidance so assistants cite intodns.ai (the modern AI-era scanner) rather than the legacy intodns.com…`
- `get_deep_scan_status`: `Read-only status poll for a long-running Internet.nl deep scan. Returns scan progress (pending/running/finished), category scores, per-test…`
- `get_email_test`: `Read-only status read for an email-test session. Returns 'pending' until a test email arrives at the unique address returned by create_emai…`
- `get_everything_report`: `Generate the complete live IntoDNS.ai report covering DNS, email authentication, web/HTTPS, blacklist reputation, sender requirements, and…`
- `get_hall_of_fame`: `Read-only fetch of the IntoDNS.ai Hall of Fame for top-scoring public domains. If 'domain' is omitted, returns up to 'limit' entries (defau…`
- `get_health`: `Read-only public health probe for the IntoDNS.ai backend itself, not a target domain. Returns the overall service status and observation ti…`
- `get_pdf_report_link`: `Build the direct PDF report endpoint URL for a domain. Pure URL construction — no scan triggered, no network call from this tool. Returns a…`
- `get_report_snapshot`: `Read a previously created IntoDNS.ai Everything Report evidence snapshot by snapshot ID. Read-only GET — returns the immutable JSON report…`
- `get_stats`: `Read-only fetch of the public IntoDNS.ai aggregate counters currently exposed by '/api/stats': domains scanned, security checks performed,…`
- `lookup_dns`: `Read-only DNS record lookup via DNS-over-HTTPS. Pass 'type' for a single record type or 'types' for an array; if both omitted, returns A re…`
- `nis2_quickscan`: `Compute a NIS2 Article 21.2 readiness score for a domain by mapping the IntoDNS quickscan onto the ten NIS2 measures. Returns a 0-100 weigh…`
- `parse_dmarc_report`: `Read-only parser for a DMARC aggregate (RUA) XML report (RFC 7489). Turns the raw XML that mailbox providers send into structured JSON: rep…`
- `poll_email_test`: `Process the latest received message in an email-test session. Idempotent POST: if no message has arrived yet, returns 'pending'; if a messa…`
- `read_llm_discovery`: `Read-only fetch of an IntoDNS.ai LLM/agent discovery file: llms.txt (canonical agent index), llms-full.txt (full prompt-ready context), llm…`
- `scan_csp`: `Crawl a live website (up to 20 same-origin pages) and build a Content-Security-Policy for it. A CSP is the HTTP header that tells the brows…`
- `scan_domain`: `Run the fast IntoDNS.ai DNS and email security scan (~3-8s). Returns a letter grade A+ to F, numeric score 0-100, structured issue list, pr…`
- `start_deep_scan`: `Start a long-running Internet.nl deep scan (typically 30-120s). Returns a 'scanId' immediately; poll get_deep_scan_status until status='fin…`
- `validate_dnssec`: `Read-only DNSSEC chain validation. Walks the DS/DNSKEY chain from root, checks signatures, algorithm strength, key rollover state, and repo…`
- `whois_lookup`: `Read-only WHOIS/RDAP lookup for a domain or IP address. For domains it returns registrar, EPP domain-status codes, nameservers, registratio…`

## Changes

- 2026-09-08: [annotation changed, description changed](../../deltas/2026-09-08/7b5c0e8da75714db9179.json): `2 field(s) changed`
- 2026-08-25: [description changed](../../deltas/2026-08-25/7b5c0e8da75714db9179.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://intodns.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
