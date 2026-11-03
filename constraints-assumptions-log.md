# Constraints and assumptions log · Realtime Quiz · v0.1 · week 2

| Id   | Type       | Statement (measurable)                                                       | Source / owner                               | Validate by |
|------|------------|------------------------------------------------------------------------------|----------------------------------------------|-------------|
| C-01 | Constraint | Pilot with 50 students runs in week 14 of the 14-week semester               | charter (Milestones), semester calendar      | fixed       |
| C-02 | Constraint | Effort capacity is 4 students x 10 h/week = 40 h/week, 560 h in total        | charter (Resources), ITC course rules        | fixed       |
| C-03 | Constraint | Cash budget is 200 USD (VPS 100, domain 15, tools and reserve 85)            | charter (Budget), Head of IT                 | fixed       |
| C-04 | Constraint | WebSocket broadcast latency is under 500 ms at the pilot                     | case-study brief (NFR table), sponsor        | fixed       |
| C-05 | Constraint | Every release meets WCAG AA and has a green CI pipeline (Definition of Done) | case-study brief (DoD), supervising lecturer | fixed       |
| A-01 | Assumption | The Linode VPS at gicitc.com stays at 25 USD/month for 4 months             | owner: Head of IT                            | W3 -> R-01  |
| A-02 | Assumption | Each of the 4 students delivers 10 h/week in every week up to week 12        | owner: PM (lecturer)                         | W4 -> R-02  |
| A-03 | Assumption | The 50 pilot students use browsers with WebSocket support in week 14         | owner: student representative                | W10 -> R-03 |
| A-04 | Assumption | Pilot quizzes are text-only, agreed with 2 instructors (no media in F13)     | owner: PM (lecturer)                         | W6 -> R-04  |
| A-05 | Assumption | The 17 estimates in features.csv total 504 h with an error of at most 15%    | owner: team lead                             | W7 -> R-05  |

Review at every milestone. Overdue assumption = open issue.
