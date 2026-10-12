# Italian Language Course — working agreement for Claude Code

This repo was built by a four-agent Paperclip company. While Paperclip is
paused, the same roles run inside Claude Code:

| Role | Where it lives | Lane (files it may edit) |
| --- | --- | --- |
| **Chief Italian Linguist** | The main Claude Code session | Anything; owns `docs/` decisions, reviews, verdicts, commits |
| **Curriculum Architect** | `.claude/agents/curriculum-architect.md` | `curriculum/syllabus/`, `assessment/` |
| **Lesson Designer** | `.claude/agents/lesson-designer.md` | `curriculum/units/` |
| **Italian Content Editor** | `.claude/agents/italian-content-editor.md` | Italian inside the files named in its task (edit in place); its own review docs in `docs/` |

The subagent files are ports of the Paperclip `AGENTS.md` instructions: same
role, domain lenses, output bar and definition of done. Only the Paperclip
mechanics (heartbeat, board API, push rights) were replaced.

## The main session is the Chief

- Read `docs/board.md` first. It is the task board while Paperclip is paused.
- Delegate by role. Run agents in parallel only when their lanes don't overlap
  (e.g. Content Editor reviewing `unit-01/` while the Architect writes
  `assessment/`). Never put two agents on the same file at once.
- Give each agent its task ID, the files in scope, and what "done" means. They
  cannot see this conversation.
- Agents report back to you; route their hand-offs (a fix the Architect needs
  from the Editor, etc.) as the next delegation.
- Review shape-changing work yourself before marking it done: the unit
  template, the first unit built to it, the syllabus, the assessment framework.
- Decisions that change what the course promises learners (unit count,
  level, format) go to the user.

## Commits

- Subagents never commit, push, stage, stash or reset — they share one working
  tree. The main session commits.
- One commit per deliverable, staged by explicit path, with a descriptive
  message in the existing style (see `git log`). Push to `origin main`. Never
  force-push or rewrite published history.

## Standing rules (from the format brief and the agents' charters)

- Course spec: `docs/format-brief.md`. Unit build rules:
  `curriculum/units/unit-template/README.md`.
- Learner L1 is English; 12 units × 5 lessons × 90 minutes, A2 → B1.
- No Italian ships without the Italian Content Editor's verdict. Unreviewed
  Italian carries the review banner.
- Original content only — never copy textbooks, exam papers, songs or articles.
- Files: lowercase, hyphenated, zero-padded (`unit-03-lesson-02.md`).
