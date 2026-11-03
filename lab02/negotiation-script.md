# Negotiation · sponsor asks for all Should features by week 10

## Data sheet (week 4)
| Measure                                  | Value                          |
|------------------------------------------|--------------------------------|
| Capacity W5-W10                          | 6 x 40 = 240 h                 |
| Must remaining (300 done 148)            | 152 h                          |
| Should total (Task 2 rating)             | 86 h (F09 20, F10 30, F11 24, F12 12) |
| Needed by W10 = Must remaining + Should  | 152 + 86 = 238 h               |
| Surplus by W10, contingency used         | 240 - 238 = 2 h, buffer 0 h    |
| Shortfall by W10, 56 h contingency kept  | 238 - (240 - 56) = 54 h = 1.35 weeks |
| Velocity, sprints 1-2 (points done)      | 18, 21 -> 19.5 avg             |

"Everything by week 10" fits only by spending the whole 56 h contingency. Any slip then breaks the week-14 pilot (C-01).

## Script
**Sponsor:** I need every Should feature demonstrable at the open day in week 10. It is mostly small stuff.
**PM:** I want the open day to succeed. The four Should features total 86 h, an average of 21.5 h each, over two weeks of team capacity. Together with the 152 h of Must work left, we need 238 h against 240 h of capacity.
**Sponsor:** So it fits. It is a small change.
**PM:** It fits only with 2 h to spare. That uses all 56 h of contingency, and the pilot in week 14 has no buffer left for a failed build or a sick teammate.
**Sponsor:** Then the team can work a bit harder.
**PM:** To keep the 56 h buffer we would need 54 more hours in 6 weeks. That is 9 h/week, 22.5 % above our 40 h/week. Our velocity is 19.5 points a sprint and it has not been higher than 21.
**Sponsor:** Other teams manage this without problems.
**PM:** I cannot compare with them. Our fixed facts are 4 students x 10 h/week and a 200 USD cash budget. Buying the 54 h from a TA at 12 USD/h costs 648 USD, 3.2 times the whole budget.
**Sponsor:** Fine, let's decide later, once we see how the sprints go.
**PM:** Waiting costs capacity. If we decide at week 6, only W7-W10 remain: 4 x 40 = 160 h against 238 h needed, a shortfall of 78 h.
**Sponsor:** So what can I tell the department for the open day?
**PM:** Here are two ways to give you a strong open day. Option 1: Must complete + Responsive (F09, 20 h) + Analytics (F10, 30 h) by W10 = 152 + 50 = 202 h, 38 h buffer kept. It displaces Export (F11, 24 h) and Notifications (F12, 12 h) to the W14 pilot. Option 2: a demo build with mocked analytics (8 h) at W10, so 152 + 20 + 8 = 180 h, 60 h buffer. It displaces real analytics (F10, 30 h) to W14, and the demo shows sample data, not live data.
**Sponsor:** Which one shows more of the product?
**PM:** Option 1 shows real responsive design and real analytics. Option 2 keeps the larger buffer: 60 h against 38 h.
**Sponsor:** I choose option 1. Real analytics matters more for the department.
**PM:** I will record this as DR-01 today and update the baseline by W5. F11, F12 stay at the W14 pilot and no Could work starts before W11.
