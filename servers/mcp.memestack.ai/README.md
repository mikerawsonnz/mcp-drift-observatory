# mcp.memestack.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.memestack.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.memestack.ai/mcp` | 20 | [`9cf78df04441`](6495c3b7c78c1957343a.json) | 2026-08-20 |

## Tools at `https://mcp.memestack.ai/mcp`

- `browse_by_category`: `Get a category and its featured images. Categories group related tags (e.g. "charts", "memes", "lightning-network").`
- `browse_by_tag`: `Browse images for a specific tag. Returns the tag profile (description, stats) and optionally a paginated list of images tagged with it.`
- `browse_images`: `Browse and filter the image gallery without a search query. Useful for discovering content by tag, trending, or recent uploads.`
- `cite_image`: `Generate canonical attribution blocks for one or more MemeStack images. Returns markdown, HTML, and plain-text citation strings ready to pa…`
- `find_meme_for_text`: `Find a meme that captures a vibe, idea, or concept. Returns ready-to-embed images with citation blocks. Use this when writing posts, articl…`
- `find_related`: `Find semantically related images using AI embedding similarity. Returns images with similar meaning/topic.`
- `find_similar`: `Find visually similar images using perceptual hash matching. Returns images that look alike.`
- `generate_meme`: `Generate a new image from a text prompt using AI (Grok Imagine). Paid tool — billed per call via the agent payment rails (x402/L402); not c…`
- `get_image`: `Get full metadata for a specific image by ID, including caption, alt text, tags, OCR text, zap stats, and URLs.`
- `get_leaderboard`: `Get top-ranked images by zaps received, or top zappers by amount zapped, over a time period.`
- `get_mutation_group`: `Get all variants of a meme template tracked on MemeStack. Returns the dominant image plus every variant in the same mutation group, with ci…`
- `get_tag_profile`: `Get the profile for a tag (description, image count, total zaps, related tags) without fetching any images. Use browse_by_tag to also retri…`
- `get_user_profile`: `Get a user's public profile including display name, stats, and avatar info.`
- `list_categories`: `List all available image categories. Use this to discover what categories exist before calling browse_by_category.`
- `popular_tags`: `List the most-used tags on MemeStack by all-time usage count. (Time-period filtering is not yet supported — tag usage is currently counted…`
- `reverse_image_search`: `Find MemeStack images that look visually similar to a given image. Accepts an HTTPS image URL or a 'data:image/...;base64,...' URL for byte…`
- `search_images`: `Search the MemeStack image gallery. Runs semantic AI and keyword matching in parallel and merges results. Returns images with captions, tag…`
- `search_text_in_image`: `Search for images by the text written or printed in them (OCR). Different from regular search — only matches the text_in_image field, not c…`
- `submit_image`: `Submit an image to the MemeStack review queue. Paid tool — 100 sats (or USDC equivalent) per submission via the agent payment rails (x402/L…`
- `tag_autocomplete`: `Suggest tag slugs matching a prefix. Use this to verify a tag exists before filtering by it, or to discover related tags. Prefix must be ≥…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.memestack.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
