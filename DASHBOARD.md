# 100X Dashboard

The dashboard is a navigation and decision layer, not a second source of investment data.

## Artha view

Artha should consume `data/universe.json` and dynamically create four tabs by filtering the single `status` field:

- **CORE**
- **WATCH**
- **FRONTIER**
- **REJECTED**

Each table row should link to the corresponding company research Markdown file using the `research_file` field in the company record.

## Data ownership

- `data/universe.json` — canonical current structured data.
- `companies/india/` — detailed India company research.
- `companies/usa/` — detailed USA company research.
- `research/` — dated research events and changes.
- Git history — complete historical record of changes.

There should be no manually maintained CORE/WATCH/FRONTIER/REJECTED company lists in the repository.

## Identity

The canonical security `id` is the **ISIN**. Ticker is a display/trading identifier. Exchange is not part of the core identity model. Initial geography scope: **India and USA**.
