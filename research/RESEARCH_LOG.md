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
