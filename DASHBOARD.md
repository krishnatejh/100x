# 100X Dashboard

The dashboard is a navigation and decision layer, not a second source of investment data.

## Artha view

Artha should consume `data/universe.json` and dynamically create four tabs by filtering the single `status` field:

- **CORE**
- **WATCH**
- **FRONTIER**
- **REJECTED**

Each table row should link to the corresponding company research Markdown file using the `research_path` field in the company record.

For CORE companies, the UI should display the separate `action` dimension (for example WAIT, ACCUMULATE or HOLD). Status and action are intentionally independent.

## Data ownership

- `data/universe.json` — canonical current structured data.
- `data/universe.schema.json` — machine-readable contract.
- `data/schema.md` — human-readable definitions and controlled taxonomies.
- `companies/india/` — detailed India company research.
- `companies/usa/` — detailed USA company research.
- `sectors/SECTOR_COVERAGE.md` — sector coverage and discovery-bias control.
- `research/` — dated research events and changes.
- Git history — complete historical record of changes.

There should be no manually maintained CORE/WATCH/FRONTIER/REJECTED company lists in the repository.

## Identity

The canonical security `id` is the **ISIN**. Ticker is a display/trading identifier. Exchange is not part of the core identity model. Initial geography scope: **India and USA**.

## Validation

`data/universe.json` should be validated against `data/universe.schema.json` before it is consumed by Artha or used for migration/update operations. Validation should also check that each non-null `research_path` exists in the repository and that ISINs are unique.
