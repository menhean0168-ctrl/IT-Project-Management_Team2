# DR-01 · Open-day demo scope, week 10
Status: approved 2026-11-03 · Requested by: Head of IT

## Context
At the end of week 4 the Head of IT asked for every Should feature to be demonstrable at the open day in week 10, with the week-14 pilot unchanged. Fixed facts:
- C-01 pilot with 50 students in week 14
- C-02 team 4 x 10 h/week, capacity W5-W10 = 240 h
- C-03 cash budget 200 USD

Remaining Must work is 152 h (300 h minus 148 h done) and Should work is 86 h, so 238 h are needed against 240 h. Only 2 h are spare, or a 54 h shortfall if the 56 h contingency is kept.

## Options considered
| Option | Time | Cost | Quality at the open day |
|--------|------|------|-------------------------|
| 0 All Should by W10 (the request) | 0 weeks | 0 USD, but all 56 h contingency used | Full Should scope, no buffer for the W14 pilot |
| 1 Must + F09 (20 h) + F10 (30 h) by W10 = 202 h | 0 weeks | 0 USD, 38 h buffer kept | Real responsive design and analytics; F11, F12 follow at W14 |
| 2 Demo build with mocked analytics (8 h) = 180 h | 0 weeks | 0 USD, 60 h buffer kept | Sample data only; F10 and the rest follow at W14 |

## Decision
Option 1. F09 and F10 move to the W10 demo milestone. F11 and F12 stay at the W14 pilot. No Could work starts before W11.

## Consequences
- New milestone "Open day demo" in W10 in the schedule baseline, updated by W5.
- New Won't for W10 (deferred to W14): F11 Export (24 h) and F12 Notifications (12 h).
- Could items F13 to F16 stay unscheduled until W11; F17 stays Won't.
- Risk R-07 added: demo on unfinished analytics (F10, 30 h) in W10.
- Buffer before W14 is 38 h, down from 56 h.

## Approvers
- Head of IT (sponsor)
- Supervising lecturer (PM)
