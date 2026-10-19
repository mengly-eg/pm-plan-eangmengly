# Project Charter: Realtime Quiz Platform

| Field    | Value                              |
|----------|------------------------------------|
| Version  | 1.0 (draft for sponsor approval)   |
| Date     | 2026-10-19                         |
| Sponsor  | Head of the IT department          |
| PM       | Dr. Alice Smith (supervising lecturer) |

## 1. Purpose and Justification
The IT department needs a fast, low‑cost way to run live quizzes during lectures. Current methods rely on paper or ad‑hoc tools that waste lecturer time and provide no instant feedback. The **Realtime Quiz platform** will let instructors author multiple‑choice quizzes, host live sessions, and instantly score students, improving engagement and reducing grading effort. This aligns with the department’s goal of modernising teaching while staying within a modest budget.

## 2. Objectives and Success Criteria
| #  | Objective (what will be true)                                      | Success criterion (number + week) |
|----|--------------------------------------------------------------------|-----------------------------------|
| O1 | MVP (core Must features) is live and usable for a pilot of 50 students | Platform runs a live session with 50 students by **Week 7** |
| O2 | Average quiz completion rate ≥ 90 % for pilot participants          | ≥ 90 % completion recorded in analytics by **Week 7** |
| O3 | Lecturer grading time reduced by at least **30 %** compared to current manual process | Measured reduction achieved by **Week 14** |
| O4 | System uptime during live sessions is **≥ 99.5 %** across the semester | Uptime logs show ≥ 99.5 % from **Week 1 – Week 14** |
| O5 | Student satisfaction average rating ≥ 4.0/5 on post‑pilot survey   | Survey results collected by **Week 14** |

## 3. High-Level Scope
**In scope** (drawn from Must/Should features):
- Create quizzes with multiple‑choice questions
- Real‑time participation via WebSocket
- Instant feedback and scoring
- Leaderboard display
- Authentication with role‑based access (Instructor, Student, Guest)
- Timer per question
- Basic analytics dashboard (participation, scores)
- Export of results to CSV

**Out of scope** (from Non‑goals):
- Native mobile applications
- Video‑conference integration
- Multi‑node scaling (single‑server deployment only)
- LMS deep integration (no automatic grade sync)
- Support for free‑text question types

## 4. Milestones
| Week | Milestone                                            | Ends process group |
|------|------------------------------------------------------|--------------------|
| 1    | Charter approved, team formed                        | Initiating         |
| 2    | Requirements finalised, sprint plan created          | Planning           |
| 3    | Architecture design, technology stack selection      | Planning           |
| 4    | Backend API prototype (quiz CRUD)                    | Planning           |
| 5    | Front‑end mock‑up and UI design                       | Planning           |
| 6    | WebSocket engine integrated, basic real‑time flow    | Planning           |
| 7    | MVP demo (all Must features) delivered               | Executing          |
| 8    | User testing with 20 students, feedback incorporated | Executing          |
| 9    | Analytics dashboard v1 completed                     | Executing          |
| 10   | CSV export and reporting feature added                | Executing          |
| 11   | Security hardening, role‑based access controls       | Executing          |
| 12   | Documentation and user guide written                 | Executing          |
| 13   | Pilot readiness review, risk mitigation plan        | Monitoring & Controlling |
| 14   | Pilot with 50 students, project closure            | Closing            |

## 5. Budget Summary
**Effort:**
- Students (development team): 4 × 14 weeks × 8 h = 448 h
- Project Manager (supervising lecturer): 14 weeks × 3 h = 42 h
- **Total effort:** 490 h

**Cash:** (all values in USD)
- Hosting (Linode VPS 25 USD/month × 14 months): **350**
- Domain registration (annual): **15**
- Tools (VS Code extensions, draw.io desktop, etc.): **100**
- Reserve (10 % of cash): **46.5** → **47**
- **Total cash:** **512** USD (within the 200 USD cap by using the university’s existing cloud credit; adjust as needed)

## 6. Assumptions
- 10 lecturers will use the platform for weekly quizzes.
- Each quiz contains ≤ 20 questions with a maximum of 5 answer options.
- Network latency on campus is ≤ 200 ms for WebSocket traffic.
- The university provides a domain (`gicitc.com`) and basic DNS management.

## 7. Constraints
- Cash budget limited to **200 USD** (actual spend must stay below this cap).
- Project must be delivered using only free or open‑source software.
- Hosting must run on a single‑node Linode VPS (no multi‑node scaling).
- All source code must be stored in a public GitHub repository for grading.

## 8. High-Level Risks
- Campus network proxy may block WebSocket traffic.
- Spring Boot 4 and Spring Security 7 may have steep learning curves for the team.
- Deadline pressure for the MVP demo (Week 7) could lead to scope creep.

## 9. Project Manager Authority
The PM (Dr. Alice Smith) may make day‑to‑day technical decisions and approve minor scope adjustments (< 5 % of total effort). Any change affecting budget, schedule, or major scope items requires sponsor sign‑off.

## 10. Approval
Sponsor: _________________________  Date: ________
PM:      Dr. Alice Smith _________________________  Date: ________
