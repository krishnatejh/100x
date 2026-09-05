# 100X Universe Data Schema

`data/universe.json` is the canonical structured dataset for the 100X universe.

## Required company fields

| Field | Type | Allowed / expected values | Purpose |
|---|---|---|---|
| `id` | string | Valid ISIN | Canonical security identity; must be unique |
| `name` | string | Company/security name | Display name |
| `ticker` | string | Trading symbol | Display/trading identifier |
| `country` | string | Initially `India` or `USA` | Issuer geography |
| `currency` | string | ISO 4217 code, e.g. `INR`, `USD` | Reporting/trading currency |
| `sector` | string | Controlled sector taxonomy | Sector coverage and bias analysis |
| `status` | string | `CORE`, `WATCH`, `FRONTIER`, `REJECTED` | Current universe classification |
| `action` | string | Controlled action taxonomy | Allocation/action dimension |
| `research_path` | string/null | Repository path or null | Link to detailed research |
| `last_reviewed` | string | `YYYY-MM-DD` | Freshness of structured assessment |
| `scores` | object | Four numeric scores, 0–10 | 100X framework scoring |

## Score fields

- `business_potential`
- `probability_of_success`
- `investment_attractiveness`
- `overall_100x`

All scores use a 0–10 scale. `overall_100x` is a judgement summary and must not hide the three component scores.

## Status taxonomy

- **CORE** — high-conviction candidate with a credible long-term path to exceptional returns.
- **WATCH** — interesting opportunity requiring better evidence, valuation, or execution proof.
- **FRONTIER** — very high potential but highly uncertain emerging technology/business.
- **REJECTED** — investigated and excluded; retain the reason in the company's research file.

## Action taxonomy

- **ACCUMULATE** — valuation/fundamentals support adding now in a disciplined manner.
- **ACCUMULATE_ON_CORRECTION** — attractive candidate but preferred entry requires a better valuation.
- **WAIT** — remain on the list; do not add materially at the current setup.
- **HOLD** — existing position can be maintained; no immediate allocation change.
- **REVIEW** — evidence has changed enough to require a fresh investment review before action.
- **TRIM** — reduce exposure because valuation, risk or thesis has deteriorated.
- **EXIT** — thesis failure or risk/reward no longer supports ownership.

`action` is independent of `status`. A CORE company can therefore be `WAIT`, `ACCUMULATE`, `HOLD`, etc.

## Identity rules

- ISIN is the canonical `id`.
- Ticker is retained for display/trading purposes.
- Exchange is deliberately excluded from the core identity model.
- Duplicate ISINs are not permitted.
- A ticker change does not create a new security record when the ISIN remains the same.

## Research ownership

Structured current-state fields belong in `universe.json`.
Detailed thesis, valuation work, risks, scenarios, evidence and decision history belong in the linked company Markdown file.

Do not duplicate the universe into separate CORE/WATCH/FRONTIER/REJECTED lists.
