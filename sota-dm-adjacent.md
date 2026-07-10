# DM-adjacent information-market mechanisms — SoTA

information-market and elicitation mechanisms that are *not* decision
markets per se, but share properties that let them be assimilated into
decision-market design. this list is a bid to map and categorize that
space.

> **defining "DM-adjacent" — deliberately open.** a working boundary: a
> mechanism is DM-adjacent if it elicits decision-relevant signals from
> incentivized agents with an incentive-compatibility or identification
> property that transfers to, or composes with, decision-market design.
> this definition is provisional on purpose — sharpening it is the point
> of owning the category.
>
> status: **v0**, seeded from the maintainer's reference library.

## a. peer prediction / elicitation without ground truth

rewarding truthful reports when no verifiable outcome exists — a cousin
of the decision-market identification problem.

- Miller, Resnick & Zeckhauser (2005), *Eliciting Informative Feedback: The Peer-Prediction Method* — the foundational construction.
- Witkowski & Parkes, *Peer Prediction with Private Beliefs*.
- Frongillo & Witkowski (2016), *A Geometric Method to Construct Minimal Peer Prediction Mechanisms*; (2017) *A Geometric Perspective on Minimal Peer Prediction*; (2013) *Learning the Prior in Minimal Peer Prediction*.
- Kong, Schoenebeck et al. (2020), *Information Elicitation Mechanisms for Statistical Estimation*.
- Zheng et al. (2021), *The Limits of Multi-task Peer Prediction*.

## b. proper & market scoring rules / market-maker theory

the pricing substrate decision markets run on.

- Chen & Vaughan (2010), *A New Understanding of Prediction Markets via No-Regret Learning*.
- Chen & Pennock (2012), *A Utility Framework for Bounded-Loss Market Makers*.
- *An Axiomatic Study of Scoring Rule Markets* (2018).
- Frongillo & Waggoner, *Elicitation and Machine Learning* (survey).
- *An Axiomatic Characterization of Continuous-Outcome Market Makers* (2010).

## c. CFMM ↔ prediction-market equivalence

the bridge from DeFi constant-function market makers to prediction-market
scoring rules — the property that lets on-chain liquidity venues be read
as prediction mechanisms.

- Frongillo et al. (2023), *An Axiomatic Characterization of CFMMs and Equivalence to Prediction Markets*.
- Waggoner, *CFMMs and Equivalence to Prediction Markets* (a16z crypto talk).
- Angeris et al. (2020), *Improved Price Oracles: Constant Function Market Makers*; (2021) *Replicating Market Makers*.

## d. self-resolving / unverifiable-outcome markets

- Srinivasan et al. (2023), *Self-Resolving Prediction Markets for Unverifiable Outcomes*.

## e. combinatorial / structured markets

- Hanson, *Combinatorial Information Market Design* (the LMSR / combinatorial line).

## f. on-chain oracle & PM platforms (practitioner adjacency)

- Peterson et al. (2018), *Augur: a decentralized oracle and prediction market platform*.
- Zeitgeist, *Rikiddo Scoring Rule*.
- Sztorc, *Extra-Predictive Applications of Prediction Markets*; *Peer-to-Peer Oracle System and Prediction Marketplace*; *Unlocking the Power of Prediction Markets*.
- Clark et al., *On Decentralizing Prediction Markets and Order Books*.

## see also

- core decision markets → [sota-decision-markets.md](sota-decision-markets.md)
- objections → [counterarguments.md](counterarguments.md)
