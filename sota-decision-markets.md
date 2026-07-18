# decision markets — SoTA bibliography

A completeness (long-list) bibliography of the decision-market research
line — the companion to the hand-curated shortlist in
[README](README.md) and the objection index in
[counterarguments](counterarguments.md).

> Status: **v0**, compiled from the maintainer's reference library. The
> README stays a hand-picked shortlist; this is the completeness pass.
> Years/attributions still being verified.

## foundations

- Hanson (1999), [*Decision Markets*](https://mason.gmu.edu/~rhanson/decisionmarkets.pdf) — the early concise formulation of markets that estimate consequences conditional on decisions.
- Hanson (2000/2013), *Shall We Vote on Values, But Bet on Beliefs?* — the futarchy proposal.
- Othman & Sandholm (2010), *Decision Rules and Decision Markets* — when the price drives the choice, naïve decision rules are manipulable (unbounded worst case); the problem the solutions below answer.

## SoTA solutions

Two solution families for the truthfulness problem — randomize the decision, or don't.

*Randomize (full support):*
- Chen & Kash (2011), *Information Elicitation for Decision Making* — the full-support characterization: the decision rule must sometimes randomize.
- Chen, Kash, Ruberry & Shnayder (2011), *Decision Markets with Good Incentives* — the strictly-proper construction (inverse-probability decision scoring).
- Chen et al. (2014), *Eliciting Predictions and Recommendations for Decision Making* — extends elicitation-for-decisions.

*Don't randomize (equity / decision scoring rules):*
- Oesterheld & Conitzer (2020), *Decision Scoring Rules* — follow the recommendation, pay the expert in shares of the outcome; truthful with no exploration cost, but only the recommended action's value is elicited.
- Oesterheld (2017), *Futarchy Implements Evidential Decision Theory* — why the deterministic route is evidential, not causal (see counterarguments A3).

## manipulation: theory & evidence

*Theory:*
- Chen, Dimitrov, Sami, et al. (2010), *Gaming Prediction Markets: Equilibrium Strategies with a Market Maker* — strategic (non-myopic) manipulation of an MSR market maker.

*Evidence:*
- Hanson, Oprea & Porter (2006), *Information Aggregation and Manipulation in an Experimental Market* — lab manipulators are countered; accuracy holds.
- Hanson & Oprea (2009), *A Manipulator Can Aid Prediction Market Accuracy* — manipulation can raise accuracy via added liquidity.
- Teschner (2017), *Manipulation in Conditional Decision Markets* — a decision-market experiment with profitable manipulation (counterargument B10).

*Aggregation limits:*
- Ostrovsky (2012), *Information Aggregation in Dynamic Markets with Strategic Traders* — separable securities aggregate; others need not.

*Recent:*
- Gill et al. (2025), *The Microstructure of Conditional Prediction Markets: A Theory of Selection, Multiplicity, and Mode Collapse in Futarchy* — formal selection / multiplicity / mode-collapse (counterargument A11).

## governance applications

- Hahn & Tetlock (2005), *Using Information Markets to Improve Public Decision Making* — the peer-reviewed case for information markets in public decisions.
- Hanson (2007), *The Policy Analysis Market: A Thwarted Experiment in the Use of Prediction Markets for Public Policy* — the DARPA public-policy market episode.
- Abramowicz (2008), [*Predictocracy: Market Mechanisms for Public and Private Decision Making*](https://academic.oup.com/yale-scholarship-online/book/19774) — a book-length treatment of prediction-market mechanisms for legislatures, agencies, corporations, and courts.
- Merkle, *DAOs, Democracy and Governance* — self-modifying goal-driven organizations (also in the README).
- Buterin (2016), *Casper interest rates as a futarchy objective function*.

## see also

- DM-adjacent mechanisms → [sota-dm-adjacent.md](sota-dm-adjacent.md)
- objections → [counterarguments.md](counterarguments.md)
