# Governance · Realtime Quiz hybrid life cycle

## Stage gates

### G1 · Plan approved · end of week 3 (2026-10-19)
- [ ] Approved project charter and scope baseline (evidence: `lab01/project-charter.md`)
- [ ] WBS completed to level 2 and milestone schedule verified (evidence: `lab03/life-cycle.mmd`)
- [ ] Risk register identifies WebSocket proxy and Spring Boot compatibility risks (evidence: risk log)
- [ ] Resource allocation of 4 students at 10 h/week confirmed (evidence: `scrum-setup.md`)
- [ ] Budget and hosting plan verified (evidence: Linode VPS specification)
- **Inputs:** Charter, scope statement, WBS, schedule, budget in hours
- **Decision maker:** Sponsor (Head of IT) & PM
- **Outcomes:** continue / continue with changes / stop / repeat

### G2 · MVP checkpoint · end of week 7 (2026-11-16)
- [ ] Working MVP with core WebSocket real-time quiz execution functional (evidence: sprint 2 review demo)
- [ ] All Sprint 1 and Sprint 2 backlog items meet the Definition of Done (evidence: sprint review report)
- [ ] Automated unit test line coverage $\ge 80\%$ (evidence: JaCoCo report in CI)
- [ ] Campus proxy WebSocket connectivity tested successfully (evidence: technical test report)
- [ ] Project tracking shows hours used within stage tolerance (evidence: timesheet)
- **Inputs:** Sprint 2 review notes, CI test reports, risk review
- **Decision maker:** Sponsor & PM
- **Outcomes:** continue / continue with changes / stop / repeat

### G3 · Release candidate · end of week 11 (2026-12-14)
- [ ] All Must and at least 80% of Should items meet the DoD (evidence: backlog export)
- [ ] Line coverage $\ge 80\%$ on service and real-time components (evidence: JaCoCo report in CI)
- [ ] Load test with 100 simulated students, p95 broadcast $< 500$ ms (evidence: load test report)
- [ ] Security checklist signed, no secrets hardcoded in repository (evidence: security checklist file)
- [ ] Total hours used $\le 90\%$ of 560 h allocation (evidence: timesheet total)
- **Inputs:** Sprint 4 review notes, CI report, load test report, risk register
- **Decision maker:** Sponsor with the PM
- **Outcomes:** continue / continue with changes / stop / repeat

### G4 · Acceptance and closure · week 14 (2027-01-04)
- [ ] Successful pilot run executed with 50 students (evidence: pilot sign-off sheet)
- [ ] All acceptance criteria for Must features fully met and verified (evidence: user story sign-offs)
- [ ] Hand-over documentation, runbook, and repository transferred (evidence: GitHub repo link)
- [ ] Final budget and timesheet reconciliation completed (evidence: financial summary)
- [ ] Retrospective and lessons learned workshop completed (evidence: retrospective notes)
- **Inputs:** Pilot feedback, final code increment, sign-off checklist
- **Decision maker:** Sponsor & PM
- **Outcomes:** continue / continue with changes / stop / repeat

## Tolerances (manage by exception)

| Tolerance | Stage 1 (W1–3) | Stage 2 (W4–7) | Stage 3 (W8–11) | Stage 4 (W12–14) |
|-----------|----------------|----------------|-----------------|------------------|
| Time | $\pm 3$ days | $\pm 3$ days | $\pm 2$ days | 0 days (fixed pilot date) |
| Cost (hours) | $\pm 10\%$ | $\pm 10\%$ | $\pm 5\%$ | $0\%$ (no overtime in pilot week) |
| Scope | $\pm 5\%$ Must features | $\pm 5\%$ Must features | $0\%$ Must features | $0\%$ scope changes |
| Quality | 0 high-severity bugs | $\le 2$ open minor bugs | 0 high-severity bugs | 0 open bugs |
| Risk | Active mitigation plan | Active mitigation plan | Resolved proxy risks | Deployment risk monitored |

**Escalation path:** Developers $\rightarrow$ Scrum Master $\rightarrow$ Project Manager $\rightarrow$ Sponsor  
**Exception trigger:** Any projected deviation exceeding the stage tolerances above automatically triggers an Exception Report.

## Reporting
- **Weekly Highlight Report:** Submitted by the PM to the sponsor every Friday (length: 1 page), covering four core headings: *Done this week*, *Next week's plan*, *Top risks*, and *Tolerance status*.
- **Sprint Review:** Held at the end of every 2-week sprint as a key checkpoint for the PM and invited stakeholders to inspect working software increments.
- **Exception Report Template:** 
  1. *Deviation:* Description of how time, cost, scope, or quality exceeded stage tolerances.
  2. *Options:* At least two recovery paths (e.g., dropping Should scope vs. reallocating hours).
  3. *Recommendation:* The PM's proposed course of action for sponsor sign-off.

## Closure criteria

| Area | Criterion | Verified by | Owner |
|------|-----------|-------------|-------|
| Acceptance | All 8 Must features verified against acceptance criteria and pilot sign-off | Sponsor sign-off sheet | Product Owner |
| Hand-over | Repository, Linode VPS credentials, deployment runbook, and user manual delivered | Technical verification checklist | Lead Developer |
| Lessons learned | Completed sprint retrospectives and final project post-mortem workshop | Retrospective artifact log | Scrum Master |
| Administrative closure | Final timesheets, artifact archiving, and formal stakeholder sign-off | PM audit report | Project Manager |