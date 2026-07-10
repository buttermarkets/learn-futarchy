# decision-market counterarguments

an adversarial index of the known arguments for why decision markets
(and futarchy) fail — or fail in specific cases. the companion to the
[literature](README.md): where that list is what to read, this is what
to answer.

each entry is a single objection, its one-line claim, its class, and a
source. **class**: `F` = formal (a theorem, closed form, or model);
`I` = informal (argued, empirical, or design-level). the catalog is
deliberately neutral — it states each objection at its strongest and
does not rank or rebut them here.

> status: **v0 seed** — compiled from the public literature and the
> practitioner corpus (Hanson, Othman–Sandholm, Chen–Kash,
> Oesterheld–Conitzer, Dynomight, distbit, Rasmont, and others).
> incomplete by design; the numerous informal/practitioner objections
> are still being folded in.
>
> companions: the SoTA bibliographies
> [decision markets](sota-decision-markets.md) and
> [DM-adjacent mechanisms](sota-dm-adjacent.md).

---

## a. identification & decision theory

the family that says a conditional price is not the causal quantity a
decision-maker needs.

| id | counterargument | claim | class | source |
|----|-----------------|-------|-------|--------|
| A1 | conditioning ≠ intervening | conditional price `E[W|A]` diverges from `E[W|do(A)]` whenever choosing `A` is itself evidence about hidden fundamentals | I/F | greaterwrong, [Prediction Markets are Confounded](https://www.greaterwrong.com/posts/xnC68ZfTkPyzXQS8p/prediction-markets-are-confounded-implications-for-the); PhilH |
| A2 | decision selection bias | information arriving between pricing and decision biases the accepted set; acceptance correlates with the good state | F | Hanson, "decision selection bias" |
| A3 | futarchy implements EDT | conditional-market governance is evidential, not causal, decision theory | F | Oesterheld (2017) |
| A4 | bribe ≤ mechanism value (FDT) | a pure-mechanism market is CDT-shaped; a bribe exceeding its own value defeats it, and unbounded (FDT) resistance is unreachable | I | distbit |
| A5 | Bronze Bull / endogenous selection | approval signals fundamentals; corrective causal trades get refunded exactly in the branch where they'd matter, so arbitrage never fixes the bias | I | Rasmont (LessWrong) |
| A6 | cancellation option value | refunds in the void branch rationally inflate the conditional price (e.g. ~74¢ on a 59% coin) | F | Dynomight |
| A7 | closed-form cost of DSB | even ideal traders leave a bias `p(1-p)/(2-p)` under endogenous acceptance | F | distbit (ggresearch) |
| A8 | partial randomization only attenuates | ε-randomization scales the confound by `(1-ε)`; a 5% coin flip leaves ~95% of it | F | distbit; Hanson |
| A9 | no-reversion futility | partial randomization *without* market reversion has optimal randomization = 0 (bias rises with decision accuracy) | F | distbit (ADSB trilemma) |
| A10 | conditional accuracy is data-hungrier | an `x%`-probability event needs ~`1/x` more markets than the unconditional version to reach the same accuracy | I | practitioner (ggresearch) |
| A11 | selection / multiplicity / mode collapse | conditional-PM microstructure admits multiple equilibria and can collapse onto one mode, so the price need not track the intended counterfactual even absent manipulation | F | Gill et al. (2025), *Microstructure of Conditional Prediction Markets* |

## b. manipulation & adversarial

the family that says a strategic actor can move the answer.

| id | counterargument | claim | class | source |
|----|-----------------|-------|-------|--------|
| B1 | unbounded manipulation | under a max-price rule with cancellation, a correct-belief trader profitably pumps an inferior action; with unbounded scoring (incl. LMSR) the worst-case approximation ratio is unbounded | F | Othman & Sandholm (2010) |
| B2 | capital-efficiency asymmetry | an attacker needs capital for one outcome token; a loss-free defender must mint/hold the full set — an n:1 capital lock that lets small capital win far from the decision | I/F | distbit (ggresearch) |
| B3 | self-fulfilling metric manipulation | buy the funded outcome token cheap, move the metric yourself, let the market resolve your way | I | distbit (ggresearch) |
| B4 | Goldilocks liquidity band | impact is measurable only in a narrow liquidity range: too shallow and prices are spoofable, deep enough and manipulating the metric itself is cheaper | I | distbit |
| B5 | dissipative-KPI failure | a metric resists manipulation only if moving it is costly *and* the cost can't be recycled; TVL and per-app fees fail, ETH tx-fees pass | I | distbit |
| B6 | unconditional front-running | on unconditional KPI markets, speculators front-run the project against itself | I | lajarre; Sztorc/Hivemind lineage |
| B7 | influence market from rare settlement | when only a small branch settles but the large branch drives the real decision, outside-stake actors distort prices while facing settlement risk only on the rare branch | I | greaterwrong; distbit |
| B8 | blackmail attack | threaten to move the metric/market unless paid off | I | distbit |
| B9 | wash trading / coordinated bidding | collusive volume and curation-auction rings | I | general |
| B10 | manipulation confirmed experimentally | in lab conditional decision markets, traders profitably manipulate the decision — not just a worst-case theorem | F | Teschner (2017), *Manipulation in Conditional Decision Markets* |

## c. objective & metric governance (Goodhart family)

the family that says even a perfectly-run market optimizes the wrong,
or a decaying, thing.

| id | counterargument | claim | class | source |
|----|-----------------|-------|-------|--------|
| C1 | Goodhart / benchmark capture | optimizing a proxy corrupts it; stronger optimizers make it worse | I | Goodhart lineage |
| C2 | metric lifecycle / goal drift | the hard problem is governing the metric over time (audit, revise, rotate), not choosing it once | I | Bolton, [Futarchy of Mutating Preferences](https://thequantummilkman.substack.com/p/futarchy-of-mutating-preferences) |
| C3 | objective hijacking in repeated markets | round-by-round rule adjustment makes traders price "what survives the next filter," not the counterfactual | I | Merkle critique; practitioner |
| C4 | semantic fragility | ambiguous KPIs ("is the protocol healthy") are not objectively resolvable | I | practitioner (red-team) |
| C5 | metric self-modification | self-referential rule/metric changes destabilize the objective | I | Hanson, on Merkle's futarchy |

## d. institutional & political economy

the family that says the market can't stand where governance must.

| id | counterargument | claim | class | source |
|----|-----------------|-------|-------|--------|
| D1 | parasitic on governance | futarchy needs a working governance to define and enforce what it governs; it can't bootstrap its own legitimacy | I | greaterwrong, [Futarchy is Parasitic on What It Tries to Govern](https://www.greaterwrong.com/posts/mW4ypzR6cTwKqncvp/futarchy-is-parasitic-on-what-it-tries-to-govern) |
| D2 | principal-agent blocker | principals rarely let markets actually decide; firms ran internal prediction markets for decades without binding them | I | practitioner |
| D3 | state-capacity requirement | market governance sits on top of enormous institutional capacity; weak states are bad hosts | I | practitioner |
| D4 | sovereign boundary | permissionless markets let foreign capital buy domestic policy signals | I | practitioner |
| D5 | toxic flow vs civic truth-telling | insider participation is simultaneously the source of value and the corruption risk | I | practitioner |
| D6 | a price is not a reason | reasoned-record institutions cannot act on "the market moved to 0.73" without a translation layer | I | practitioner (admin-law) |

## e. liquidity & microstructure

| id | counterargument | claim | class | source |
|----|-----------------|-------|-------|--------|
| E1 | thin liquidity (classic) | decision markets are too thin to say anything | I | Hanson-era debate (now aging) |
| E2 | ghost / agentic liquidity | under agent trading, real depth is hard to distinguish from spoofed depth | I | practitioner (open) |
| E3 | adverse selection | informed flow drives quoted spreads / distorts prices | I | practitioner |
| E4 | beauty-contest dynamics | near thresholds, traders price others' expected pricing, not fundamentals | I | Keynes lineage |

## f. mechanism-design pathologies

| id | counterargument | claim | class | source |
|----|-----------------|-------|-------|--------|
| F1 | deterministic rules aren't IC | any deterministic report→allocation rule on conditional markets inherits max-rule manipulability (e.g. the share ≠ contribution bug in proportional funding) | F | Chen–Kash lineage |
| F2 | invalid / N-A resolution | how to price and resolve a "neither / void" branch without a free option | I | practitioner |

## g. epistemic & AI-era

| id | counterargument | claim | class | source |
|----|-----------------|-------|-------|--------|
| G1 | monoculture | shared model priors collapse epistemic diversity into correlated errors | I | practitioner (red-team) |
| G2 | singleton risk | binding futarchy is a path to a governance singleton | I | practitioner |
| G3 | Goodhart acceleration under agents | stronger optimizers make benchmark choice more consequential, not less | I | practitioner |

---

## how to use this

these are the objections any serious decision-market design has to
survive. a design's honesty is measured by which rows it answers with a
mechanism, which it bounds, and which it concedes as out of scope. the
strongest recent work does not claim to defeat every row — it is
explicit about which family it lives in.
