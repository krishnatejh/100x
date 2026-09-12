# 100X Investment Research

A long-term, sector-neutral research system for identifying listed companies with plausible asymmetric 50X–100X+ shareholder-return potential over 10–25+ years.

## Philosophy

We do not predict 100X winners. We ask what would have to be true for exceptional outcomes to occur, test those assumptions, assess probability, and compare today's valuation with the required future economics.

## Universe

- **CORE** — high-conviction candidate with a credible path to exceptional returns.
- **WATCH** — interesting opportunity requiring better evidence, valuation, or execution proof.
- **FRONTIER** — very high potential but highly uncertain emerging technology/business.
- **REJECTED** — investigated and excluded; reason retained for future reference.

Status is stored once in `data/universe.json`. CORE/WATCH/FRONTIER/REJECTED are application views and are not maintained as separate company lists.

## Beyond the 100X Framework

The project remains strictly focused on identifying plausible 50X–100X+ outcomes. During that research, a company may occasionally reveal a compelling investment case that deserves separate discovery even though its strict 100X path is insufficient or uncertain.

This is represented by the boolean `beyond_100x` flag in the same canonical company record. It is a **discovery flag**, not a second status, score, portfolio, or recommendation. The Beyond 100X experience is a filtered view of `data/universe.json`; no second universe or duplicate company record exists.

- `CORE` companies must have `beyond_100x: false` because they are already surfaced by the primary framework.
- `WATCH`, `FRONTIER`, and `REJECTED` companies may have `beyond_100x: true` only when a specific alternative investment case has been explicitly researched and documented.
- Failing the 100X test does not automatically qualify a company for Beyond 100X.

## Identity

Each listed security uses its **ISIN as the canonical `id`**. Ticker is retained as the trading/display symbol. Exchange is intentionally excluded from the core research identity. The initial geography scope is **India and USA**.

## Data contract

The machine-readable structure is defined by `data/universe.schema.json`, with human-readable field definitions and taxonomies in `data/schema.md`. `data/universe.json` is the canonical current dataset. New company records must conform to the schema, use a unique ISIN, use allowed `status`, `thesis_health`, `position_action` and `fresh_capital_action`, and use `research_path` consistently.

## Repository structure

- `DASHBOARD.md` — architecture and navigation overview.
- `data/universe.json` — canonical structured universe used by the project and its views.
- `data/universe.schema.json` — machine-readable validation schema.
- `data/schema.md` — human-readable data definitions and controlled taxonomies.
- `companies/COMPANY_TEMPLATE.md` — standard research template.
- `companies/india/` — India company research pages.
- `companies/usa/` — USA company research pages.
- `sectors/SECTOR_COVERAGE.md` — sector coverage and discovery-bias control.
- `research/` — dated research notes and changes.
- `research/RESEARCH_LOG.md` — material research decisions and thesis changes.

Detailed company research lives in the corresponding Markdown file. Structured current-state data lives in `universe.json`; the same data should not be duplicated in separate CORE/WATCH/FRONTIER/REJECTED files.


## Validation

Before consuming or committing universe data, validate `data/universe.json` against `data/universe.schema.json`. At minimum, validation must catch malformed JSON, duplicate ISINs, invalid status/thesis/action values, invalid scores, invalid dates and missing required fields. Broken `research_path` references should also be flagged.

## Access

This repository is intentionally **private**. Research, valuation work, investment theses, and decision history are treated as private investment-research material. Authorized GitHub access is used for collaboration and automation; public visibility is not required for the 100X workflow.


## Classification taxonomy

The canonical universe uses three separate dimensions: `sector` (one GICS-aligned broad sector), `industry` (one controlled primary business classification), and `themes` (zero to five controlled cross-cutting opportunity areas). The authoritative enums and rules are documented in `data/schema.md` and enforced by `data/universe.schema.json`.
