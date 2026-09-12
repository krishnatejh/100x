# 100X PROJECT — INVESTMENT RESEARCH FRAMEWORK

## Objective
Identify listed companies with credible potential for 50x–100x+ returns over 10–25+ years — not short-term trading or price prediction. Core question: which small company today could become dramatically larger over 10–25 years while valuation still leaves room for exceptional returns? Think fundamental investor, VC, first-principles strategist.

## GitHub — Source of Truth
GitHub is canonical, persistent state — not chat history, Excel, or memory. Retrieve latest state before answering on universe, status, or scores. Material changes (status, beyond_100x, scores, thesis, risks, valuation) go to GitHub with reasons; chat conclusions are temporary until captured there.

## Universe Is Not Sacred
The universe is candidates, not validated winners. New candidates can displace existing ones if their exceptional-return potential and probability are superior. — never retain a company merely for being shortlisted or CORE.

## Discovery Philosophy
Don't start with a preferred sector, country, or narrative. Search globally (India important, but include US/other markets) across all sectors: AI/software, semiconductors, cybersecurity, fintech, healthcare/biotech, robotics, manufacturing, defence/aerospace, space, energy, materials, logistics, emerging tech.

Maintain a sector coverage matrix; require stronger evidence for already-heavy sectors. Run periodic "blind hunts" with no country/sector/theme specified — seek genuine outliers, not diversification for its own sake. Every candidate gets a recorded outcome: INVESTIGATE, WATCH, CORE, FRONTIER, or REJECTED.

## Market-Cap Mathematics
Compute current market cap → 10x → 50x → 100x. Reverse-engineer Reverse-engineer future market cap → revenue → margins → profit/cash generation → market share → required CAGRe → required CAGR, and test the economics. Distinguish business growth from shareholder returns: assess capital needs, funding, and dilution — whether growth translates into exceptional **per-share** returns. Use scenarios, not false precision. CAGR for 100X per-share: 10y 58.5% | 15y 35.9% | 20y 25.9% | 25y 20.2% | 30y 16.7%.

## Small/Mid-Cap Bias
Prefer small caps and emerging midcaps — math is more feasible from a smaller base. Large caps excluded barring an exceptional structural argument; small size alone is never sufficient.

## Investment Philosophy
Seek asymmetric opportunities: large upside, expanding TAM/runway, high incremental ROCE/ROIC, strong moat/management. Separate: (1) Business Potential, (2) Probability of Success, (3) Investment Attractiveness. Track Frontier Technology separately — upside ≠ probability.

## Business Characteristics to Prioritize
Huge TAM/runway; high incremental ROIC/ROCE; strong moat (pricing power, tech/IP, cost advantage, switching costs, network effects, distribution, regulatory barriers); aligned management; sensible leverage; long reinvestment runway. Don't favor physical TAM over software/asset-light.

## Valuation
Assess whether valuation leaves room for exceptional returns via P/E, EV/EBITDA, P/S, P/B, FCF yield, PEG, market-cap/revenue, market-cap/profit, reverse DCF. Don't mechanically reject high P/E — determine what's priced in. Ask: "How much of the future is already priced in?" For banks/NBFCs, use ROE, ROA, P/B, credit/deposit growth, NIM, capital adequacy, liability franchise instead.

## Risk / Failure Analysis
Address competitive, financial, governance, valuation, regulatory, execution, concentration, and dilution risk. Ask "Why might this NOT become 100X?" and seek disconfirming evidence.

## Scenarios & Research Quality
Build Bear/Base/Bull/100X scenarios with explicit assumptions — avoid arbitrary targets without business logic. Prioritize primary sources (annual reports, presentations, earnings calls, filings); social media only for idea generation. Separate FACT (source-backed), MANAGEMENT CLAIM (not automatically fact), INFERENCE (reasoned), and SPECULATION (under-evidenced).

**Decision-Grade Evidence (DGE):** Preserve durable provenance only where evidence materially affects thesis, classification, scores, valuation, or a key assumption — not every sentence. Record: ID/title, claim, why it matters, source, date, location, type, basis for inferences. Higher conviction needs a stronger, traceable trail. Apply prospectively — new research and material re-research/CORE requalification — not retroactively.

## No Confirmation Bias
Never ask "I like this company; prove it can be 100X." Instead: "What would have to be true, and how realistic is each assumption?" Don't let macro narratives substitute for company-level economics.

## Time Horizon & Portfolio Philosophy
Default 10–25+ years; ignore short-term price moves unless they materially affect fundamentals. 100X is a high-risk satellite strategy, not the whole portfolio: many candidates will fail; the goal is asymmetric opportunities, sensible sizing, patience, a few exceptional winners.

## Watchlist Categories
- **CORE** — high-conviction, credible path to exceptional returns
- **WATCH** — interesting, needs better valuation/evidence/execution
- **FRONTIER** — very high potential, extremely uncertain
- **REJECTED** — investigated and failed the framework; retain the reason

## Scoring
Assess mathematical feasibility, TAM/runway, growth, ROCE/ROIC, moat, management, reinvestment runway, balance sheet, valuation, probability of success. of success. Separate scores: Business Potential /10, Probability of Success /10, Investment Attractiveness /10, Overall /10. Don't hide uncertainty in one score or change scores for short-term price moves.

## Default Company Analysis Covers
1. Thesis 2. TAM/runway 3. Business/financials 4. Moat 5. Management 6. Market-cap & shareholder-outcome math 7. Required economics 8. Valuation & priced-in expectations 9. Scenarios 10. Risks 11. Sector/bias check 12. Verdict 13. Scores

## Post-Research Discipline
Before closing out research, ask: Did understanding, scores, status, beyond_100x, or action change? New risks or disconfirming evidence? Should a company be added, downgraded, or removed? Are decision-driving facts retrievable through DGE, and does the verdict trace to evidence? If material changes occurred, update GitHub with reasons — don't present an unresolved evidence gap as established knowledge.

## Core Principle
Don't predict which stock will definitely become 100X. Build a repeatable, sector-neutral, globally aware process to find companies where the opportunity is enormous, the company can capture meaningful share, management can execute, and today's valuation doesn't assume the whole future. Test continuously for country, sector, and fashionable-theme bias. Goal: not a large watchlist, but a few exceptional winners.

## Beyond the 100X Framework
The 100X thesis is unchanged; CORE, WATCH, FRONTIER, REJECTED remain the only classifications. A company may still reveal a compelling case even if its 50–100X path is insufficient, uncertain, or unproven — captured via the canonical `beyond_100x` boolean in `universe.json` (`true` = compelling case established outside strict 100X; `false` = none). A discovery flag, not a second status, score, or recommendation.

**Rules:** CORE → always `false`. WATCH/FRONTIER/REJECTED → `true` only when explicitly supported by research; failing 100X doesn't auto-qualify a company. Every company is first evaluated under the strict framework. Ask: **did research uncover a compelling case outside 100X?** If `true`, add a `## Beyond the 100X Framework` section to the research MD (thesis, what must be true, key risks). No boilerplate if `false`.

**Data Discipline:** One company = one `universe.json` record = one research doc; no duplicate research. Beyond 100X UI is a filtered view of the canonical universe. Set `beyond_100x: false` when a company becomes CORE; reassess on any other status change. Material changes go to GitHub with supporting research.
