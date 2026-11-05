# Approach comparison · Realtime Quiz

Sources: [project profile](project-profile.md) (profile 3.05, hybrid band) · [approach-scoring.csv](approach-scoring.csv) · [MoSCoW list](../lab02/moscow.md)

| Approach | Requirements | Sponsor control | First quiz | Two main risks | Fit |
|----------|--------------|-----------------|-----------:|----------------|-----|
| Waterfall | All 47 functional requirements frozen at G1 (week 3) and changed only through change control; screens are guessed before anyone sees them | Phase-end sign-offs against a baseline; the sponsor sees nothing playable before integration | week 12 | 1. The WebSocket and proxy problem is found only at integration in weeks 11-12. 2. UI and real-time behaviour are guessed up front and corrections come too late. | Low (2.80): strong on governance, weak on uncertainty and early feedback (the criteria with weight 20 each). |
| Pure Scrum | Product backlog reordered every sprint; no baseline and no plan approval | A sprint review every 2 weeks, but no gate to stop or re-plan; budget tracked only by velocity | week 5 | 1. A first-time team drifts without a plan. 2. The fixed week-14 pilot date is not protected by any gate. | Medium-high (3.70): strong on feedback and uncertainty, weak on governance (weight 20) and team experience (weight 15). |
| Hybrid | The Must scope (8 items, 300 h) is baselined at G1; item details are refined per sprint; Should and Could flex by MoSCoW | Four gates G1-G4 (plan by week 3, MVP in week 7, release candidate in week 11, acceptance in week 14) plus a sprint review every 2 weeks | week 7 | 1. Gate documents become overhead that takes hours from a 40 h/week team. 2. Two rule sets (plan and backlog) confuse a first-time team and the PO and PM clash over scope. | High (4.25): keeps the plan the sponsor demands and the feedback loop the uncertainty needs. |

Columns: how requirements are handled · how the sponsor controls the project (governance) · week in which the sponsor first plays a working quiz · two main risks · fit with the Task 1 profile

First-quiz weeks assume the Lab-02 recap schedule: waterfall integrates in weeks 11-12; pure Scrum starts sprints in week 2 (sprint 2 review at the end of week 5); the hybrid plans in weeks 2-3, sprint 1 is weeks 4-5 and the MVP checkpoint G2 falls at the end of week 7.

## Weighted score (from approach-scoring.csv)
Weights 25 / 20 / 15 / 20 / 20 (from Task 1). Score = SUMPRODUCT(weights, fit) / 100.

| Approach | Calculation | Score |
|----------|-------------|------:|
| Waterfall | 25×3 + 20×2 + 15×3 + 20×5 + 20×1 = 75 + 40 + 45 + 100 + 20 = 280 | 2.80 |
| Pure Scrum | 25×4 + 20×5 + 15×2 + 20×2 + 20×5 = 100 + 100 + 30 + 40 + 100 = 370 | 3.70 |
| Hybrid | 25×5 + 20×4 + 15×4 + 20×4 + 20×4 = 125 + 80 + 60 + 80 + 80 = 425 | 4.25 |

Waterfall 2.80 · Scrum 3.70 · Hybrid 4.25

## Sensitivity
- Test 1: requirements stability (hardest to judge, because screens are unspecified) 25 → 35 and governance 20 → 10: Waterfall 2.60, Scrum 3.90, Hybrid 4.35. Hybrid is still first and Scrum closes to within 0.45.
- Test 2: team experience 15 → 25 and technical uncertainty 20 → 10: Waterfall 2.90, Scrum 3.40, Hybrid 4.25. Hybrid is still first and its lead over Scrum grows to 0.85.
- Stress test: governance 20 → 5 and early delivery 20 → 35 (a sponsor who does not care about gates and wants fast feedback): Waterfall 2.20, Scrum 4.15, Hybrid 4.25. Hybrid is still first, but the gap shrinks to 0.10.

The ranking never changes in these tests; only the stress test brings Scrum within 0.10.

## Recommendation
**Hybrid (4.25).** The runner-up is pure Scrum (3.70). I would choose Scrum instead only if the sponsor drops the week-3 plan approval and attends every sprint review, because then the gates buy no control and cost team hours.
