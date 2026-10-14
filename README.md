# Personal Curriculum Builder

A year-long learning planner in **one self-contained HTML file**. It is a builder, not a course: you start with empty structure and grow your own curriculum over the year, one quarter at a time.

**Live demo:** https://handoffta.github.io/personal-curriculum-builder/

## What it does

- **Interests** — add, rename, recolor, and delete the areas you want to learn. Gardening and Writing come pre-loaded as placeholders so you can see the shape.
- **Four quarters** — editable tab labels, so you can call them "Winter" or "Jan–Mar." Focus items are grouped by interest within each quarter.
- **Focus items** — each has a title, a note on why it matters to you, a status (Not started / In progress / Done), and an optional link or reference. Edit inline, and move an item to a different quarter any time.
- **Year at a glance** — all four quarters side by side, color-coded by interest, with a completion count per quarter and per interest.
- **Up next** — the next few open items in the current quarter, so opening the tool tells you what to pick up today.
- **Progress stats** — total items, overall percent complete, and percent per interest, updating live.
- **Print view** — a clean single-page summary of the full year for offline reference.

The starter entries are clearly badged "example — replace or delete." No real curriculum is included on purpose; you fill it in.

## How data is stored

Everything saves to your own browser (localStorage). Nothing is sent anywhere, and there is no account. Closing and reopening the page keeps your plan. Clearing your browser data clears it, and a different browser or device starts a fresh notebook.

## Tech notes

- Single HTML file: vanilla JavaScript, no frameworks, no build step, no external dependencies, no network calls, system font stacks only. It works fully offline.
- Responsive down to phone widths, with a print stylesheet.
- Tested with an automated jsdom suite (62 checks) covering add/edit/delete for interests and items, status changes feeding the stats and the up-next panel, and persistence across simulated reloads, including a blocked-storage fallback.

---

Part of the [HandOffTA](https://github.com/HandOffTA) build portfolio. Built with Claude (Anthropic).
