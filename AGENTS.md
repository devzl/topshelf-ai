# Instructions for LLMs contributing to this repo

This file governs how any AI agent (Claude, GPT, etc.) should add or edit entries in `README.md`.

## Before adding a tool

1. Verify the repo actually exists and the URL is correct (fetch the page, don't guess).
2. Confirm it's a real, relevant, open source AI tool or adjacent tooling, not a random or low-quality repo.
3. Determine which existing category it belongs to. Only create a new category if it genuinely doesn't fit any existing one.

## Entry format

Every entry is a card, not a bullet:

```
### [owner/repo](https://github.com/owner/repo) ![GitHub stars](https://img.shields.io/github/stars/owner/repo?style=flat-square&label=%E2%98%85)
One-line description written in your own words, not copy-pasted from the repo.
```

- The name is a heading (`###`), linked to the GitHub repo.
- A shields.io star badge sits on the same line as the name. Never hardcode a star count.
- The description goes on the line below the heading, one line only.
- Do not use bullet-list entries for tools.

## Categories

- Each category is an `##` heading.
- Every category must be listed in the `## Categories` table of contents near the top of `README.md`, linking to its anchor.
- Keep category names short and specific (e.g. "Agent Skills & Frameworks", not "AI Stuff").

## Workflow

1. Fetch the repo URL and confirm description/purpose before writing anything.
2. Edit `README.md`: add to an existing category, or create a new one (heading + ToC entry) if needed.
3. Commit using [Conventional Commits](https://www.conventionalcommits.org/): `feat: add <owner/repo> to <category>` for new tools, `docs: ...` for structural/formatting changes.
4. Push to `main` unless told otherwise.

## What not to do

- Don't add tools without being asked to.
- Don't hardcode star counts.
- Don't invent categories speculatively, only add one when a tool needs it.
- Don't use em dashes in any content you write to this repo.
