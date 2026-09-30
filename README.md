# Italian Language Course — A2 → B1

A complete, teachable Italian curriculum that takes a learner from elementary
(CEFR A2) to solid intermediate (CEFR B1).

**Shape of the course:** 12 themed units × 5 lessons = 60 lessons of ~90 minutes
(~90 guided hours plus self-study). Units are theme-led; grammar is spiralled
underneath the themes, each structure introduced, recycled in a new theme, then
used in free production. Milestone assessments follow CELI/CILS B1 task types so
the course ends somewhere externally recognisable.

## Repository layout

| Path                   | Contents                                                            |
| ---------------------- | ------------------------------------------------------------------- |
| `docs/`                | Decisions that frame the curriculum — format brief, style guide.     |
| `curriculum/syllabus/` | The 12-unit grid: themes, can-do goals, grammar, lexis, recycling.   |
| `curriculum/units/`    | Unit template and the built units (`unit-01/`, `unit-02/`, …).       |
| `assessment/`          | Placement check, unit checkpoint template, milestone assessments.    |

## Conventions

- **Markdown for everything.** Plain `.md` files, one deliverable per file, so
  the whole course is diffable and reviewable in pull requests.
- **Italian is content, not decoration.** Every Italian line in this repo is
  written or reviewed to native standard and deliberately level-graded. Flat
  textbook Italian that no one would actually say does not ship.
- **CEFR references are explicit.** Can-do statements name their level so
  progression can be checked rather than assumed.
- **File naming:** lowercase, hyphenated, zero-padded (`unit-03-lesson-02.md`).

## Status

Early. The syllabus map, unit template, first sample unit, and assessment
framework are in progress. See the Paperclip board for current tasks.
