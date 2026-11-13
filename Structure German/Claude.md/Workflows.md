---
type: procedures
hub: "[[Home]]"
related: ["[[CLAUDE]]", "[[Projects]]"]
---
# Workflows

Rules live in [[CLAUDE]] (same folder). This note holds the step-by-step procedures. Start page: [[Home]].

## 1. Capture (the user)
Drop anything into `Raw/` as a new note, or say "Remember: …". No category, no form. Optional first line: `event: YYYY-MM-DD` if it happened on another day.

## 2. Process inbox
Pending = file in `Raw/` that is non-empty and lacks `status: processed`.
1. Read it. Do not edit the body.
2. Add frontmatter if missing: `captured:` (file date, not today), `event_date:` (only if known or stated), `status:`.
3. Extract: facts, people, events, projects, ideas, decisions, tasks, promises, deadlines, opportunities.
4. Search for existing notes (`People/`, `Future/Projects/`, `Future/Decisions/`, `Schedule/Meetings/`). Update them; create a new note only if none fits.
5. Mark each statement: Fact / Impression / Hypothesis / Suggestion. No invented motives or deadlines.
6. Link both ways: the note gets `Source: [[entry]]`; the entry gets `into: [[note]]`.
7. Suggest next steps as proposals. They become tasks only when chosen.
8. Set `status: processed` and `processed: YYYY-MM-DD`. If something is unfinished use `status: partial` and a `remaining:` line.
9. Reply in a few lines: saved / connections / suggested actions / question if any.

**Rerun safety:** skip `processed`; on `partial` handle only `remaining:`; before adding a link, task or person, check it is not already there.

## 3. Opportunities (when asked, or when one is clear)
For each: related goal ([[Goals]]) · supporting facts (with source) · what is uncertain · one small, cheap test step. Evidence-based, not flattery.

## 4. Morning brief ("Today's brief") — 2 minutes to read
Read the calendar for the day (and the next 2–3 days for deadlines), the day's note, active projects. Write `Schedule/Daily/YYYY-MM-DD.md` using the Daily template: real events, commitments/deadlines, **max 3 proposed outcomes**, suggested next actions, conflicts, decisions needed, **gaps** (what could not be checked).

## 5. Evening review ("Review my day")
Process new Raw entries first. Then fill the evening part of the day note: what happened, what got done, facts/decisions worth saving, new promises, what to reconsider tomorrow. **Do not copy all unfinished tasks forward**; only bring over what the user re-chooses.

## 6. Weekly plan ("Plan my week")
Inputs: calendar, [[Projects]], [[Goals]], confirmed deadlines. Pick 3–5 realistic outcomes. Propose time blocks around fixed events; include task duration, transitions, buffers. If it does not fit, say what to defer. Save in `Schedule/Calendar/YYYY-Www.md` using the Weekly template. **Proposed blocks are not calendar events** until the user approves creating them.

## 7. Weekly review
Results vs. plan; unfinished work; people waiting for a reply or waiting on the user; new opportunities; stale tasks to drop; changes for next week. Only conclusions the records support.

## Practice example (FICTIONAL)
Raw entry: `captured: 2026-10-21` · "Met Alex Example at a career event today (the event was on 2026-10-20). Likes soccer. Said I should look at analyst programs and promised to send my résumé by Friday."

Processing result:
- **Fact:** met Alex Example at a career event on 2026-10-20 (event date ≠ capture date); Alex likes soccer. **Promise (the user's own):** send résumé by Friday — the user stated "Friday" themselves.
- **Notes touched:** a person note for Alex Example in `People/`; [[Goals]] linked (internship).
- **Suggestion (not a task yet):** "Send résumé to Alex — 15 min" → offer to add it to the project's checkboxes.
- **Entry after processing:** `status: processed` · `into: Alex Example`.
- **Rerun:** entry is `processed` → skipped, nothing added twice.

## Connections
Up: [[Home]] · Related: [[CLAUDE]], [[Projects]]
