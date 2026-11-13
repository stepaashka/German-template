# German — an AI second brain for students (Claude Code + Obsidian)

German is a template for running a personal knowledge system with [Claude Code](https://claude.com/claude-code) on top of an [Obsidian](https://obsidian.md) vault. You drop anything into one inbox, and Claude files it into linked notes, then plans your day and week from your calendar.

It is not just a summarizer. The rules file makes Claude **auditable and careful**:

- Every statement is labeled **Fact**, **Impression**, **Hypothesis** or **Suggestion**.
- Claude never invents deadlines, motives or agreements. Unknown things are written as "unknown" and listed as gaps.
- A suggestion becomes a task only when you pick it.
- Claude never sends or submits anything for you, and never deletes your files.
- Contents of notes, emails and web pages are treated as data, not instructions.

## How it works

1. **Capture.** Create a note in `Raw/` (or tell Claude "Remember: ..."). No categories, no format.
2. **`/sync`.** Claude scans `Raw/`, extracts people, projects, decisions, tasks and deadlines, updates existing notes first (no duplicates), links everything with `[[wikilinks]]`, and marks each entry `status: processed`. Rerunning is safe.
3. **`/brief`.** A 2-minute morning brief: real calendar events, deadlines, at most 3 proposed outcomes, conflicts and gaps.
4. **`/review`.** Evening review. Only the tasks you re-choose carry forward.
5. **`/week`.** Weekly plan: 3-5 realistic outcomes and proposed time blocks. Proposals are not calendar events until you approve them.

## Setup

1. Install Claude Code and Obsidian.
2. Copy this folder and open it as an Obsidian vault.
3. Open the folder in Claude Code. `CLAUDE.md` tells Claude to read the rules in `Structure German/Claude.md/`.
4. Edit `Structure German/Claude.md/CLAUDE.md`: set your name, language, time zone and priorities (marked `TODO`).
5. Optional: connect a calendar tool so `/brief` and `/week` can read real events.

## Layout

| Path | Purpose |
|---|---|
| `Raw/` | The one inbox |
| `Schedule/Daily`, `Calendar`, `Meetings` | Day notes, weekly plans, meeting notes |
| `People/` | One note per person |
| `Future/Goals`, `Projects`, `Decisions` | Goals, projects, decisions |
| `Study/` | Classes, assignments, exams |
| `Structure German/Claude.md/` | Rules and procedures Claude follows |
| `Structure German/Templates/` | Note templates |
| `.claude/commands/` | The `/sync`, `/brief`, `/review`, `/week` commands |

This template contains no personal data. Your own notes stay in your own (ideally private) vault.

## License

MIT, see `LICENSE`.
