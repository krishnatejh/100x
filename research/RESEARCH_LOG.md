# 100X Research Log

This log records material research events and thesis changes. Git history remains the authoritative record of file changes; this log captures the investment-research interpretation in a human-readable form.

## Entry format

- **Date:** YYYY-MM-DD
- **Company / topic:**
- **Type:** New / Update / Upgrade / Downgrade / Rejected / Reopened
- **Previous status/action:**
- **New status/action:**
- **What changed:**
- **Evidence:** Primary sources first; include links/citations in the company research file where appropriate.
- **Interpretation:** FACT / INFERENCE / SPECULATION
- **Decision impact:**
- **Next review question:**

## 2026-09-21 — NSE preliminary 100X review

- **Type:** New candidate / preliminary full-framework review
- **Company:** National Stock Exchange of India (NSE)
- **Previous status/action:** Not previously in canonical universe
- **New status/action:** WATCH / thesis UNDER_REVIEW / HOLD / fresh capital WAIT
- **What changed:** Added `companies/india/nse.md` with a preliminary assessment of NSE's market-infrastructure economics, network effects, transaction-revenue concentration, regulatory exposure, IPO valuation and 50X–100X mathematics.
- **Evidence:** September 2026 reporting indicates an IPO price band of ₹1,700–₹1,785, approximate valuation of ₹4.42 lakh crore at the upper band, and a 100% offer-for-sale structure. Reporting also highlights material dependence on transaction charges and options activity, along with regulatory and trading-volume risks. Primary-source RHP and audited-statement verification remains outstanding.
- **Interpretation:** FACT for reported IPO terms and externally reported risk factors; INFERENCE for moat durability, long-term economics and preliminary classification; SPECULATION avoided for the 50X–100X outcome.
- **Decision impact:** NSE is classified as WATCH, not CORE. Preliminary scores: Business Potential 8/10; Probability of Success 6/10; Investment Attractiveness 5/10; Overall 100X 6/10. `beyond_100x` remains false because no compelling alternative case outside the strict 100X framework has been established.
- **Next review question:** Verify the final RHP and financial statements, normalize earnings through regulatory/trading cycles, split revenue by product, compare competitive dynamics versus BSE, and build a per-share scenario model incorporating dividends, buybacks and share-count changes.

## 2026-09-05 — Re-rating review of CORE + WATCH universe

- **Type:** Re-rating review / research prioritisation
- **Companies:** E2E Networks; Kaynes Technology; Shivalik Bimetal; Pitti Engineering; Laurus Labs; PG Electroplast; Newgen Software; Cupid; Cyient DLM; remaining CORE universe
- **What changed:** A comparative review identified a new top-tier research queue. E2E Networks is now the highest-priority WATCH candidate because of its sharp Q1 FY27 AI-infrastructure growth and a reported ₹1,000 Cr binding term sheet for NVIDIA Blackwell GPU infrastructure/services. Kaynes Technology moved high on the queue because of its OSAT/PCB expansion. Shivalik Bimetal and Pitti Engineering also showed strong Q1 FY27 operating momentum. Laurus Labs merits a probability-of-success re-rating review after a major profitability recovery. PG Electroplast requires a CORE refresh, while Newgen and Cupid merit deeper work. Cyient DLM was explicitly placed on a CORE challenge list because return-on-capital and valuation may be less attractive than the best WATCH candidates.
- **Interpretation:** FACT for reported operating results and announced strategic developments; INFERENCE for the relative research priority and potential re-rating; SPECULATION avoided until 100X mathematics and valuation work is completed.
- **Decision impact:** No automatic status changes were made. The review is captured in `research/RE_RATING_REVIEW_2026-09-05.md` and establishes the next research sequence. Canonical status/action remains controlled by `data/universe.json`.
- **Next review question:** Complete E2E and Kaynes full 100X mathematics first, then compare Shivalik/Pitti/PGEL/Laurus/Newgen/Cupid and formally challenge Cyient DLM against the strongest alternatives.

## 2026-09-05 — CORE scoring and WATCH migration

- **Type:** Research migration / update
- **Companies:** Azad Engineering; Cyient DLM; Indo-MIM; PG Electroplast; Syrma SGS Technology; 59 WATCH candidates
- **What changed:** Completed a current primary-source-led scoring pass for the five previously unscored CORE companies. Formal Business Potential, Probability of Success, Investment Attractiveness and Overall 100X scores are now populated in `data/universe.json`; detailed research pages were refreshed accordingly. The legacy WATCH universe was also extracted into `data/watchlist_migration.json` as a staging layer.
- **Interpretation:** CORE scores are current research judgements, not copied legacy values. WATCH records preserve the legacy tracker state but are not yet promoted into the canonical universe because their ISINs have not been fully verified.
- **Decision impact:** CORE remains at six companies, with all six now scored. WATCH migration is staged without guessing stable identifiers.
- **Next review question:** Verify all WATCH ISINs against the NSE security master, create research pages, normalize actions to the Artha contract, and then promote the 59 records into `data/universe.json`.

## 2026-09-05 — CORE universe migration

- **Type:** Research migration / update
- **Companies:** Azad Engineering; Cyient DLM; Indo-MIM; PG Electroplast; Syrma SGS Technology
- **Previous status/action:** CORE / ACCUMULATE SLOWLY (Azad); CORE / ACCUMULATE (Cyient DLM); CORE / WAIT (Indo-MIM); CORE / ACCUMULATE (PG Electroplast); CORE / ACCUMULATE SLOWLY (Syrma SGS)
- **New status/action:** Same as above
- **What changed:** Migrated the five remaining CORE companies from the legacy tracker into the canonical `data/universe.json` structure and created linked company research pages. Existing tracker actions, valuation views, technical views, accumulation guidance and thesis-break triggers were preserved.
- **Interpretation:** FACT for migrated tracker decisions. The five companies did not have populated 100X score fields in the source tracker, so no scores were reconstructed or invented at migration.
- **Decision impact:** CORE classifications retained. Artha can now render all six CORE companies; all six are now formally scored.
- **Next review question:** Reassess CORE membership after comparing probability-weighted 100X potential across the complete universe.

## 2026-09-05 — MTAR Technologies

- **Type:** Research migration / update
- **Previous status/action:** CORE / WAIT
- **New status/action:** CORE / WAIT
- **What changed:** Migrated MTAR into the new canonical universe structure and completed a refreshed company research page covering FY26 and Q1 FY27 developments.
- **Interpretation:** Business evidence strengthened, but valuation remains a major constraint; no status upgrade was warranted.
- **Decision impact:** Retain CORE classification with WAIT action.
- **Next review question:** Quantify customer concentration and order-book conversion, then build a reverse-DCF / FY27–FY30 valuation sensitivity.

## 2026-09-08 — CORE action review

- **Type:** Action review / valuation discipline
- **Companies:** Azad Engineering; Cyient DLM; Indo-MIM; MTAR Technologies; PG Electroplast; Syrma SGS Technology
- **Previous status/action:** CORE / ACCUMULATE SLOWLY (Azad); CORE / ACCUMULATE (Cyient DLM); CORE / WAIT (Indo-MIM); CORE / WAIT (MTAR); CORE / ACCUMULATE (PG Electroplast); CORE / ACCUMULATE SLOWLY (Syrma SGS)
- **New status/action:** CORE / WAIT (Azad); CORE / WAIT (Cyient DLM); CORE / WAIT (Indo-MIM); CORE / WAIT (MTAR); CORE / ACCUMULATE SLOWLY (PG Electroplast); CORE / WAIT (Syrma SGS)
- **What changed:** A fresh comparative review found no reason to upgrade CORE status, but several legacy actions were inconsistent with the current Investment Attractiveness scores and valuation conclusions. Cyient DLM, Azad and Syrma now move to WAIT because high valuations and/or insufficient current return-on-capital evidence make active accumulation premature. PG Electroplast is reduced from ACCUMULATE to ACCUMULATE SLOWLY because growth remains attractive but capital efficiency and margin conversion need confirmation. Indo-MIM and MTAR remain WAIT.
- **Interpretation:** FACT for current reported operating evidence and the existing scorecards; INFERENCE for the action changes. No short-term price prediction is involved.
- **Decision impact:** CORE is now deliberately conservative: only PG Electroplast is an active accumulation candidate, and only slowly. No CORE company is currently rated for aggressive accumulation.
- **Next review question:** Challenge whether Cyient DLM and the most valuation-constrained CORE names should remain CORE after deeper comparison with E2E, Kaynes, Shivalik Bimetal, Pitti Engineering and other high-priority WATCH candidates.

## 2026-09-10 — Decision-model correction

- **Type:** Data-model and methodology correction
- **Problem:** The legacy single `action` field mixed two different decisions: what to do with an existing position and whether to deploy fresh capital. This caused the 2026-09-08 CORE review to make `WAIT` appear like a change in long-term ownership conviction.
- **Schema change:** Removed `action`; added `thesis_health`, `position_action`, and `fresh_capital_action`.
- **Enums:** Thesis health = STRENGTHENING / INTACT / UNDER_REVIEW / WEAKENING / BROKEN. Position action = HOLD / REDUCE / EXIT. Fresh capital action = DEPLOY / WAIT.
- **CORE correction:** A fresh-capital WAIT is explicitly not an exit signal. Existing CORE positions are HOLD unless explicit evidence supports REDUCE or EXIT.
- **Principle:** Valuation can change the attractiveness of new purchases without invalidating a 10–25+ year business thesis or requiring sale of an existing position.

## 2026-09-10 — Classification taxonomy foundation

- **Type:** Methodology and schema preparation
- **Decision:** Lock a three-dimensional classification model: `sector`, `industry`, and `themes`.
- **Sector:** Exactly one of the 11 GICS-aligned sectors.
- **Industry:** Exactly one controlled primary-business enum.
- **Themes:** Zero to five controlled cross-cutting opportunity areas.
- **Design principle:** Sector and industry describe what a company fundamentally is and does; themes describe structural opportunities, technologies, strategic value chains, or major end markets.
- **Migration status:** Taxonomy/schema/documentation updated only. Existing company values in `universe.json` have not yet been migrated; full company mapping will be reviewed separately.

## 2026-09-10 — Universe classification migration

- **Type:** Canonical data migration
- **Scope:** All 46 companies migrated from legacy free-text `sector` labels to the controlled three-dimensional taxonomy: `sector`, `industry`, and `themes`.
- **Rules applied:** Exactly one GICS-aligned sector, exactly one controlled primary industry, and zero to five controlled themes per company.
- **Purpose:** Separate economic classification from cross-cutting opportunity exposure and enable sector/industry concentration and theme/discovery-bias analysis.
- **Note:** Classification is a taxonomy normalization exercise, not a change to company status, thesis, scores, valuation, or investment action.

## 2026-09-10 — Schema v3.0 consistency cleanup

- Bumped canonical universe `schema_version` from `2.0` to `3.0` to reflect the breaking classification-model change.
- Clarified the theme-overlap rule: themes cannot merely restate primary industry, but controlled overlap is allowed for distinct end-market/discovery exposure (for example aerospace/defence).
- Regenerated `sectors/SECTOR_COVERAGE.md` from live canonical data with sector, industry and theme concentration views.
- Noted discovery concentration and global-search gaps.
- `artha-contract.json` intentionally excluded because it was removed and is no longer part of the repository contract.


## 2026-09-10 — E2E Networks full 100X review

- **Type:** Full research / status retained
- **Previous status/action:** WATCH / thesis UNDER_REVIEW / HOLD / fresh capital WAIT
- **New status/action:** WATCH (HIGH PRIORITY) / thesis UNDER_REVIEW / HOLD / fresh capital WAIT
- **What changed:** Completed the full 100X framework analysis covering business model, AI/GPU cloud opportunity, TAM/runway, financial inflection, moat, management, capital allocation, market-cap mathematics, reverse economics, valuation, scenarios, risks and sector-bias checks. Added the canonical research page at `companies/india/e2e-networks.md`.
- **Scores:** Business Potential 9.0/10; Probability of Success 5.5/10; Investment Attractiveness 5.0/10; Overall 100X Score 6.5/10.
- **Evidence:** Sharp AI-driven growth and encouraging GPU utilisation provide genuine positive evidence. The large AI infrastructure opportunity and L&T relationship strengthen the strategic case. Major unresolved issues remain around repeatable cluster economics, incremental ROIC, free-cash-flow conversion after replacement capex, competition, NVIDIA dependence, customer concentration, financing/dilution and valuation.
- **Interpretation:** FACT for reported operating developments and disclosed/announced infrastructure developments; INFERENCE for moat durability and long-term economics; SPECULATION explicitly separated for the 50X–100X outcome.
- **Decision impact:** No CORE promotion. E2E remains a HIGH-PRIORITY WATCH because business potential is exceptional but probability and investment attractiveness are not yet strong enough. The decisive question is whether E2E becomes a high-return AI platform or remains a capital-intensive GPU infrastructure operator.
- **Next review question:** Can multiple GPU clusters demonstrate sustained utilisation, attractive incremental ROIC and improving free-cash-flow conversion without excessive leverage or dilution?


## 2026-09-11 — ESDS Software Solution full 100X review

- **Type:** Full research / new candidate added
- **Previous status/action:** Not previously in canonical universe
- **New status/action:** WATCH (HIGH PRIORITY) / thesis UNDER_REVIEW / HOLD / fresh capital WAIT
- **What changed:** Completed a full 100X framework review and added ESDS Software Solution to `data/universe.json` with a canonical research page at `companies/india/esds-software-solution.md`. The review covered cloud/data-centre/managed-services/software economics, AI/GPU infrastructure, financial trajectory, moat, management, market-cap mathematics, valuation, scenarios, failure modes and discovery bias.
- **Scores:** Business Potential 8.5/10; Probability of Success 4.5/10; Investment Attractiveness 2.5/10; Overall 100X Score 5.5/10.
- **Evidence:** FY26 financial growth and profitability were strong. The large five-year Sharon AI agreement creates substantial upside optionality but is also the primary risk because the commitment is very large relative to ESDS's historical scale. Customer advances and headline contract values must not be confused with recurring free cash flow or automatically treated as ESDS revenue.
- **Interpretation:** FACT for reported financials, disclosed business lines and publicly disclosed contract arrangements; INFERENCE for moat and long-term value capture; SPECULATION explicitly separated for 50X–100X outcomes.
- **Decision impact:** ESDS is not promoted to CORE. It enters as a HIGH-PRIORITY WATCH with fresh capital WAIT. Current valuation and unresolved contract/unit-economics risk materially reduce investment asymmetry.
- **Next review question:** Do AI infrastructure deployments convert into independently verifiable revenue, sustained utilisation, attractive incremental ROIC and durable free cash flow without excessive leverage or dilution?
