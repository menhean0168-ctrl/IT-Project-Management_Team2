# Scrum setup · Realtime Quiz

## Roles

| Role | Person | Accountable for | Not responsible for |
|------|--------|-----------------|---------------------|
| Product owner | Student A | Managing and prioritizing the product backlog, defining acceptance criteria, and accepting user stories | Writing code architecture or managing team sprint capacity |
| Scrum master | Student B | Facilitating Scrum events, removing impediments, and protecting the team from external distractions | Assigning tasks to developers or dictating technical solutions |
| Developers | Students A–D | Building increments of software that meet the Definition of Done (DoD) | Changing sprint goals or modifying project scope unilaterally |
| Project manager | Lecturer | Overall governance, stage gates G1–G4, budget, and stakeholder reporting | Daily Scrum facilitation or sprint backlog creation |
| Sponsor | Head of IT | Approving the project plan at G1 and evaluating milestones at G2–G4 | Day-to-day sprint execution or task allocation |

*Note on PO dual-role:* Student A acts as both a Developer and the Product Owner, which can create a conflict of interest. To mitigate this, backlog refinement sessions are kept transparent, and priority decisions rely strictly on the MoSCoW list and sponsor requirements.

## Sprint goal (sprint 1, weeks 4–5)
Establish a working project skeleton with CI pipelines and deliver core user registration and authentication so that users can sign up and log in securely.

## Event calendar · sprint 1 (2026-10-20 to 2026-11-02)

| Event | Date(s) | Time | Timebox | Attendees | Output |
|-------|---------|------|---------|-----------|--------|
| Sprint planning | Tue 2026-10-20 | 10:00 | 2 h | PO, SM, Devs | Sprint goal, sprint 1 backlog |
| Daily scrum | Mon–Fri (10-21 to 11-02) | 09:00 | 15 min | Devs (+SM) | Updated daily plan and blockers |
| Backlog refinement | Thu 2026-10-29 | 14:00 | 1 h | PO, Devs | Refined user stories for Sprint 2 |
| Sprint review | Mon 2026-11-02 | 14:00 | 1 h | Team, PM, Sponsor | Stakeholder feedback, working increment |
| Sprint retrospective | Mon 2026-11-02 | 15:15 | 45 min | Team | Process improvements & action items |

## Definition of ready
1. The user story has a clear identifier (FR id from MoSCoW) and maps to a specific feature.
2. Acceptance criteria are fully written using Given/When/Then format.
3. Story points are estimated using Fibonacci numbers (1, 2, 3, 5, 8).
4. External technical dependencies and blockers are identified and resolved.
5. A UI wireframe or API contract sketch is attached if applicable.

## Definition of done
1. Code compiles successfully without errors or warnings.
2. Automated unit and integration tests pass successfully in the local workspace.
3. Line coverage of new service code $\ge 80\%$ in the JaCoCo report (verified by CI).
4. Static code analysis and security checks run cleanly with no high-severity vulnerabilities.
5. The feature is successfully merged into the `lab-03` branch via a pull request review.
6. Code adheres to the project's formatting and style guidelines.
7. Demonstrated and tested on a desktop and a mobile-sized viewport.
8. Relevant documentation or API endpoints are updated.

Planning velocity: **30 points** · Capacity: 4 students $\times$ 10 h/week $\times$ 2 weeks = 80 hours.