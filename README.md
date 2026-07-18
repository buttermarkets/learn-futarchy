# learn futarchy

## start here

- [Prediction market FAQ](https://www.astralcodexten.com/p/prediction-market-faq) (Astral Codex Ten)
- Alex Tabarrok and Scott Kominers, [Prediction markets & information-aggregation mechanisms](https://a16zcrypto.com/posts/podcast/prediction-markets-information-aggregation-mechanisms) (a16z podcast)
- Buterin, [Introduction to Futarchy](https://blog.ethereum.org/2014/08/21/introduction-futarchy) (Ethereum blog)
- Hanson, [Futarchy Details](https://www.overcomingbias.com/p/futarchy-details)
- Robin Hanson @ GG24, [Governance via Prediction Markets](https://www.youtube.com/watch?v=72wyqDQnbT4)
- Martin Köppelmann, [The Road to Futarchy](https://www.youtube.com/watch?v=FUAdCatOM-M)

## literature

### what is futarchy?

*Separate values (voted) from beliefs (bet), then let markets pick the policy that best serves the metric.*

- Hanson, [Futarchy: Vote Values, But Bet Beliefs](https://mason.gmu.edu/~rhanson/futarchy.html)
- Distbit, [The Different Types of Futarchy](https://github.com/buttermarkets/ggresearch/blob/main/topic/gov-designs/the-different-types-of-futarchy-more-than-you-wanted-to-know.md) (the landscape)
- Buterin, [From prediction markets to info finance](https://vitalik.eth.limo/general/2024/11/09/infofinance.html) (the broader frame)

### the market engine

*How beliefs become a tradeable, always-priced signal.*

- Hanson, [Combinatorial Information Market Design](https://mason.gmu.edu/~rhanson/combobet.pdf)
- Hanson, [Logarithmic Market Scoring Rules](https://mason.gmu.edu/~rhanson/mktscore.pdf)
- Wolfers, Zitzewitz, [Prediction Markets](https://users.nber.org/~jwolfers/Papers/Predictionmarkets.pdf) (do markets aggregate?)
- Hanson, Oprea, Porter, [Information Aggregation and Manipulation in an Experimental Market](https://mason.gmu.edu/~rhanson/biastest.pdf)
- Zack Amoveo, [MSRs and Prediction Markets](https://github.com/zack-bitcoin/amoveo-docs/blob/master/basics/msrs_and_prediction_markets.md); Gnosis, [Conditional Tokens](https://web.archive.org/web/20221219190117/https://docs.gnosis.io/conditionaltokens/docs/introduction1/) (the token mechanism)

### from prediction to decision markets

*Once the price drives the choice, a naïve decision rule is manipulable.*

- Hanson, [Decision Markets](https://mason.gmu.edu/~rhanson/decisionmarkets.pdf) — the early formulation of markets that estimate consequences conditional on decisions.
- Othman, Sandholm, [Decision Rules and Decision Markets](https://www.cs.cmu.edu/~sandholm/decision%20rules%20and%20decision%20markets.AAMAS10.pdf)

### making decision markets truthful

*When the report drives the choice, the expert can misreport to steer it. Keeping them honest is a trade-off space, not one recipe.*

- Chen, Kash, [Information Elicitation for Decision Making](https://projects.iq.harvard.edu/sites/projects.iq.harvard.edu/files/yiling/files/decisionrules.pdf) — **randomize**: give the decision rule full support so every action is sometimes taken and scored. You learn every action's effect, but pay an exploration cost (rarer randomization ⇒ rewards scale up inversely).
- Oesterheld, Conitzer, [Decision Scoring Rules](https://users.cs.duke.edu/~conitzer/decisionWINE20.pdf) — **don't randomize**: the principal just follows the recommendation and pays the expert in "shares" of the realized outcome. Truthful with no suboptimal actions — but you only elicit the recommended action's expected utility, not the unchosen counterfactuals.

## counterarguments & attack vectors

Full objections index: [counterarguments](counterarguments.md). The formal manipulation/failure results are in [sota-decision-markets](sota-decision-markets.md).

- Hanson, [Decision Selection Bias](https://www.overcomingbias.com/p/decision-selection-bias)
- Anders_H, [Prediction Markets are Confounded — Implications for the feasibility of Futarchy](https://www.greaterwrong.com/posts/xnC68ZfTkPyzXQS8p/prediction-markets-are-confounded-implications-for-the) (2015, general statement of the confounding problem)
- Distbit, [Correlation vs Causation in Futarchy](https://distbit.xyz/correlation-vs-causation-in-futarchy)
- Oesterheld, [Futarchy Implements Evidential Decision Theory](https://casparoesterheld.com/2017/12/18/futarchy-implements-evidential-decision-theory/)
- Rasmont, [Futarchy is Parasitic on What It Tries to Govern](https://www.lesswrong.com/posts/mW4ypzR6cTwKqncvp/futarchy-is-parasitic-on-what-it-tries-to-govern) (the "Bronze Bull" endogenous-selection argument)
- Distbit, [Futarchy is not secure without a proposal gatekeeper](https://distbit.xyz/malicious-futarchy-proposal-strategies/) — adversarial proposal strategies that exploit conditional execution and market incentives.
- Bolton Bailey, [Futarchy of Mutating Preferences](https://thequantummilkman.substack.com/p/futarchy-of-mutating-preferences)
- Hanson, [Futarchy and the Transfer Problem](https://www.overcomingbias.com/p/futarchy-and-the-transfer-problem)
- [Robin Hanson and "Mencius Moldbug" debate futarchy at Foresight 2010](https://www.youtube.com/watch?v=Tb-6ikXdOzE)

## governance

Applying market signals to real institutions and DAOs.

- Merkle, [DAOs, Democracy and Governance](https://www.ralphmerkle.com/papers/DAOdemocracyDraft.pdf)
- Waggoner, [Governance mixing auctions and futarchy](https://ethresear.ch/t/governance-mixing-auctions-and-futarchy/10772)
- Butter, [Conditional Funding Markets](https://ggresear.ch/t/conditional-funding-markets/27)
- Sztorc, [Fork Futures](https://www.truthcoin.info/blog/fork-futures/)
- [Futarchy Nonprofits](https://docs.google.com/document/d/1cxAWuW1HxJY_bD0gYELpUPzo5-ONCl6r9UHnqjE0_TQ/mobilebasic)
- Buterin, [AI as the engine, humans as the steering wheel](https://vitalik.eth.limo/general/2025/02/28/aihumans.html)
- [Markets in Fact-Checking](https://worksinprogress.co/issue/markets-in-fact-checking/)
- Heavey, [Futarchy as Trustless Joint Ownership](https://www.umbraresearch.xyz/writings/futarchy)
- Greshams Code, [MetaDAO: The Bull Case](https://greshamscode.substack.com/p/metadao-the-bull-case)
- Hanson, [Futarchy Futurism](https://www.overcomingbias.com/p/futarchy-futurism)

## going deeper

- [decision-market SoTA bibliography](sota-decision-markets.md)
- [DM-adjacent information-market mechanisms](sota-dm-adjacent.md)
- [the objection index](counterarguments.md)

## projects

- [Butter](https://butter.markets)
- [MetaDAO](https://metadao.fi)
- [Futarchy.fi](https://futarchy.fi/)
- [Amoveo](https://github.com/zack-bitcoin/amoveo-docs/blob/master/blog_posts/futarchys_failure.md) (discontinued)
- [Gnosis](https://web.archive.org/web/20230323140305/https://docs.gnosis.io/conditionaltokens/) (partially discontinued)
- [Zeitgeist](https://docs.zeitgeist.pm/docs/learn/futarchy)
- [TruthCoin](https://www.truthcoin.info/papers/) (discontinued)
