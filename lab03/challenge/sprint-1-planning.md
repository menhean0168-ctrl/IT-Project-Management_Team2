# Sprint 1 Planning (Simulated) · 2026-10-20

## Planning Poker Estimation

| Item | A | B | C | D | Agreed | Note |
|------|---|---|---|---|-------:|------|
| B-01 | 3 | 3 | 5 | 2 | 3 | C and D explain: C included full cloud setup while D assumed local docker only. Team agreed on 3 for local docker skeleton + CI. |
| B-02 | 3 | 2 | 3 | 3 | 3 | B estimated low assuming simple forms; agreed on 3 to cover role assignment logic. |
| B-03 | 5 | 8 | 5 | 5 | 5 | B explained high score due to RSA key signing; team agreed on 5 by using standard HS256 JWT tokens. |
| B-04 | 3 | 3 | 3 | 5 | 3 | D estimated high due to UI routing checks; agreed on 3 for backend Spring Security role guards. |
| B-05 | 5 | 5 | 3 | 5 | 5 | C estimated low assuming simple REST endpoints; agreed on 5 to cover DB relations and validation. |
| B-06 | 8 | 13 | 8 | 8 | 8 | B explained 13 due to drag-and-drop UI reordering; team agreed to keep 8 by moving drag-and-drop out of scope and using simple up/down buttons. |
| B-07 | 3 | 2 | 3 | 3 | 3 | B estimated low; agreed on 3 to handle single-answer scoring logic and evaluation. |

**Committed points:** 30 points (~75 h of total 80 h capacity).  
**Sprint Goal:** Establish a working project skeleton with CI pipelines and deliver core user registration, authentication, and basic quiz authoring.

---

## Burndown Analysis

- **First time two full days behind ideal line:** **Day 5** (Ideal remaining was 15 points; actual remaining was 23 points, a gap of 8 points).
- **Velocity achieved:** **25 points** (Items B-01 through B-05 and B-07 met the DoD).
- **Returned to product backlog:** Item **B-06** (8-point item unfinished at Day 10 with 5 points remaining; item returned to backlog for Sprint 2).
- **Forecast for Sprints 2–4:** Total remaining Must + Should backlog is 95 points ($120 - 25 = 95$). At a velocity of 25 points/sprint, the team will need $\frac{95}{25} = 3.8$ sprints. With 3 sprints remaining, the team must drop Should scope via MoSCoW to protect the fixed pilot date.