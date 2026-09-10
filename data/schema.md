# 100X Universe Data Schema

`data/universe.json` is the canonical structured dataset for the 100X universe.

## Classification model

Each company uses three distinct classification dimensions:

- **Sector** — one broad economic sector, using the 11 GICS-aligned sectors.
- **Industry** — one controlled primary business classification.
- **Themes** — zero to five controlled cross-cutting technologies, structural opportunities, strategic value chains, or major end markets.

**Rule:** Sector and industry answer what the company fundamentally is and does. Themes answer which major long-term opportunity areas may materially influence growth.

## Classification enums

### Sector — exactly one
- `COMMUNICATION_SERVICES`
- `CONSUMER_DISCRETIONARY`
- `CONSUMER_STAPLES`
- `ENERGY`
- `FINANCIALS`
- `HEALTH_CARE`
- `INDUSTRIALS`
- `INFORMATION_TECHNOLOGY`
- `MATERIALS`
- `REAL_ESTATE`
- `UTILITIES`

### Industry — exactly one
- `SOFTWARE`
- `IT_SERVICES`
- `SEMICONDUCTORS`
- `TECHNOLOGY_HARDWARE`
- `ELECTRONIC_EQUIPMENT`
- `ELECTRONIC_MANUFACTURING_SERVICES`
- `COMMUNICATIONS_EQUIPMENT`
- `BANKS`
- `DIVERSIFIED_FINANCIALS`
- `CAPITAL_MARKETS`
- `INSURANCE`
- `AEROSPACE_DEFENSE`
- `MACHINERY`
- `ELECTRICAL_EQUIPMENT`
- `INDUSTRIAL_COMPONENTS`
- `ENGINEERING_SERVICES`
- `CONSTRUCTION_ENGINEERING`
- `TRANSPORTATION_LOGISTICS`
- `PHARMACEUTICALS`
- `BIOTECHNOLOGY`
- `LIFE_SCIENCES_TOOLS_SERVICES`
- `HEALTH_CARE_SERVICES`
- `MEDICAL_DEVICES`
- `AUTOMOBILES`
- `AUTOMOBILE_COMPONENTS`
- `HOUSEHOLD_DURABLES`
- `CONSUMER_PRODUCTS`
- `RETAIL`
- `TRAVEL_SERVICES`
- `FOOD_BEVERAGES`
- `HOUSEHOLD_PERSONAL_PRODUCTS`
- `AGRICULTURE`
- `CHEMICALS`
- `METALS_MINING`
- `CONSTRUCTION_MATERIALS`
- `ADVANCED_MATERIALS`
- `OIL_GAS`
- `ENERGY_EQUIPMENT`
- `POWER_GENERATION`
- `RENEWABLE_POWER`
- `POWER_TRANSMISSION`
- `TELECOM_SERVICES`
- `DIGITAL_PLATFORMS`
- `INTERACTIVE_MEDIA`
- `ENTERTAINMENT`
- `REAL_ESTATE`
- `REAL_ESTATE_SERVICES`

### Themes — zero to five
- `AI`
- `CLOUD`
- `CYBERSECURITY`
- `ADVANCED_COMPUTING`
- `DATA_INFRASTRUCTURE`
- `DIGITAL_TRANSFORMATION`
- `ROBOTICS_AUTOMATION`
- `QUANTUM_COMPUTING`
- `SEMICONDUCTOR_ECOSYSTEM`
- `CHIP_DESIGN`
- `CHIP_MANUFACTURING`
- `OSAT`
- `DEFENCE`
- `AEROSPACE`
- `SPACE`
- `DRONES`
- `ENERGY_TRANSITION`
- `ENERGY_STORAGE`
- `BATTERIES`
- `NUCLEAR`
- `ELECTRIFICATION`
- `GRID_MODERNIZATION`
- `CLIMATE_TECH`
- `BIOTECH_INNOVATION`
- `CDMO`
- `GENOMICS`
- `PRECISION_MEDICINE`
- `HEALTH_TECH`
- `FINTECH`
- `DIGITAL_PAYMENTS`
- `SAAS`
- `E_COMMERCE`
- `ADVANCED_MANUFACTURING`
- `PRECISION_MANUFACTURING`
- `WATER_INFRASTRUCTURE`
- `TELECOM_INFRASTRUCTURE`

## Classification rules

1. Every company has exactly **one sector**.
2. Every company has exactly **one industry**.
3. Every company has **zero to five themes**.
4. Sector is GICS-aligned and broad; industry represents the company's primary economic activity.
5. Themes must not be used merely to duplicate the industry. They represent cross-cutting structural opportunities, technologies, strategic value chains, or end markets.
6. Do not create ad-hoc labels. New enum values require an explicit taxonomy review.
7. Country/geography is not a theme; use the existing `country` field. Macro narratives belong in research unless a future controlled taxonomy explicitly adds them.

## Required company fields

| Field | Type | Purpose |
|---|---|---|
| `id` | string | Canonical security identity; must be unique |
| `name` | string | Display name |
| `ticker` | string | Trading symbol |
| `country` | string | Issuer geography |
| `currency` | string | ISO 4217 code |
| `sector` | enum | One GICS-aligned broad sector |
| `industry` | enum | One controlled primary industry |
| `themes` | array | Zero to five controlled themes |
| `status` | enum | Research classification |
| `thesis_health` | enum | Evolution of long-term thesis |
| `position_action` | enum | Action for an existing position |
| `fresh_capital_action` | enum | Whether new capital should be allocated now |
| `research_path` | string/null | Link to detailed research |
| `last_reviewed` | date | Freshness of structured assessment |
| `scores` | object | Four 0–10 scores |

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
- **HOLD** — continue owning.
- **REDUCE** — reduce exposure.
- **EXIT** — sell/close the position.

## Fresh-capital-action taxonomy
- **DEPLOY** — allocate fresh capital to the company.
- **WAIT** — do not allocate fresh capital now.

`WAIT` is not a sell signal. A company can be `HOLD` for an existing position and `WAIT` for fresh capital.

## Scores
- `business_potential`
- `probability_of_success`
- `investment_attractiveness`
- `overall_100x`

All scores use a 0–10 scale.
