# mcp.bootpay.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.bootpay.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.bootpay.ai/mcp` | 9 | [`83177a4adc42`](a46719d28a156bbc76f4.json) | 2026-11-26 |

## Tools at `https://mcp.bootpay.ai/mcp`

- `detect_project_stack`: `🔍 사용자 프로젝트의 스택을 판정합니다. **결제 연동 요청을 받으면 generate_payment_code보다 먼저 호출하세요.** 무엇을 판정하는가: - 클라이언트: web(React/Next/Nuxt/Vue/Svelte/Angular) / an…`
- `get_cs_guide`: `Bootpay 고객응대 매뉴얼을 조회합니다. 섹션을 지정하면 해당 부분만 반환합니다.`
- `get_csp_allowlist`: `결제창이 CSP(Content-Security-Policy)에 막힐 때 헤더에 넣어야 할 PG 도메인 허용목록과 프레임워크별 설정 스니펫을 생성합니다. "Refused to frame" / "violates the following Content S…`
- `get_doc`: `⚠️ 결제 코드가 필요하면 이 도구 대신 generate_payment_code를 호출하세요. 이 도구는 문서 상세 조회 전용입니다. get_doc으로는 결제 연동 코드를 생성할 수 없습니다.`
- `get_sdk_versions`: `모든 Bootpay SDK의 최신 버전을 반환합니다. 코드를 작성하기 전에 반드시 이 도구를 호출하여 정확한 버전을 확인하세요. 학습 데이터의 버전(3.x, 4.x 등)은 더 이상 동작하지 않습니다.`
- `get_setup_checklist`: `⚠️ 결제 연동 시에는 이 도구보다 get_integration_context를 먼저 호출하세요. Admin 도구가 있으면 실제 프로젝트 설정을 자동으로 확인합니다. 이 도구는 수동 설정 체크리스트용입니다.`
- `get_troubleshooting`: `결제 연동에서 자주 막히는 문제 하나(topic)의 원인 · 확인 순서 · 해결 방법을 정리한 안내서를 돌려줍니다. 「결제창이 안 뜬다」·「웹훅이 안 온다」·「심사가 안 끝난다」처럼 증상이 있을 때 topic 을 골라 부르고, 결과의 확인 순서대로…`
- `list_docs`: `전체 문서 목록 또는 특정 카테고리의 문서 목록을 반환합니다.`
- `search_docs`: `부트페이 개발자 문서(결제 · 정기결제 · 구독 · 커머스 API · 알림톡 · 웹훅 등)를 한국어 키워드로 검색해 제목 · 경로 · 한 줄 요약을 돌려줍니다. 고른 문서의 본문은 get_doc(path) 로 읽습니다. 결과가 없으면 키워드를 바꾸거…`

## Changes

- 2026-11-26: [description changed](../../deltas/2026-11-26/a46719d28a156bbc76f4.json): `2 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.bootpay.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
