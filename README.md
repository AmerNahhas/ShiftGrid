# ShiftGrid – Workforce Scheduling App

A simulated Agile/Scrum project managing the end-to-end development of a workforce scheduling application for shift-based teams.

## Project Overview

ShiftGrid is a B2B SaaS tool designed to help operations managers build and publish shift schedules, allow employees to manage their availability, and give admins payroll reporting visibility — all in one platform.

This repository documents the full Scrum lifecycle of the project including backlog grooming, sprint planning, execution, and retrospectives.

---

## Role

**Amer Nahhas — Scrum Master / Project Manager**

Responsibilities:
- Facilitated sprint planning, daily standups, and retrospectives
- Maintained and prioritized the product backlog
- Removed blockers and coordinated cross-functional team communication
- Tracked sprint velocity and ensured delivery against sprint goals

---

## Team

| Name | Role |
|------|------|
| Amer Nahhas | Scrum Master / PM |
| Sara Chen | Frontend Developer |
| James Okafor | Backend Developer |
| Priya Nair | QA Engineer |

---

## Tools Used

- **Jira** — Scrum board, backlog, sprint management
- **GitHub** — Project documentation
- **Agile/Scrum** — 2-week sprints, user stories, story points

---

## Sprint Summary

### Sprint 1 — May 22 to June 5, 2026
**Goal:** Enable employees and managers to view, create, and swap shift schedules through the app

| Ticket | Story | Points | Status |
|--------|-------|--------|--------|
| SSB-1 | User can view their weekly shift schedule | 3 | ✅ Done |
| SSB-2 | Manager can create and publish weekly schedules | 5 | ✅ Done |
| SSB-3 | Employee can request a shift swap with a coworker | 5 | ✅ Done |

**Velocity:** 13 points delivered — 100% completion

---

### Sprint 2 — June 5 to June 19, 2026
**Goal:** Enable managers to enforce hour limits, allow employees to request time off, and provide admins with payroll reporting

| Ticket | Story | Points | Status |
|--------|-------|--------|--------|
| SSB-4 | Manager can set maximum hours per employee per week | 3 | ✅ Done |
| SSB-5 | Employee can submit time-off requests through the app | 3 | ✅ Done |
| SSB-6 | Admin can generate a payroll hours report | 5 | ✅ Done |
| SSB-7 | Bug: Mobile UI misalignment on shift swap confirmation screen | — | 🔄 Carried over |

**Velocity:** 11 points delivered — 100% of planned stories complete

---

## Sprint 1 Retrospective

**What went well:**
- All 3 Sprint 1 stories delivered on time with no scope changes
- QA caught a mobile UI bug early (SSB-7) before it reached production
- Clear acceptance criteria prevented back-and-forth during review

**What to improve:**
- Notification service dependency was identified late in Sprint 1 — should be flagged during backlog grooming
- Mobile testing should be added to the Definition of Done from Sprint 1

**Action items for Sprint 2:**
- Add mobile testing checklist to QA process
- Flag external dependencies during sprint planning, not mid-sprint

---

## Backlog

Full product backlog and ticket history available in the Jira project.


## Automation Rules

Three automation flows built in Jira to reduce manual work and enforce team process:

| Rule | Trigger | Condition | Action |
|------|---------|-----------|--------|
| Auto-assign new issues to SM | Work item created | issuetype in (Story, Bug) | Assign to Scrum Master |
| In Progress notification comment | Work item transitioned to In Progress | None | Add comment reminding assignee to update daily |
| Auto-set High priority on Bug creation | Work item created | issuetype = Bug | Set priority to High |
---

## Key Takeaways

- Managed a 2-sprint Scrum cycle delivering 24 story points across 6 user stories
- Facilitated cross-functional coordination across dev, QA, and product roles
- Applied real-world Scrum ceremonies: sprint planning, standups, retrospectives
- Tracked and resolved a production bug through proper Agile workflow
