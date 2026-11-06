# hotker.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/hotker.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://hotker.ai/mcp` | 6 | [`c0e4a7927f3b`](843aca1f3ccaa84caf86.json) | 2026-08-30 |

## Tools at `https://hotker.ai/mcp`

- `calculate_combo_discount`: `통신사, 인터넷 등급과 모바일 회선 조건으로 24개월 결합할인 참고값을 계산합니다.`
- `calculate_contract_penalty`: `SKT·KT·LG U+ 선택약정 할인반환금 또는 공시지원금 반환액의 기본 참고값을 계산합니다.`
- `calculate_mobile_tco`: `사용자가 제공한 단말가, 요금제 유지기간, 부가서비스와 확정 할인으로 12~36개월 총비용을 계산합니다. 누락·추정 조건을 명시하며 실시간 판매가를 만들지 않습니다.`
- `get_calculation_evidence`: `HOTKER TCO, 약정 반환금과 결합할인 계산식의 엔진 버전, 공식 통신사 출처와 한계를 반환합니다.`
- `search_verified_mobile_deals`: `공식·통신사 확인 상태이고 유효기간이 남아 있으며 추정이나 누락이 없는 24개월 TCO 휴대폰 조건만 검색합니다.`
- `search_verified_products`: `HOTKER production 카탈로그에서 SEO INDEX 판정을 통과한 최신 상품만 검색합니다. NOINDEX·REVIEW·수집중 상품은 반환하지 않습니다.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://hotker.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
