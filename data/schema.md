# 100X Universe Data Schema

`data/universe.json` is the canonical structured dataset for the 100X universe.

## Required company fields

| Field | Type | Allowed values | Purpose |
|---|---|---|---|
| `id` | string | Valid ISIN | Canonical security identity; must be unique |
| `name` | string | Company/security name | Display name |
| `ticker` | string | Trading symbol | Display/trading identifier |
| `country` | string | Initially `India` or `USA` | Issuer geography |
| `currency` | string | ISO 4217 code | Reporting/trading currency |
| `sector` | string | Controlled sector taxonomy | Sector coverage and bias analysis |
| `status` | string | `CORE`, `WATCH`, `FRONTIER`, `REJECTED` | Research classification |
| `thesis_health` | string | See taxonomy below | Evolution of long-term thesis |
| `position_action` | string | `HOLD`, `REDUCE`, `EXIT` | Action for an existing position |
| `fresh_capital_action` | string | `DEPLOY`, `WAIT` | Whether new capital should be allocated now |
| `research_path` | string/null | Repository path or null | Link to detailed research |
| `last_reviewed` | string | `YYYY-MM-DD` | Freshness of structured assessment |
| `scores` | object | Four numeric scores, 0–10 | 100X framework scoring |

## Status taxonomy
- **CORE** — high-conviction candidate with a credible long-term path to exceptional returns.
- **WATCH** — interesting opportunity requiring more evidence, better valuation, or execution proof.
- **FRONTIER** — very high potential but highly uncertain.
- **REJECTED** — investigated and excluded; reason retained.

Status is a research classification, not a buy/sell signal.

## Thesis-health taxonomy
- **STRENGTHENING** — new evidence increases confidence.
- **INTACT** — long-term thesis remains valid.
- **UNDER_REVIEW** — important questions require investigation; no conclusion yet.
- **WEAKENING** — evidence is materially reducing confidence.
- **BROKEN** — core assumptions are no longer valid.

Valuation alone should generally affect `fresh_capital_action`, not `thesis_health`.

## Position-action taxonomy
For an investor who already owns the stock:
- **HOLD** — continue owning.
- **REDUCE** — reduce exposure.
- **EXIT** — sell/close the position.

`EXIT` requires explicit documented reasoning and should not be implied merely by a high valuation.

## Fresh-capital-action taxonomy
For new money available today:
- **DEPLOY** — allocate fresh capital to the company.
- **WAIT** — do not allocate fresh capital now.

`WAIT` is not a sell signal. A company can be `HOLD` for an existing position and `WAIT` for fresh capital.

## Scores
- `business_potential`
- `probability_of_success`
- `investment_attractiveness`
- `overall_100x`

All scores use a 0–10 scale.

## Identity and research rules
- ISIN is the canonical `id`.
- Ticker is retained for display/trading purposes.
- Structured current-state fields belong in `universe.json`.
- Detailed evidence and rationale belong in the linked company research file.
