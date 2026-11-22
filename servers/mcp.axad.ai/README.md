# mcp.axad.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.axad.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.axad.ai/mcp` | 23 | [`524556096013`](7edd553d503f1bb71bb8.json) | 2026-11-22 |

## Tools at `https://mcp.axad.ai/mcp`

- `browse_catalog`: `Browse Axad's library of lessons and practice exams. With no lang, returns the languages Axad teaches. With lang, returns the sections and…`
- `close_lesson`: `Close a lesson the learner finished or set aside. Its place, chats and cards are kept, and it no longer counts against the plan's active le…`
- `due_cards`: `List the learner's flash cards that are due for review now, the most overdue first, each with an example sentence. lang limits it to one la…`
- `find_images`: `Search the shared image library for pictures that show a word, chunk, action or scene. query is a literal English description of the pictur…`
- `get_account`: `Return the learner's Axad account: their plan, its limits and what they use of them (cards in the bag, active lessons), and their credit sp…`
- `list_lessons`: `List the learner's lessons, the active ones first, then the closed ones, each with its language, page and progress. For a learner who wants…`
- `list_runbooks`: `List Axad's learning paths (daily review, exam path, page by page, free-form chat), with the learner's place in each when signed in.`
- `next_step`: `Read the learner's current step in a learning path they started, without moving it. Returns the step: what it asks, which tools and widgets…`
- `nominate_image`: `Ask for a picture of a generic concept every learner shares: a concrete thing, action, place or everyday scene. Returns an existing library…`
- `open_lesson`: `Open a lesson and read where the learner is in it: a lesson of Axad's library (lesson), one the learner already has (material), or a new le…`
- `read_page`: `Read one page of a lesson that has pages (a practice exam: one question and its text a page) and keep the learner's place there; for a less…`
- `record_step`: `Record how the current step of a learning path went (done, skipped or struggled) with an optional note, and move the learner on. Returns th…`
- `redeem_gift`: `Redeem a gift code the learner was given: what it gives is added to their account at once (credit, more cards in the bag, more open practic…`
- `review_card`: `Record how well the learner recalled a card: 1 forgot, 2 hard, 3 good, 4 easy. Schedules the card's next review (FSRS) and returns its due…`
- `save_cards`: `Save flash cards to the learner's bag: words, phrases, idioms, sentences or patterns they engaged with, at or just above their level. Takes…`
- `search_bag`: `Search the learner's flash cards by words in the card's language or by a short meaning. Returns the matching cards, up to limit (default 10…`
- `show_cards`: `Shows Axad's answer as one stack of cards, as the Axad app does: use it for every reply that teaches a language the learner learns, instead…`
- `show_drill`: `Displays a short practice round for the learner to answer by tapping, one question at a time: choice, cloze, order or translate. It shows t…`
- `show_home`: `Displays Axad's start menu as a list of taps: go on with the open lesson, start a lesson, paste a sentence, inburgering practice, review ca…`
- `show_review`: `Displays the learner's due flash cards one at a time: the front, the answer and example on a tap, then four taps to grade the recall, which…`
- `speak`: `Make a natural voice recording of a sentence in the language the learner learns. Returns a link to the audio and the start and end time of…`
- `start_runbook`: `Start a learning path for the learner in a language, or return their place in it if they started it before. Returns the current step: what…`
- `upgrade_link`: `Return a link on axad.ai where the learner can pick a plan, add a card for more free use, or buy credit; want says which. Returns the url a…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.axad.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
