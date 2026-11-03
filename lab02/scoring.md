# Weighted scoring · build vs buy vs hybrid

## Weights (agreed 2026-11-03, before scoring)
- Learning value: 40 — this is a Software Engineering capstone, so building and learning is the main goal.
- Cost: 25 — the cash budget is fixed at 200 USD (C-03) and nobody can approve an overspend.
- Time: 20 — the week-14 pilot with 50 students is the fixed date (C-01), so slipping isn't an option.
- Fit: 15 — the 47 requirements matter, but Should and Could items can be dropped, so fit is the most flexible.
Sum = 100

## Options
- **Build:** the team builds the full Realtime Quiz platform as planned (504 h of work), hosted on the Linode VPS at 25 USD/month x 4 = 100 USD.
- **Buy:** Kahoot!+ Bronze, up to 50 players per session, 7.99 USD/month billed monthly x 4 months = 31.96 USD. No custom code, so no real engineering for the capstone.
- **Hybrid:** buy Kahoot!+ Bronze for the live-session engine (31.96 USD), build only authoring, analytics and export on the VPS (about 100 USD).

## Scores and evidence
| Criterion | Weight | Build | Buy | Hybrid |
|-----------|--------|-------|-----|--------|
| Learning value for the capstone | 40 | 5 | 1 | 3 |
| Cost within the 200 USD cash budget | 25 | 4 | 5 | 3 |
| Time to the week-14 pilot | 20 | 3 | 5 | 4 |
| Fit to the 47 functional requirements | 15 | 5 | 2 | 4 |

Evidence (one line per score):
- Build, learning 5: the team designs and codes every part, which is the point of the capstone.
- Build, cost 4: VPS 100 USD + domain 15 USD = 115 USD, 57.5 % of the 200 USD budget.
- Build, time 3: 504 h of work against 560 h capacity, Must share 59.5 %, so the margin is thin.
- Build, fit 5: we control the code, so all 47 requirements are possible.
- Buy, learning 1: only quiz content is configured, no engineering.
- Buy, cost 5: 31.96 USD (4 x 7.99), 16 % of the budget.
- Buy, time 5: the tool works from day one, so the pilot date is safe.
- Buy, fit 2: Kahoot is closed, so custom roles (FR-A1..A4) and reporting are limited, and the 50-player cap leaves no headroom for the 50-student pilot.
- Hybrid, learning 3: authoring, analytics and export are still built by the team.
- Hybrid, cost 3: VPS 100 + domain 15 + Kahoot 31.96 = 146.96 USD, 73 % of the budget.
- Hybrid, time 4: the live engine is bought, so the hardest real-time work (F02, F05, F08) is skipped.
- Hybrid, fit 4: most requirements are covered, but the live-session ones depend on Kahoot.

Weighted score = sum of weight x score:
- Build  = 40*5 + 25*4 + 20*3 + 15*5 = 200 + 100 + 60 + 75 = 435 (87 % of 500)
- Buy    = 40*1 + 25*5 + 20*5 + 15*2 = 40 + 125 + 100 + 30 = 295 (59 % of 500)
- Hybrid = 40*3 + 25*3 + 20*4 + 15*4 = 120 + 75 + 80 + 60 = 335 (67 % of 500)

## Sensitivity
Moved 10 points of weight from the heaviest criterion (learning, 40 to 30) to the lightest (fit, 15 to 25). Cost 25 and time 20 unchanged, sum = 100.

- Build  = 30*5 + 25*4 + 20*3 + 25*5 = 150 + 100 + 60 + 125 = 435
- Buy    = 30*1 + 25*5 + 20*5 + 25*2 = 30 + 125 + 100 + 50 = 305
- Hybrid = 30*3 + 25*3 + 20*4 + 25*4 = 90 + 75 + 80 + 100 = 345

Winner changes? No. Build stays first (435 vs 345 vs 305), so the recommendation is robust to this weight shift. Build keeps its lead because it scores 4 or 5 on three of the four criteria.
