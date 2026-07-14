# agents guide — learn-futarchy

This repo is a curated *learn futarchy* resource: a guided reading path (`README.md`) plus companion indexes. If you are an agent adding entries, follow these rules.

## the rule that matters: "why this entry?"

Every entry you add should answer **"why this entry?"** — a short, one-line description after an em-dash, saying what the reader gets from it or why it belongs.

Skip the description *only* when the entry is either:
- **canonical / well-known** — a work the field cites by name (e.g. Hanson's futarchy paper, Othman–Sandholm), or
- **self-explanatory from its title** — the title already says what it is.

When in doubt, write the line. A bare link with no reason is the thing to avoid.

Format:
```
- Author (year), *Title* — why this entry (what the reader gets).
```

## put it in the right page and section

Match the entry to the file and section; do not dump everything into the README.

- **`README.md`** — the hand-curated shortlist and guided reading path (start here → what is futarchy → the market engine → from prediction to decision → making decision markets truthful → counterarguments & attack vectors → governance → projects). High-signal only; long lists do not go here.
- **`counterarguments.md`** — the objection index: tables grouped by family (identification, manipulation, objective governance, institutional, liquidity, mechanism-design, epistemic). Add a row in the right family.
- **`sota-decision-markets.md`** — the decision-market long-list (completeness): foundations, SoTA solutions, manipulation (theory & evidence), governance.
- **`sota-dm-adjacent.md`** — information-market / elicitation mechanisms adjacent to decision markets.

New canonical or completeness material goes in the SoTA files. Only promote something into the README shortlist if it genuinely belongs on a first reading path.

## house style

- Headings lowercase; normal casing for prose and work titles.
- Verify citations — real authors, years, venues; never invent a citation or URL. If you cannot confirm one, say so rather than guess.
- Public repo — no local paths, private notes, or unpublished internal material.
- Keep descriptions factual and short.
