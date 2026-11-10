# TDR-01 · Life cycle and methodology for the Realtime Quiz project

Status: proposed · 2026-10-19 · to be decided by the sponsor and the PM

## Context
The Realtime Quiz project is built by a team of four students allocating 10 hours per week each over a fixed 14-week duration (560 total hours). The sponsor (Head of IT) requires an approved predictive plan by the end of week 3 and a fully functioning pilot with 50 students in week 14. While the core Must-have features (300 hours) are fixed in the MoSCoW list, high technical uncertainty exists regarding campus proxy behavior with WebSockets and Spring Boot 4 integration. Furthermore, the team is executing their first Scrum project, creating a need to balance predictive governance with agile iterations.

## Options considered
1. **Waterfall (score 2.80):** High governance and fixed planning, but fails on technical uncertainty and late feedback loops.
2. **Pure Scrum (score 3.70):** Strong adaptability and continuous feedback, but lacks formal stage gates demanded by sponsor governance.
3. **Hybrid (score 4.25):** Combines up-front initiation/planning and stage-gate control with 2-week iterative Scrum delivery sprints.

## Decision
We choose **Hybrid (score 4.25)**. The two primary reasons are:
1. **Technical Uncertainty & Early Feedback:** High technical risks (WebSocket proxies, real-time sync) require iterative release and feedback before the week-14 pilot.
2. **Governance Compliance:** The sponsor requires a clear, approved project baseline at week 3 and structured gate control, which pure Scrum does not accommodate.

## Consequences
+ **Positive:** Gives the sponsor predictable milestone checkpoints (G1–G4).
+ **Positive:** Enables early detection and resolution of WebSocket and real-time performance risks in Sprint 1 & 2.
+ **Positive:** Protects the fixed deadline through regular sprint velocity tracking and MoSCoW scope flex.
- **Negative:** Dual overhead of maintaining both project gate documentation and Scrum backlogs.
  - *Mitigation:* Limit gate document updates to lightweight Markdown files managed directly in Git.
- **Negative:** Potential role confusion for a first-time Scrum team balancing PM and PO authority.
  - *Mitigation:* Clearly define PM and PO accountabilities in `scrum-setup.md`.
- **Negative:** Risk of sprint scope creeping into gate baselines.
  - *Mitigation:* Strictly protect the Must-have scope baseline at Gate G1.

## Tailoring

| Keep from predictive | Keep from agile | Drop |
|----------------------|-----------------|------|
| WBS to Level 2 (for scope baseline and Lab-04 setup) | 2-week Sprints with Product Backlog refinement | Heavy formal change control boards for non-Must scope items |
| Phase Gates G1–G4 with formal criteria sign-off | Sprint Planning, Daily Scrums, Reviews, and Retrospectives | Comprehensive up-front UI/UX specification documents |
| Overall project schedule & milestone deadlines | Definition of Ready (DoR) and Definition of Done (DoD) | Detailed task-level gantt tracking past week 3 |

## Phase gates

| Gate | Week / date | Evidence required | Decision maker | Outcomes |
|------|-------------|-------------------|----------------|----------|
| G1 | W3 / 2026-10-19 | Approved charter, scope baseline, WBS, schedule, and initial risk register | Sponsor (Head of IT) & PM | continue / continue with changes / stop / repeat |
| G2 | W7 / 2026-11-16 | Working MVP with core WebSocket real-time quiz execution, passing DoD in CI | Sponsor & PM | continue / continue with changes / stop / repeat |
| G3 | W11 / 2026-12-14 | Release candidate with 100% Must features, line coverage ≥ 80%, load test report | Sponsor & PM | continue / continue with changes / stop / repeat |
| G4 | W14 / 2027-01-04 | Successful pilot run with 50 students, sign-off checklist, final hand-over docs | Sponsor & PM | continue / continue with changes / stop / repeat |