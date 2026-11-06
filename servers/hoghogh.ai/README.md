# hoghogh.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/hoghogh.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://hoghogh.ai/mcp` | 19 | [`487254ddc754`](f6d5640e85d221ac25e9.json) | 2026-09-12 |

## Tools at `https://hoghogh.ai/mcp`

- `calculate_delay_penalty`: `Calculate خسارت تأخیر تأدیه under art. 522 ق.آ.د.م using the Central Bank price index. The index series is official data — never approximat…`
- `calculate_diyeh`: `Calculate دیه for a bodily injury using the CURRENT official rate and the fractions set by قانون مجازات اسلامی. ALWAYS use this instead of…`
- `calculate_inheritance`: `Calculate Iranian inheritance shares (سهم‌الارث) under قانون مدنی arts. 862–949, including حجب نقصانی reduction rules. The jurisprudential…`
- `calculate_lawyer_fee`: `Calculate حق‌الوکاله from آیین‌نامهٔ تعرفهٔ حق‌الوکاله (1398/12/28): financial claims are a marginal ladder on the claim value (art. 9); fa…`
- `calculate_litigation_fee`: `Calculate Iranian court filing fees (هزینهٔ دادرسی) for a monetary claim at a given stage (بدوی / تجدیدنظر / فرجام), using the current offi…`
- `calculate_mahrieh`: `Calculate the present-day value of a مهریه: coins at the live market rate, and any cash portion adjusted by the Central Bank index (تبصرهٔ…`
- `calculate_notary_fee`: `Calculate حق‌التحریر (the notary office's fee) from the official 1405 tariff for دفاتر اسناد رسمی. Distinct from حق‌الثبت (use calculate_st…`
- `calculate_severance`: `Calculate an Iranian employee's end-of-service entitlements (حق سنوات، عیدی، مانده مرخصی) under قانون کار, using the current official minim…`
- `calculate_stamp_duty`: `Calculate حق‌الثبت (registration duty) for property, vehicle, company, marriage and divorce documents. Distinct from حق‌التحریر (the notary…`
- `calculate_tax`: `Calculate Iranian salary, property-transfer, inheritance or rental tax. For inheritance: rates depend on asset kind and heir class (arts. 1…`
- `lookup_annual_rate`: `Fetch official Iranian yearly rates from the database: minimum wage (min_wage), court filing fees (court_fee_*), salary tax exemption (sala…`
- `lookup_law_article`: `Fetch the VERBATIM text of a specific article when you already know the law and the article number (e.g. «ماده ۱۰ قانون مدنی»). Use this to…`
- `lookup_procedure`: `Look up Iranian procedural deadlines (مهلت تجدیدنظر، واخواهی، اعتراض ثالث، اجرای حکم…) with the governing law and article, by case type. Us…`
- `lookup_sentencing_range`: `Look up the statutory punishment for an Iranian crime — imprisonment, fine, lashes, قصاص, دیه — with the governing article. Use when the us…`
- `lookup_statute_of_limitations`: `Check Iranian limitation periods (مرور زمان) — prosecution, execution, and filing deadlines — for a case category. Use when the user asks w…`
- `search_advisory_opinions`: `Search the advisory opinions (نظریات مشورتی) of the Judiciary's legal department (اداره کل حقوقی قوه قضائیه) — the official, citable interp…`
- `search_case_law`: `Search 31,000+ Iranian court rulings and آرای وحدت رویه (binding precedent). Use when the user asks how courts have actually decided an iss…`
- `search_circular`: `Search official circulars and directives (بخشنامه‌ها) from the judiciary and government bodies — the source of current official RATES and p…`
- `search_law_articles`: `Semantic + keyword search across the full text of Iranian statutes (50,000+ articles: قانون مدنی، مجازات اسلامی، کار، تجارت، آیین دادرسی و……`

## Changes

- 2026-09-12: [description changed, schema changed](../../deltas/2026-09-12/f6d5640e85d221ac25e9.json): `28 field(s) changed; signals: length_more_than_doubled`
- 2026-09-07: [annotation changed, description changed](../../deltas/2026-09-07/f6d5640e85d221ac25e9.json): `77 field(s) changed`
- 2026-09-04: [schema changed](../../deltas/2026-09-04/f6d5640e85d221ac25e9.json): `77 field(s) changed; signals: length_more_than_doubled`
- 2026-09-02: [description changed](../../deltas/2026-09-02/f6d5640e85d221ac25e9.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://hoghogh.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
