# Sprint 3 Review – ShiftGrid
**Sprint:** SSB Sprint 3  
**Dates:** June 19 – July 3, 2026  
**Scrum Master:** Amer Nahhas  
**Attendees:** Amer Nahhas (SM), Sara Chen (Dev), James Okafor (Dev), Priya Nair (QA)

---

## Sprint Goal
Fix critical iOS bugs and build the scheduling intelligence layer — conflict detection, availability calendar, and manager alerts.

---

## Sprint Results

**Velocity:** 27 story points committed — 27 delivered — 100% completion

| Ticket | Story | Points | Status |
|--------|-------|--------|--------|
| SSB-11 | Bug: Login page crashes on Safari iOS | 3 | ✅ Done |
| SSB-7 | Bug: Mobile UI misalignment on shift swap screen | 3 | ✅ Done |
| SSB-12 | Manager can view team availability calendar | 5 | ✅ Done |
| SSB-13 | System flags shift conflicts before publishing | 5 | ✅ Done |
| SSB-14 | Employee can set preferred working hours | 3 | ✅ Done |
| SSB-15 | Admin can export shift schedule as PDF | 3 | ✅ Done |
| SSB-16 | Manager receives alert when shift is understaffed | 5 | ✅ Done |
| SSB-17 | Employee can view shift history for last 30 days | 3 | ✅ Done |

---

## Demo Highlights

**SSB-11 — iOS Safari Login Fix**
Critical bug affecting all iOS Safari users resolved in the first days of the sprint. James identified a Content Security Policy header conflict specific to Safari iOS 16+. Fix verified by Priya on iPhone 13 and iPhone SE with no regression.

**SSB-12 + SSB-13 — Availability Calendar & Conflict Detection**
The scheduling intelligence layer is now live. Managers can view real-time team availability and the system automatically flags conflicts before publishing — eliminating accidental double-bookings and hour limit violations. SSB-13 was a critical path dependency on SSB-12 and was completed on schedule.

**SSB-16 — Understaffing Alerts**
Managers now receive in-app and email alerts when a published shift falls below minimum staffing threshold. This closes a major operational gap identified in Sprint 1 planning.

---

## What Went Well
- Critical path executed in order — SSB-12 → SSB-13 → SSB-16 with no blockers
- Both iOS bugs resolved early, freeing QA bandwidth for feature testing
- All 8 stories met Definition of Done criteria before sprint close
- Automation rules caught and flagged SSB-11 immediately on creation

## What Could Improve
- SSB-16 dependency on SSB-13 created a bottleneck mid-sprint — James had idle time waiting for Sara to finish SSB-12
- Mobile testing checklist should be standardized across all stories, not just bug tickets
- PDF export (SSB-15) had scope ambiguity around department filtering — clarified during sprint but should have been caught in grooming

---

## Risks Going Forward
- SSB-7 mobile bug was resolved but similar issues may exist on Android — not yet tested
- Notification service (used in SSB-16) has no redundancy — single point of failure
- Sprint 4 backlog is currently empty — grooming session needed

---

## Next Steps
- Sprint 4 planning session scheduled — backlog grooming required
- Android testing to be added to Definition of Done
- Notification service reliability to be assessed before Sprint 4 kickoff
- Product Owner to review and prioritize remaining feature requests

---

## Overall Assessment
Sprint 3 delivered the most complex sprint to date — 27 points including two bug fixes and four interdependent features on the critical path. The team executed cleanly and the ShiftGrid scheduling intelligence layer is now fully functional.
