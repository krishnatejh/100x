# 100X Technical Reference

This document retains the internal implementation and data-governance information that was previously included in the main README. The main README is intentionally focused on the public-facing investment research philosophy and methodology.

## Identity

Each listed security uses its **ISIN as the canonical `id`**. Ticker is retained as the trading/display symbol. Exchange is intentionally excluded from the core research identity.

The current geography scope includes **India and USA**.

## Data Contract

The machine-readable structure is defined by:

- `data/universe.schema.json` — machine-readable validation schema.
- `data/schema.md` — human-readable field definitions and controlled taxonomies.
- `data/universe.json` — canonical current structured dataset.

New company records must conform to the schema and use:

- A unique ISIN.
- Allowed `status` values.
- Allowed `thesis_health`, `position_action` and `fresh_capital_action` values.
- A consistent `research_path`.

## Canonical Data and Views

`data/universe.json` is the canonical structured current state.

CORE, WATCH, FRONTIER and REJECTED are classifications represented within the canonical universe. Separate duplicate company lists should not be maintained.

Detailed company research lives in the corresponding Markdown research file. Structured current-state data should not be duplicated across multiple files unnecessarily.

## Beyond the 100X Framework — Data Rules

The `beyond_100x` boolean is maintained in the canonical company record.

It is a **discovery flag**, not a second status, score, portfolio or recommendation.

- `CORE` companies must have `beyond_100x: false`.
- `WATCH`, `FRONTIER` and `REJECTED` companies may have `beyond_100x: true` only when a specific alternative investment case has been explicitly researched and documented.
- Failing the strict 100X test does not automatically qualify a company for Beyond 100X.
- Beyond 100X is a filtered view of the canonical universe; no second universe or duplicate company record should exist.

## Repository Structure

- `README.md` — public-facing project overview, investment philosophy and methodology.
- `DASHBOARD.md` — dashboard architecture and navigation overview.
- `TECHNICAL_REFERENCE.md` — internal implementation and data-governance reference.
- `data/universe.json` — canonical structured universe.
- `data/universe.schema.json` — machine-readable validation schema.
- `data/schema.md` — human-readable data definitions and controlled taxonomies.
- `companies/COMPANY_TEMPLATE.md` — standard company research template.
- `companies/india/` — India company research pages.
- `companies/usa/` — USA company research pages.
- `sectors/SECTOR_COVERAGE.md` — sector coverage and discovery-bias control.
- `research/` — dated research notes and changes.
- `research/RESEARCH_LOG.md` — material research decisions and thesis changes.

## Decision-Grade Evidence (DGE)

Detailed company research should preserve durable provenance for **decision-driving evidence** without attempting to cite every routine statement.

DGE belongs in the relevant company research Markdown so that evidence remains close to the reasoning it supports. A typical DGE item records:

- DGE ID/title.
- Claim.
- Why it matters to the decision.
- Specific source.
- Date/reporting period.
- Page, section, timestamp or equivalent location where practical.
- Type: FACT, MANAGEMENT CLAIM, INFERENCE or SPECULATION.
- Supporting basis for an inference.

Chat-local citation tokens or generic source categories are not sufficient durable provenance for material conclusions. Prefer stable document names and links where available.

DGE is a research-governance convention, not a new canonical JSON database. One company remains one canonical universe record with one corresponding research document.

## Validation

Before consuming or committing universe data, validate `data/universe.json` against `data/universe.schema.json`.

At minimum, validation should catch:

- Malformed JSON.
- Duplicate ISINs.
- Invalid status, thesis-health or action values.
- Invalid scores.
- Invalid dates.
- Missing required fields.
- Broken `research_path` references.

## Access

Research, valuation work, investment theses and decision history are treated as project research material.

Authorized GitHub access may be used for collaboration and automation.

## Classification Taxonomy

The canonical universe uses three separate dimensions:

- **Sector** — one GICS-aligned broad sector.
- **Industry** — one controlled primary business classification.
- **Themes** — zero to five controlled cross-cutting opportunity areas.

The authoritative enums and rules are documented in `data/schema.md` and enforced by `data/universe.schema.json`.

## Maintenance Principle

The public-facing README should remain concise and focused on the investment research framework.

Implementation details, repository conventions, data structures and validation rules belong in technical documentation such as this file.
