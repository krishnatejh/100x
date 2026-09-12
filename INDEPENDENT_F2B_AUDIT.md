# Independent F2B Audit — 100X Research Operating System

## 1. Executive Verdict

### **OBJECTIVE PLAUSIBLE BUT PROCESS HAS MATERIAL GAPS**

**The framework can improve the questions you ask. The current operating system does not yet reliably turn those questions into better discovery, comparable decisions, or cumulative learning.**

Its central strength is the insistence that a large opportunity must translate into attractive business economics and shareholder returns from today’s valuation. Its central weakness is that **asking for this demonstration frequently substitutes for completing it**.

The repository currently supports a credible research checklist. It does not yet demonstrate a reliable exceptional-investment selection engine.

### What the actual state shows

| Observation | Current evidence | Audit implication |
|---|---|---|
| Geography | All **49 canonical companies are Indian**; the USA directory contains only `.gitkeep`. | Global discovery is an intention, not an operating result. |
| Classification | **6 CORE, 41 WATCH, 0 FRONTIER, 2 REJECTED.** | WATCH contains most of the universe and provides limited discrimination. |
| Research coverage | **39 of 49 records have no linked research and null scores.** | Most of the canonical universe is an intake backlog, not an evaluated opportunity set. |
| CORE provenance | All six CORE names were retained from the legacy tracker. Five subsequently received relatively short scoring summaries. | Existing membership has not been visibly re-earned under a common admission standard. |
| Economic concentration | Industrials and IT account for **28 of 49 records**. All six CORE companies have manufacturing-based business models. | Sector labels understate common economic exposures. |
| Evidence preservation | Several completed reviews list generic source categories without document links; CORE reports contain chat-local citation tokens. | Future sessions cannot efficiently reproduce important factual claims. |
| Governance freshness | The coverage matrix still reports **46 companies, 6 CORE and 40 WATCH**, under schema v3.0; the universe is v3.1. | Supporting memory already diverges from canonical state. |
| Learning | There is a documented correction to the action model, but no visible forecast-resolution or systematic cross-company learning process. | The system has demonstrated process repair, not yet improving investment judgement. |

Sources: `data/universe.json`, `research/RESEARCH_LOG.md`, `sectors/SECTOR_COVERAGE.md`.

The available Git history runs from September 5–12, 2026. That is too short to assess investment results or condemn an unfinished research queue. It is sufficient to identify structural weaknesses in admission standards, evidence preservation, discovery and learning.

**The most dangerous failure is not an obviously bad report. It is a plausible, polished report whose unresolved assumptions quietly become the starting facts of the next session.**

This audit evaluates the research system. Company examples test its methods and consistency; they are not investment judgements. Missing provenance establishes that evidence is difficult to verify—not that every unsupported claim is false.

---

## 2. End-to-End Objective Trace

Severity refers to the weakness in the current process.

| Link | What works | What can break | Severity |
|---|---|---|---|
| **Objective** | Explicit exceptional-return objective, long horizon, smaller-company preference and valuation awareness. | “50–100X+” becomes a binary 100X test; time horizon and shareholder-return convention remain elastic. | **HIGH** |
| **Framework** | Connects runway, moat, management, reinvestment, capital efficiency and price. | Topic coverage can count as completion without demonstrating the economic connection between them. | **CRITICAL** |
| **Discovery** | Recognises country/theme bias and calls for blind hunts. | Actual intake is India-only, heavily inherited and influenced by guidance, operating momentum and prominent themes. No search denominator is recorded. | **HIGH** |
| **Research** | Recent reports ask useful questions about replacement capex, contract economics and value capture. | Decisive questions are repeatedly deferred while reports are labelled complete and candidates receive scores. | **CRITICAL** |
| **AI Reasoning** | Instructions explicitly challenge narrative and confirmation bias. | No observable control separates independent reassessment from elaboration of earlier conclusions. Model/session standards can vary invisibly. | **HIGH** |
| **Evidence** | Primary sources are preferred; some direct links and reported/inferred distinctions exist. | Unresolvable citation tokens and generic source lists prevent claim-level verification. Management assertions can acquire the authority of established facts. | **CRITICAL** |
| **Decision** | Thesis health, existing-position action and fresh-capital action are separated. New candidates are not automatically promoted. | Incumbents have a weaker visible retention hurdle; scores lack defined meaning; unresolved challenges have no closure requirement. | **CRITICAL** |
| **GitHub Memory** | Current state, research files and Git history preserve substantial information. | They preserve conclusions better than the evidence, assumptions and comparisons that generated them. Current prose can conflict with structured state. | **HIGH** |
| **Future Research** | Reports contain next questions, upgrade conditions and a proposed research sequence. | No durable mechanism selects the next highest-value question, detects overdue work or prevents new stories displacing unresolved work. | **HIGH** |
| **Learning** | Some insights recur across reports; the action-model correction is real learning. | There is no routine that resolves predictions, analyses mistakes and changes how future companies are evaluated. | **HIGH** |

### Can a future session reconstruct the decision?

| Reconstruction requirement | Assessment |
|---|---|
| **Why was the decision made?** | Usually partly reconstructable for researched companies; original CORE admission rationale is much weaker. |
| **What evidence supported it?** | Often only broad source descriptions or summary statements survive. |
| **What assumptions were made?** | Some endpoint assumptions survive; funding, dilution, reinvestment and intermediate operating assumptions are usually incomplete. |
| **What uncertainty remained?** | Risk lists and open questions preserve this reasonably well, but rarely specify what resolves it. |
| **What alternatives were rejected?** | Two company rejections and several relative comparisons exist; no consistent contemporaneous comparison set is preserved. |
| **What changed and why?** | Git and the research log help, but material events are not consistently reflected across the current research surfaces. |

**Version history makes changes recoverable. It does not make investment reasoning reproducible.**

---

## 3. Top 10 Material Gaps

### 1. Canonical evidence is insufficiently verifiable — **CRITICAL**

**Gap and evidence:**
The E2E and ESDS reports declare full framework reviews but end with generic descriptions of sources reviewed. Their source sections contain no document URLs. The Knack and Ujjivan reviews have the same weakness. Several CORE reports preserve tokens such as `turn2search3`, which do not identify retrievable evidence within the repository.

See `companies/india/e2e-networks.md` §17, `companies/india/esds-software-solution.md` §18, and `companies/india/pg-electroplast.md`.

**Why it matters / failure mechanism:**
An erroneous financial figure, misunderstood contract or stale valuation can support a score, become canonical, and then anchor future research. Repetition creates apparent corroboration without new evidence.

**Recommended fix:**
For each decision-driving claim, retain the exact document, date/reporting period, page or section, and relevant excerpt or calculation. Distinguish:

- Reported historical result.
- Management claim or guidance.
- Analyst calculation.
- Unverified assertion.

An unresolved critical fact should block a high-conviction classification.

**Effort:** Low per new review; medium to repair existing priority records.
**Expected impact:** Very high—protects every downstream stage.

---

### 2. Market-cap mathematics is not yet a shareholder-return model — **CRITICAL**

**Gap and evidence:**
All six CORE reports use a 40× terminal P/E and 20% net margin in their illustrative reverse mathematics, without a sufficiently developed company-specific justification.

The issue is not that these endpoints are necessarily impossible. It is that they do substantial analytical work without an adequate bridge:

- PG Electroplast’s reported quarterly PAT margin is approximately **3.7%**, versus the assumed eventual **20%**.
- Cyient DLM’s reported EBITDA margin is approximately **10.5%**, while the endpoint assumes **20% net margin**.
- MTAR’s report gives FY26 revenue of ₹876 crore and required endpoint revenue around ₹268,000 crore. That requires approximately **25.7% revenue CAGR over 25 years**. The report’s broader “20%+ compounding” language does not explicitly reconcile this much more demanding operating requirement.

Sources: `companies/india/pg-electroplast.md`, `companies/india/cyient-dlm.md`, `companies/india/mtar-technologies.md`.

**Why it matters / failure mechanism:**
The system can manufacture feasibility by combining large TAM, unusually favourable terminal economics and an extended horizon. Mentioning dilution as a risk does not incorporate it into the return calculation.

For example:

```text
P_T / P_0 = (Market cap_T / Market cap_0) × (Shares_0 / Shares_T)
```

With 3% annual share-count growth over 25 years, a 100× market-cap increase produces only approximately **47.8× price appreciation**, before dividends and currency effects.

**Recommended fix:**
Use a compact, funded per-share bridge: operating growth → margins → reinvestment/cash generation → financing and dilution → terminal valuation → shareholder return. Test ordinary as well as optimistic terminal assumptions. Model banks through retained earnings, ROE and capital requirements.

**Effort:** Medium.
**Expected impact:** Very high—separates extraordinary company growth from extraordinary investment returns.

---

### 3. CORE is visibly grandfathered, not consistently requalified — **CRITICAL**

**Gap and evidence:**
The research log explicitly retains migrated CORE classifications. Git commit `99407ee` allowed unscored CORE records during migration. Subsequent scoring populated numbers but did not establish a common qualification gate.

Newer E2E and ESDS reviews require stronger proof before promotion. Existing CORE reports acknowledge unresolved capital efficiency, valuation and scale questions while retaining membership.

See `research/RESEARCH_LOG.md`: migration and action reviews.

**Why it matters / failure mechanism:**
The first shortlist acquires an incumbency advantage. New candidates must disprove uncertainty; incumbents survive because uncertainty has not yet disproved them.

A particularly revealing consistency test: the Knack rejection treats scale, capital intensity and insufficient moat evidence as exclusionary, while similar categories of unresolved risk coexist with CORE status elsewhere. This does not establish that the companies deserve identical decisions. It establishes that the **reason for applying different standards is not adequately demonstrated**.

**Recommended fix:**
Requalify all six CORE names using the same evidence and economic requirements applied to new candidates. Assess them initially without their old status or score. Compare qualified candidates against challengers, including an unrelated business model.

**Effort:** Medium.
**Expected impact:** Very high—removes path dependence from the most consequential classification.

---

### 4. Discovery controls describe bias but do not reliably change the search — **HIGH**

**Gap and evidence:**
All 49 canonical companies are Indian. The documented technical scope names India and USA, while the constitution calls for global discovery. No completed genuinely global blind-hunt record is visible.

The September 5–6 research queues lean heavily on recent results, management guidance and prominent industrial/AI opportunities.

Sources: `TECHNICAL_REFERENCE.md`, `research/RE_RATING_REVIEW_2026-09-05.md`, `research/2026-09-06-future-guidance-list-review.md`.

**Why it matters / failure mechanism:**
AI can repeatedly rediscover the companies most represented in accessible text. Asking it for ideas “without a preferred sector” does not remove its familiarity bias.

Candidate counts also do not measure search coverage. An empty sector could mean no search, poor sources, or a thorough search that found nothing.

**Recommended fix:**
Reserve recurring research time for searches drawn from actual listed-company populations, rotating geography, size and business economics. Record search scope, source, candidates screened and reasons for stopping.

Apply a common investment standard. Correct overrepresentation primarily by changing **where you search**, rather than imposing a harsher truth standard on an otherwise exceptional company.

**Effort:** Low to establish; recurring modest effort.
**Expected impact:** High—expands the opportunity set rather than repeatedly refining the same one.

---

### 5. Probability and scores lack operational meaning — **HIGH**

**Gap and evidence:**
The project requires “probability-weighted” exceptional-return comparisons but defines neither the event underlying “Probability of Success” nor scoring anchors.

E2E’s 100X probability is described as low while its probability score is 5.5/10. MTAR similarly describes the extreme outcome as low probability while recording 6.5/10. These could be consistent if the scores measure business success rather than 100X success—but that distinction is not specified.

**Why it matters / failure mechanism:**
Different sessions can score survival, business quality, execution or shareholder returns under the same label. Decimal scores create comparability that the underlying analysis does not support.

Large TAM, growth runway and business potential can also count the same attractive story multiple times.

**Recommended fix:**
Define separate questions:

1. Can the business survive and fund the next stage?
2. Can it establish durable attractive economics?
3. What supports an exceptional per-share outcome from the specified entry valuation?

Use broad, reasoned confidence ranges and relevant reference classes, including failures and ordinary outcomes. A 7/10 must not be interpreted as 70%. Remove the overall score as a decision gate unless its purpose is demonstrably useful.

**Effort:** Low to medium.
**Expected impact:** High—improves comparability and reduces fabricated certainty.

---

### 6. Disconfirmation is usually a future checklist, not a completed challenge — **HIGH**

**Gap and evidence:**
The template’s disconfirmation section asks for evidence that *would* weaken the thesis. Reports contain useful failure conditions, but little systematic recording of contrary evidence actively sought, found, adjudicated and reflected in decisions.

The Cyient CORE challenge is repeatedly deferred. Upgrade triggers such as “attractive incremental ROIC” and “better diversification” rarely specify a baseline, threshold or review date.

**Why it matters / failure mechanism:**
“Needs more proof” can persist indefinitely. Adverse developments can be narrated as temporary, while positive developments support strengthening conviction.

**Recommended fix:**
For every priority thesis, maintain three decision-driving assumptions with:

- Current evidence and strongest contrary evidence.
- Expected observable development.
- Review date or event.
- What result changes the classification or research priority.

Record unresolved disagreement rather than smoothing it into a balanced narrative.

**Effort:** Low.
**Expected impact:** High—makes conviction falsifiable.

---

### 7. The system lacks a substantive learning loop — **HIGH**

**Gap and evidence:**
The repository contains no systematic comparison of prior forecasts with outcomes, no error classification and no maintained set of transferable investment lessons.

There are beginnings: the action-model correction is genuine learning, and the E2E/ESDS reports share useful capital-intensity questions. But the latter transfer is incidental rather than required.

**Why it matters / failure mechanism:**
Every report can repeat the same errors about management guidance, working capital, terminal margins or reinvestment without making the next report better.

**Recommended fix:**
Resolve a few pre-recorded, decision-relevant expectations over 12–36 months. When an expectation fails, distinguish bad data, a weak economic model, poor judgement and genuinely unexpected events.

Add a short reusable lesson only when it changes a future question or decision rule, and identify the companies affected.

**Effort:** Low setup; modest recurring effort.
**Expected impact:** High and cumulative.

---

### 8. Research effort is not allocated by expected decision value — **HIGH**

**Gap and evidence:**
There are 41 WATCH records, 39 without linked research. A ranked sequence exists in a dated review, but no consistent mechanism explains subsequent reprioritisation, resolves stalled questions or limits active deep dives.

ESDS becomes another high-priority review while earlier work remains unfinished; no explicit opportunity-cost decision is recorded.

**Why it matters / failure mechanism:**
Novel stories can repeatedly displace difficult, potentially decisive work. The system optimises for producing a new report rather than improving an important decision.

**Recommended fix:**
Keep a short active queue—perhaps three substantive questions. Select work based on:

> How likely is resolving this question to change an important decision, and how much effort will it take?

Use cheap screening before full research. Give parked candidates a specific reopening condition. Reserve exploration time so existing names do not monopolise attention.

**Effort:** Low.
**Expected impact:** High—directly targets research value per hour.

---

### 9. Canonical memory has semantic drift and incomplete closure — **HIGH**

**Gap and evidence:**

- The coverage matrix is behind the universe.
- Knack and Ujjivan decisions exist in research files and Git, but not in the material research log.
- Ujjivan’s Beyond-100X section changed on September 12 while the canonical review date remains September 11.
- Kaynes has a clearly labelled example page saying **CORE placeholder**, while its canonical record is WATCH with no research link.
- MTAR’s current header says fresh capital WAIT, while its body still says “WAIT / accumulate in tranches.”

These are not all equally serious. The Kaynes page explicitly warns that it is a skeleton. Nevertheless, they demonstrate how a future AI session could retrieve incompatible meanings.

**Why it matters / failure mechanism:**
The session can select whichever conclusion best fits its current context. A schema-valid status does not prove the evidence, prose and decision history agree.

**Recommended fix:**
At material closeout, reconcile only the necessary surfaces: current JSON, company decision summary, material log, and coverage when affected. Mark historical and example content unmistakably. Define what `last_reviewed` certifies.

**Effort:** Low.
**Expected impact:** High—reduces silent context corruption without substantial infrastructure.

---

### 10. The objective can drift through an excessive focus on 100X and unbounded secondary research — **MEDIUM**

**Gap and evidence:**
The constitution targets **50–100X+**, but reports generally calculate 50X mechanically and devote the substantive feasibility argument to 100X.

Beyond 100X is explicitly constrained and currently flags only one company. That is not evidence of major mission drift. However, it creates another legitimate destination for interesting research without an explicit attention budget.

**Why it matters / failure mechanism:**
A plausible 50–70X investment can be screened out because 100X sounds implausible. Conversely, almost any appealing business can remain research-worthy under an increasingly broad interpretation of the project.

The distinction matters: 50X over 25 years requires approximately **16.9% annual compounding**, versus **20.2%** for 100X.

**Recommended fix:**
Define the return convention, horizon and entry valuation explicitly. Evaluate 50X and 100X separately. Keep Beyond-100X findings inexpensive to preserve and subordinate in research priority.

**Effort:** Low.
**Expected impact:** Medium to high—protects against both false negatives and diluted attention.

---

## 4. Strongest Argument Against the System

The strongest skeptical case is that this is an **incumbent-watchlist justification system with an excellent vocabulary**.

It begins with an inherited, India-heavy manufacturing shortlist. Existing favourites retain CORE status. Their reports acknowledge demanding valuations and weak or uncertain capital efficiency, then preserve the classification through favourable endpoint assumptions and language about eventual global platforms.

New candidates face a more demanding hurdle. Less fashionable business models can be rejected for lacking extreme scalability, while familiar industrial or AI stories retain optionality through a hypothetical business-model transformation.

AI makes this failure mode unusually dangerous. It can describe TAM, moat, capital allocation, downside and uncertainty fluently without resolving any of them. The result sounds skeptical because it contains risks. It sounds quantitative because it contains terminal market caps. It sounds calibrated because it contains four scores.

None of those features establishes that the selection is better.

The process may systematically encounter opportunities after strong results, major contracts or reratings have already attracted attention. It may then spend most of its time explaining why the future is exciting but the valuation is difficult. Meanwhile, less visible companies never enter the funnel.

Finally, because the system does not systematically resolve prior expectations or revisit false negatives, it can fail without discovering why. An eventual winner could validate the narrative retrospectively; repeated misses could be blamed on the inherent difficulty of finding 100-baggers.

**Under this failure mode, research output grows, apparent sophistication grows, and confidence grows. The probability of finding an exceptional investment need not improve at all.**

---

## 5. What Genuinely Works

These components have a plausible causal contribution to success.

### 1. Separating business potential from investment attractiveness

This prevents business admiration from automatically becoming a capital-allocation conclusion. The September 8 action review actually changed several accumulation actions because valuation and capital-efficiency evidence did not support them.

That is observable discipline, not merely an instruction.

### 2. Reverse economics as an early elimination tool

Used conservatively, market-cap mathematics quickly exposes how large an outcome must become. This can save substantial research effort.

Its value is in rejecting internally inconsistent stories—not certifying a precise 25-year endpoint.

### 3. Asking who captures the economic value

The E2E review distinguishes AI demand from profitable GPU ownership. The ESDS review distinguishes headline contract value, customer advances and recurring free cash flow; it also identifies the importance of which side of the contract ESDS occupies.

Those questions can materially change an investment thesis.

### 4. Refusing automatic promotion after positive news

E2E and ESDS remain WATCH despite strong narratives and operating developments. The re-rating review also explicitly prevents news-driven automatic upgrades.

This helps keep catalysts from substituting for underwriting.

### 5. Separating business deterioration from fresh-capital attractiveness

The action-model correction reduces the risk of treating “do not add now” as “the business thesis has failed.” That matters for retaining genuine long-duration winners.

It still needs an opportunity-cost discipline so HOLD does not become an endowment effect.

### 6. Preserving rejection reasons and current state

The two documented rejections can prevent repeat work. A canonical universe can stop each session from inventing its own current watchlist.

The benefit depends on preserving evidence and reasons alongside the labels.

---

## 6. Minimum High-Impact Improvements

The project does not need a redesign. Four operating changes would address most of the material gaps.

### Must Fix Now

#### 1. Replace “full report completed” with a decision-evidence gate

A priority review is decision-ready only when it contains:

- Traceable evidence for the critical facts.
- A funded per-share return bridge.
- The few assumptions that drive the result.
- The strongest contrary evidence.
- A classification justified against explicit alternatives.

Put this inside the existing company file. Missing decisive evidence remains visibly unresolved.

**First application:** requalify the six CORE names under this same standard.

#### 2. Turn open questions into scheduled decision tests

For each priority company, record three critical assumptions and the next event that can validate or weaken them. A review must resolve, revise or explicitly carry forward each test.

A missed test should trigger reassessment, not an automatic sell. Lack of evidence may reduce research conviction without establishing business failure.

### Should Fix Soon

#### 3. Run a bounded search-and-research queue

Maintain a small active queue with an explicit question and reason for priority. Protect recurring time for genuinely new discovery from outside the inherited geography and economic cluster.

Track search effort and qualified unfamiliar candidates, rather than watchlist size.

#### 4. Add a lightweight learning-and-closeout routine

When new evidence arrives:

1. Compare it with the prior expectation.
2. Record what the discrepancy teaches.
3. Apply that lesson to relevant other companies.
4. Reconcile the current decision, history and coverage.

This is one short routine, not four new databases.

### Nice to Have

- A few fixed example cases to check whether a changed model applies the framework differently.
- Saved excerpts of decision-critical sources where links may disappear.
- A simple historical review including failures, delistings and ordinary compounders.

These are useful after the evidence, economics and decision gates work. More elaborate scoring or taxonomy is not currently a priority.

---

## 7. Missing Feedback and Learning Loops

| Loop | Missing mechanism | Minimum useful implementation |
|---|---|---|
| **Discovery** | No connection between search method and subsequent candidate quality. | Record source/search scope and time spent; later identify which routes produced genuinely useful unfamiliar candidates. Revisit a sample of screened-out names. |
| **Research quality** | “Reviewed” is not tested against factual accuracy or reproducibility. | Recheck the few claims driving a decision. Track errors by type and repair the affected reasoning. |
| **Decision quality** | Scores and classifications are not compared with pre-recorded expectations. | Before deciding, state observable 12–36-month expectations. Review outcomes without rewriting the original forecast. |
| **Error correction** | A corrected fact need not propagate into other files or decisions. | Identify which thesis, score, comparator or classification depended on it; update those explicitly. |
| **Cross-company learning** | Insights remain embedded in company narratives. | Extract a bounded lesson, its evidence and exceptions; name the other candidates whose evaluation it changes. |

### Example of actual cross-company learning

Suppose research shows that customer advances explain most apparent operating-cash-flow strength during an expansion.

The lesson should become:

> For businesses using customer advances to fund expansion, separate financing-like cash inflows from recurring cash generation and examine the obligations attached to them.

The next relevant company review should apply that test automatically.

It should **not** become “customer advances are bad” or “capital-intensive companies cannot compound.” Learning requires a mechanism and its limits, not a new blanket prejudice.

For decision evaluation, track both errors:

- **False positives:** attractive-looking candidates whose economics fail to develop.
- **False negatives:** dismissed candidates whose per-share economics subsequently improve.

Reviewing only selected companies teaches the system how its favourites performed, not whether its selection method worked.

---

## 8. Practical AI Governance

### Minimum controls for a single-person project

| Failure mode | Practical control |
|---|---|
| **Hallucinated canonical facts** | Require exact source support for decision-driving facts. Verify issuer, reporting period, units and consolidated/standalone basis. Leave unknowns unknown. |
| **Confirmation bias** | Ask for the strongest evidence that contradicts the thesis, and the observation that would change the decision. A generic risks section does not satisfy this. |
| **Narrative bias** | Complete the economic bridge before writing the investment thesis. Remove fashionable labels and ask whether the remaining unit economics justify interest. |
| **Inconsistent scoring** | Use defined anchors and a common comparison sheet. Treat scores as ordinal summaries, not measured probabilities. Record why an assessment changed. |
| **Anchoring** | On major reviews, assess current evidence before revealing the previous score/status. Then reconcile the independent conclusion with history. |
| **Stale conclusions** | Separate source period, valuation date and thesis-review date. Use event-driven reviews plus a backstop review schedule for priority names. |
| **Changing model behaviour** | Record model and framework version for material decisions. When changing models, compare a few unchanged cases and explain divergent conclusions before accepting revised scores. |
| **Polished prose mistaken for evidence** | Open the review with three boxes: established evidence, decisive unknowns, and decision. Narrative quality never clears an evidence gap. |

Using a second model may expose different objections, but it does not provide independent evidence. Two models repeating the same unsupported assertion are one unsupported assertion repeated twice.

### Make classifications more meaningful without adding bureaucracy

- **CORE:** The evidence and economic qualification standard has been met, including a credible exceptional-return case tied to valuation. Existing membership receives no exemption.
- **WATCH:** State the actual blocker—unresearched, valuation, unit economics, execution or evidence—and the condition for another review.
- **FRONTIER:** Reserve for uncertainty about whether the technology or business model can become economically viable. Distinguish this from ordinary valuation or evidence uncertainty.
- **REJECTED:** Preserve the reason and whether reopening requires a price change, new evidence or a changed business model.

The existing schema also assigns HOLD to unresearched WATCH companies and EXIT to framework rejections. That is stronger than the underlying research may support. Allow “not assessed/not applicable” for position decisions rather than forcing an ownership conclusion.

**Failure to qualify for a 100X research strategy does not, by itself, establish that an existing position should be sold.**

### Minimum drift prevention

Before closing a material review, answer:

1. Does the current classification match the written decision?
2. Are the decisive facts and assumptions retrievable?
3. Is the next decision test explicit?
4. Did relevant history and coverage change?
5. Did this reveal a lesson that affects another company?

That is sufficient governance for a single-user project. Most additional controls would have lower value than doing the research these questions expose.

---

## 9. Final Answer

### **No.**

**I would not currently trust this operating system’s classifications and scores as the principal basis for finding one or two extraordinary listed-company winners.**

I would use its framework to organise initial investigation. I would independently reconstruct the evidence and economics before relying on its conclusions.

What must change is specific:

1. **CORE must be earned under a common current standard, including by incumbents.**
2. **Critical facts must remain verifiable outside the original AI session.**
3. **Exceptional returns must be demonstrated per share, after funding requirements, dilution and valuation—not inferred from company scale.**
4. **Discovery must systematically reach beyond the inherited India-heavy opportunity set.**
5. **Research must resolve assumptions and improve subsequent decisions, rather than repeatedly restating what needs to be proven.**

The project’s greatest opportunity is not to produce more comprehensive reports. It is to become more selective about which unanswered questions deserve work—and more demanding about what counts as an answer.

**The decisive test is whether the next research cycle causes you to discover a genuinely overlooked candidate, reject a previously attractive story, or change an important decision for a traceable reason. If it only produces another polished report, the operating system is not yet doing its job.**
