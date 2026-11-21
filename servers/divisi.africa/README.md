# divisi.africa: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/divisi.africa.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://divisi.africa/mcp` | 47 | [`de9490174eca`](e5e7fb4da22c649c0642.json) | 2026-11-21 |

## Tools at `https://divisi.africa/mcp`

- `add_task`: `Add a task to a farm, due on 'due_date' (within a year back or two years ahead), optionally for one crop or batch ('unit', a name or id). I…`
- `add_unit`: `Add something the person grows or keeps, the way the app does, and Divisi schedules its tasks. 'what' is in their words: a crop ("maize"),…`
- `add_zone`: `Add a field, pen, pond or apiary to a farm. A name already used gets a number added. Only farm owners and managers can add one. Pass the sa…`
- `apply_to_programme`: `Ask to join a programme as the person. This puts the organisation's request on their list; nothing is shared until they read it and say yes…`
- `ask_agronomist`: `Ask Divisi's agronomists, experts and other farmers by posting the question in Community as the person. It is public and free; answers come…`
- `book_consultation`: `Ask a verified expert for a call ('virtual') or a farm visit ('in_person', to one of the person's farms) at the time proposed, at the exper…`
- `cancel_consultation`: `Call off a consultation before it starts, either side. A paid booking is refunded to the farmer in full.`
- `cancel_rsvp`: `Give up the person's place at an event, so the next person waiting gets it.`
- `consultation_step`: `Take the next step on a consultation, as the person: 'propose' another time (with 'starts_at'), 'accept' or 'decline' the time the other si…`
- `create_listing`: `Put something on the Market as the person, from what they said in one sentence ("40 broilers ready on the 12th, Harare"): produce for sale…`
- `express_interest`: `Tell Divisi the person needs a service where they farm, so they are told when it arrives there. 'need': inputs (seed and fertiliser), finan…`
- `farm_money`: `Money in, money out and what is left, worked out: per crop or batch, for costs of the whole farm, and in total, with the totals by heading…`
- `farm_report`: `How the person's farms are doing and what needs them. Per farm: the weather now, the days ahead and any warning; every crop, flock, herd, p…`
- `find_crops`: `Crops that suit a place, best first, with when to plant each. Give a town or district name ("Murewa", "Nakuru") or a lat/lng. The list is i…`
- `find_events`: `Upcoming field days, trainings and meetups, soonest first: near a town, district or lat/lng (within 'radius_km', at most 200), or online. '…`
- `find_experts`: `Verified agronomists, vets and advisers on Divisi, best first: who they are, what they know, where they are, whether they visit farms near…`
- `find_market`: `Where a market is and when it runs. Give a market's 'name' ("Mbare Musika", "Mile 12", "Wakulima"; spelling and the word market do not matt…`
- `find_programmes`: `Outgrower schemes and other farmer programmes taking farmers this season where the person farms (their farm by default, or a town, district…`
- `identify_problem`: `Which pests or diseases might explain what a farmer sees on a crop: candidates from that crop's Divisi guide, best match first, each with h…`
- `inbox`: `The person's message conversations, newest first, each with who it is with, how many messages are unread and the last message. 'search' mat…`
- `log_work`: `Write work done, money in or out, or both, into the farm records, in the person's words. 'unit' names the crop or batch it was for (its nam…`
- `make_offer`: `Offer to buy from (or sell to) a listing as the person: 'quantity' of its unit at 'price_per_unit' in major units. A buyer chooses how to p…`
- `manage_listing`: `Keep one of the person's listings up to date: 'renew' keeps it on the Market (with 'quantity_available', how many are left now), 'sold' tak…`
- `market_prices`: `The typical price range Divisi has seen for a product near a place, per 'unit' ("kg", "50 kg bag", "crate"), from listings, deals and publi…`
- `move_tasks`: `Move a crop's or batch's tasks that are not done so the first of them falls on 'start_on', keeping the gaps between them: when planting sli…`
- `my_consultations`: `The person's consultations, booked or booked with them, newest first, each with its next step. 'open_only' false includes finished ones.`
- `my_deals`: `The person's Market deals that are still going, as buyer and seller, most recently changed first ('include_finished' adds closed ones): wha…`
- `my_money`: `The person's money in Divisi: what is theirs to spend or withdraw, what is coming from sales (held until each buyer has the goods, with the…`
- `my_requests`: `The services the person has asked Divisi for and still wants, newest first: waiting, reminders set, and what has reached their area (with w…`
- `pay_deal`: `What paying for one of the person's deals through Divisi takes, and the page in Divisi where they pay it themselves: how much comes from th…`
- `plan_season`: `Write the person's own season plan for one crop or batch ('unit', a name or id): the jobs they want and when. Divisi turns each into a task…`
- `read_guide`: `The summary of Divisi's guide to one crop, pest or disease, named in any language: for a crop, its overview, key facts, season stages and t…`
- `read_thread`: `The messages in one of the person's conversations, newest first, 30 a page. Only conversations they are in can be read.`
- `record_sale`: `Write down a sale from one of the person's listings that happened outside Divisi (at the gate, on WhatsApp): 'quantity' of the listing's un…`
- `reply_to_review`: `Answer a rating someone gave the person, once, in their own words. It shows under the rating.`
- `respond_to_offer`: `Answer an offer the person received: 'accept' (makes a deal), 'decline', or 'counter' with another 'price_per_unit' (and 'quantity', the sa…`
- `review_deal`: `Rate the other person on a finished deal, 1 to 5 'stars', with a short 'comment' if they want one. Others see it when they decide whether t…`
- `rsvp`: `Take a place at an event as the person. A full event puts them on its waiting list. Retrying is safe: one place each.`
- `search_market`: `Find Market listings: produce and inputs for sale ('kind' SALE) or what people want to buy (WANTED), near a town, district or lat/lng (with…`
- `sell_harvest`: `Put a crop or a batch of animals from the person's farm up for sale, as it nears harvest or slaughter. Divisi fills in what it knows: what…`
- `send_message`: `Send a text message as the person: into a conversation they are in ('conversation_id'), or to a person ('to_person_id'), which opens or reu…`
- `set_up_farm`: `Add a farm the person owns. Say where with 'lat'/'lng' (best: advice is then for that spot) or a town or district as 'place' (its centre is…`
- `update_deal`: `Move one of the person's deals on. A seller: 'handed_over' with the 4-digit 'code' the buyer shows them (ask the seller for it; never guess…`
- `update_farm`: `Rename a farm, change its description, or move it ('lat'/'lng', or a 'place'). Only what is passed changes. Only farm owners and managers c…`
- `update_task`: `Look after a task: mark it done ('done', with an optional 'note' of what was done and the 'day', today if left out), move it to another 'du…`
- `when_to_plant`: `When to plant one crop at one place: the planting window open now or next, the other seasons in the year, when harvest falls, and the servi…`
- `withdraw_interest`: `Take a service request off the person's list: they no longer need it and will not be told when it arrives.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://divisi.africa/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
