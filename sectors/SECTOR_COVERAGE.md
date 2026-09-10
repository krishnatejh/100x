# 100X Coverage Matrix

This is a **discovery-control layer**, not an investment ranking. It tracks the canonical universe using the controlled `sector`, `industry`, and `themes` taxonomy to identify concentration and discovery bias.

**Snapshot:** schema v3.0; 46 companies (6 CORE, 40 WATCH).

## Sector coverage

| Sector | Total | CORE | WATCH | FRONTIER | REJECTED |
|---|---:|---:|---:|---:|---:|
| INDUSTRIALS | 15 | 3 | 12 | 0 | 0 |
| INFORMATION_TECHNOLOGY | 12 | 2 | 10 | 0 | 0 |
| HEALTH_CARE | 7 | 0 | 7 | 0 | 0 |
| CONSUMER_DISCRETIONARY | 5 | 1 | 4 | 0 | 0 |
| ENERGY | 3 | 0 | 3 | 0 | 0 |
| MATERIALS | 2 | 0 | 2 | 0 | 0 |
| COMMUNICATION_SERVICES | 1 | 0 | 1 | 0 | 0 |
| UTILITIES | 1 | 0 | 1 | 0 | 0 |

## Industry concentration

| Industry | Total | CORE | WATCH | FRONTIER | REJECTED |
|---|---:|---:|---:|---:|---:|
| ELECTRICAL_EQUIPMENT | 6 | 0 | 6 | 0 | 0 |
| PHARMACEUTICALS | 6 | 0 | 6 | 0 | 0 |
| ELECTRONIC_MANUFACTURING_SERVICES | 4 | 2 | 2 | 0 | 0 |
| AEROSPACE_DEFENSE | 3 | 1 | 2 | 0 | 0 |
| AUTOMOBILE_COMPONENTS | 3 | 0 | 3 | 0 | 0 |
| ENERGY_EQUIPMENT | 3 | 0 | 3 | 0 | 0 |
| INDUSTRIAL_COMPONENTS | 3 | 1 | 2 | 0 | 0 |
| ADVANCED_MATERIALS | 2 | 0 | 2 | 0 | 0 |
| COMMUNICATIONS_EQUIPMENT | 2 | 0 | 2 | 0 | 0 |
| CONSTRUCTION_ENGINEERING | 2 | 0 | 2 | 0 | 0 |
| ELECTRONIC_EQUIPMENT | 2 | 0 | 2 | 0 | 0 |
| HOUSEHOLD_DURABLES | 2 | 1 | 1 | 0 | 0 |
| SOFTWARE | 2 | 0 | 2 | 0 | 0 |
| DIGITAL_PLATFORMS | 1 | 0 | 1 | 0 | 0 |
| IT_SERVICES | 1 | 0 | 1 | 0 | 0 |
| LIFE_SCIENCES_TOOLS_SERVICES | 1 | 0 | 1 | 0 | 0 |
| MACHINERY | 1 | 1 | 0 | 0 | 0 |
| RENEWABLE_POWER | 1 | 0 | 1 | 0 | 0 |
| TECHNOLOGY_HARDWARE | 1 | 0 | 1 | 0 | 0 |

## Theme concentration

Themes are cross-cutting and a company may appear in multiple theme counts.

| Theme | Total | CORE | WATCH | FRONTIER | REJECTED |
|---|---:|---:|---:|---:|---:|
| ADVANCED_MANUFACTURING | 11 | 4 | 7 | 0 | 0 |
| DEFENCE | 9 | 3 | 6 | 0 | 0 |
| ELECTRIFICATION | 9 | 0 | 9 | 0 | 0 |
| PRECISION_MANUFACTURING | 8 | 3 | 5 | 0 | 0 |
| AEROSPACE | 7 | 3 | 4 | 0 | 0 |
| CDMO | 7 | 0 | 7 | 0 | 0 |
| ENERGY_TRANSITION | 6 | 0 | 6 | 0 | 0 |
| GRID_MODERNIZATION | 6 | 0 | 6 | 0 | 0 |
| CLIMATE_TECH | 5 | 0 | 5 | 0 | 0 |
| AI | 3 | 0 | 3 | 0 | 0 |
| DIGITAL_TRANSFORMATION | 3 | 0 | 3 | 0 | 0 |
| SEMICONDUCTOR_ECOSYSTEM | 3 | 1 | 2 | 0 | 0 |
| ADVANCED_COMPUTING | 2 | 0 | 2 | 0 | 0 |
| BIOTECH_INNOVATION | 2 | 0 | 2 | 0 | 0 |
| DATA_INFRASTRUCTURE | 2 | 0 | 2 | 0 | 0 |
| DRONES | 2 | 0 | 2 | 0 | 0 |
| CLOUD | 1 | 0 | 1 | 0 | 0 |
| NUCLEAR | 1 | 1 | 0 | 0 | 0 |
| SAAS | 1 | 0 | 1 | 0 | 0 |
| SPACE | 1 | 0 | 1 | 0 | 0 |
| TELECOM_INFRASTRUCTURE | 1 | 0 | 1 | 0 | 0 |
| WATER_INFRASTRUCTURE | 1 | 0 | 1 | 0 | 0 |

## Current discovery-bias observations

1. **Industrials and Information Technology dominate the universe.** Together they account for 27 of 46 candidates (59%). New candidates from these sectors should require stronger comparative evidence.
2. **Manufacturing exposure is heavy.** Advanced Manufacturing and Precision Manufacturing are among the most represented themes; this reflects the current discovery history and should not be mistaken for diversification.
3. **Strategic/industrial themes are well represented.** Defence, Aerospace, Electrification and Grid Modernization already have meaningful coverage.
4. **Healthcare is concentrated around Pharmaceuticals/CDMO.** Broader biotechnology, medical devices and health-tech discovery remains relatively underrepresented.
5. **AI/software breadth remains limited relative to the project's intended global search scope.** Existing AI exposure is concentrated in a small number of infrastructure/software candidates.
6. **Financials, Consumer Staples, Real Estate and several GICS sectors have no current candidates.** Absence is not a reason to force additions, but blind hunts should test whether attractive outliers exist.
7. The universe is currently India-only despite `countries` allowing India and USA. Global discovery remains an explicit process requirement.

## Rules

1. Do not add a company solely to improve diversification.
2. When a sector, industry, or theme is already heavily represented, require stronger company-level evidence before adding another candidate.
3. A fashionable theme does not increase probability of success by itself.
4. Maintain a separate FRONTIER bucket for extreme technology/business uncertainty.
5. Run periodic blind hunts with no predefined sector, country, or theme and compare results against this matrix.
6. Update this document whenever a material universe change affects classification coverage or concentration conclusions.
