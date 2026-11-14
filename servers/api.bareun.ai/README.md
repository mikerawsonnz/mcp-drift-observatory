# api.bareun.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.bareun.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.bareun.ai/mcp` | 6 | [`0302a8c599b8`](433537aec8fde738c83b.json) | 2026-11-14 |

## Tools at `https://api.bareun.ai/mcp`

- `analyze_syntax`: `한국어 문장의 형태소 분석을 수행합니다. 문장을 어절·형태소로 나누고 품사를 부착합니다. format=compact 면 '표층형/품사' 요약 문자열을, full 이면 전체 구조 JSON 을 돌려줍니다. with_sense=true 를 주면 동형이의어…`
- `analyze_syntax_raw`: `후처리 없는 순수 형태소 분석을 수행합니다. 분절·품사 태깅 모델의 추론 결과를 그대로 반환하며 복합명사·복합동사 분해, 자동 띄어쓰기·붙여쓰기, 사용자 사전을 적용하지 않습니다. 모델 성능 평가나 말뭉치 재태깅처럼 후처리가 섞이지 않은 출력이 필요…`
- `correct_grammar`: `한국어 문장의 맞춤법·띄어쓰기를 교정합니다. 교정된 문장과 교정 블록(원문/교정문) 목록을 돌려줍니다. 원문을 다시 쓰지 않고 어긋난 자리만 고치므로 글의 문체·말투가 그대로 남습니다. 고친 자리마다 근거가 되는 한글맞춤법 조항(예: 제1장 총칙 제…`
- `list_pos_tags`: `바른 형태소 분석이 사용하는 47개 품사 태그 목록(코드·이름·대분류·소분류·enum)을 JSON 으로 돌려줍니다. analyze_syntax 결과의 품사 코드(NNG, JKS 등)를 해석할 때 참고하세요. EN: Returns the list of…`
- `search_dict`: `우리말샘 사전을 자소(음소) 단위 슬롯 패턴으로 검색합니다. 완성형으로 표현할 수 없는 조건 — 초성·중성·종성 각각에 대한 조건('받침이 ㅎ인 용언', '중성이 ㅚ이고 받침 없는 1음절 어간') — 을 걸 수 있고, anchor=suffix 로 '…`
- `tokenize`: `한국어 문장을 어절(토큰) 단위로 분리합니다. 품사 정보 없이 어절 경계만 필요할 때 쓰고, 형태소·품사가 필요하면 analyze_syntax 를 쓰세요. auto_spacing=true 를 주면 띄어쓰기가 어긋난 문장도 바로잡아 나눕니다. EN:…`

## Changes

- 2026-11-14: [annotation changed, description changed, schema changed](../../deltas/2026-11-14/433537aec8fde738c83b.json): `51 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-11-01: [schema changed](../../deltas/2026-11-01/433537aec8fde738c83b.json): `7 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.bareun.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
