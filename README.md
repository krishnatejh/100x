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

## Identity

Each listed security uses its **ISIN as the canonical `id`**. Ticker is retained as the trading/display symbol. Exchange is intentionally excluded from the core research identity. The initial geography scope is **India and USA**.

## Data contract

The machine-readable structure is defined by `data/universe.schema.json`, with human-readable field definitions and taxonomies in `data/schema.md`. `data/universe.json` is the canonical current dataset. New company records must conform to the schema, use a unique ISIN, use an allowed `status` and `action`, and use `research_path` consistently.

## Repository structure

- `DASHBOARD.md` — architecture and navigation overview.
- `data/universe.json` — canonical structured universe used by Artha and other views.
- `data/universe.schema.json` — machine-readable validation schema.
- `data/schema.md` — human-readable data definitions and controlled taxonomies.
- `companies/COMPANY_TEMPLATE.md` — standard research template.
- `companies/india/` — India company research pages.
- `companies/usa/` — USA company research pages.
- `sectors/SECTOR_COVERAGE.md` — sector coverage and discovery-bias control.
- `research/` — dated research notes and changes.
- `research/RESEARCH_LOG.md` — material research decisions and thesis changes.

Detailed company research lives in the corresponding Markdown file. Structured current-state data lives in `universe.json`; the same data should not be duplicated in separate CORE/WATCH/FRONTIER/REJECTED files.

## Artha integration

Artha's 100X section should consume `data/universe.json` and dynamically filter records by `status` into four tabs: CORE, WATCH, FRONTIER and REJECTED. Each company record contains a `research_path` pointing to its detailed research Markdown file. Artha should not maintain a second copy of the investment universe.

## Validation

Before consuming or committing universe data, validate `data/universe.json` against `data/universe.schema.json`. At minimum, validation must catch malformed JSON, duplicate ISINs, invalid status/action values, invalid scores, invalid dates and missing required fields. Broken `research_path` references should also be flagged.

## Access

This repository is intentionally **private**. Research, valuation work, investment theses, and decision history are treated as private investment-research material. Authorized GitHub access is used for collaboration and automation; public visibility is not required for the 100X workflow.
