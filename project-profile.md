# Project profile · Realtime Quiz

Sources: [Lab-03 Setup recap table](README.md) (the charter, `lab01/project-charter.md`, is not in this repository, so the recap table stands in for it) · [MoSCoW list](../lab02/moscow.md) · [constraint analysis](../lab02/constraints.md)

| # | Criterion | Evidence (one fact) | Weight | Score 1-5 | W x S |
|---|-----------|---------------------|-------:|----------:|------:|
| 1 | Requirements stability | 8 Must features (300 h, 59.5 % of 504 h) are fixed in the MoSCoW list; screens and real-time behaviour are not specified (moscow.md) | 25 | 3 | 75 |
| 2 | Technical uncertainty | The campus proxy may block WebSocket, Spring Boot 4 examples are outdated, and late answers can cause race conditions | 20 | 4 | 80 |
| 3 | Team experience with agile | First Scrum project; Java and Spring are learned in the parallel Software Engineering course | 15 | 2 | 30 |
| 4 | Contract and governance constraints | The sponsor requires an approved plan by week 3 and a pilot with 50 students in week 14; internal project, no contract | 20 | 2 | 40 |
| 5 | Need for early delivery and feedback | Real-time behaviour must be felt by users before the pilot; 204 h of Should and Could scope can still change after early feedback (moscow.md, constraints.md) | 20 | 4 | 80 |
|   | **Profile** = SUM(W x S) / 100 | | 100 | | **3.05** |
| 6 | (optional, not in the total) Sponsor availability | The Head of IT has other duties; a review every two weeks is not yet confirmed (assumption to validate at G1) | - | 3 | - |

Score 1-5: 1 = the fact favours predictive, 5 = it favours adaptive.

Calculation: 75 + 80 + 30 + 40 + 80 = 305; 305 / 100 = 3.05.

Interpretation: < 2.5 predictive · 2.5-3.5 hybrid · > 3.5 agile. **3.05 falls in the hybrid band.**

## Profile summary
Realtime Quiz is a fixed-date, fixed-budget project with a fixed Must list but unspecified screens and real-time behaviour, built by a first-time Scrum team. The two criteria that pull hardest towards an adaptive approach are technical uncertainty and the need for early feedback (80 points each), while the sponsor's week-3 plan approval and the team's missing agile experience pull back towards a predictive plan (40 and 30 points). Task 2 must therefore compare waterfall, pure Scrum and a hybrid of the two as candidates.
