# Task board

The in-repo stand-in for the Paperclip board while Paperclip is paused. The
Chief Italian Linguist (the main Claude Code session) is the only editor:
agents end each report with a `Board:` block and the Chief copies it in. When Paperclip resumes,
reconcile this file back onto the Paperclip board, then stop editing it there or
here — one board at a time.

Statuses: `todo` · `in progress` · `blocked` · `in review` · `done`.
New tasks continue the Paperclip numbering from **ITA-13**.

| ID | Title | Owner | Status | Blocked by | Next action |
| --- | --- | --- | --- | --- | --- |
| ITA-1 | Confirm learner L1 (format brief open question) | Chief | done | — | — |
| ITA-2 | Format brief | Chief | done | — | — |
| ITA-3 | 12-unit syllabus map + grammar and lexis progressions | Curriculum Architect | done | — | Accepted in `docs/syllabus-shape-review.md` (ITA-7). |
| ITA-4 | Assessment framework | Curriculum Architect | in progress | — | Write `assessment/milestone-1.md` and `assessment/milestone-2.md`; placement check, checkpoint template and rubrics exist (uncommitted when Paperclip paused). Then → Chief for review. |
| ITA-5 | Unit template + sample Unit 1 | Lesson Designer | done | — | Accepted with three conditions: `docs/unit-template-format-verdict.md`. Conditions are carried by ITA-12. |
| ITA-6 | Vet the Italian in the three syllabus documents | Italian Content Editor | done | — | Pass with edits at `3961be5`. |
| ITA-7 | Syllabus shape review | Chief | done | — | `docs/syllabus-shape-review.md`. |
| ITA-8 | Apply shape-review defects 1–3 + the `Lei`-imperative strand | Curriculum Architect | in progress | — | Seed 4 drafted in `grammar-progression.md` (uncommitted). Remaining: confirm defects 1–3 are applied; fix the "truncated infinitives/futures" wording at `a2-b1-syllabus-map.md` §Unit 1 (pre-review §3). |
| ITA-9 | *Not recorded in the repo* | — | ? | — | Check the Paperclip board when it resumes. |
| ITA-10 | Unit 1 Italian sign-off | Italian Content Editor | in progress | — | Unblocked: Unit 1 is complete at `b046358`. Full review of `curriculum/units/unit-01/` against `docs/unit-01-italian-pre-review.md` §6. |
| ITA-11 | U7 `L4` spike: one lesson testing the L4 contract at its heaviest | Lesson Designer | in progress | — | Build `curriculum/units/unit-07/unit-07-lesson-04.md`; pass criteria are in the ITA-5 verdict. |
| ITA-12 | Template amendments from the ITA-5 verdict | Lesson Designer | blocked | ITA-4, ITA-10 | `piacere`-seed warning row (can start now); checkpoint re-alignment (after ITA-4); template examples synced to signed-off Unit 1 (after ITA-10). |

Open decision for the user (from ITA-7): ratify twelve units or choose fourteen.
Twelve is the working assumption.

---

## Log

Newest entry last within each task. Format: `- YYYY-MM-DD · who · what changed · next action (owner)`.

### ITA-4
- 2026-09-30 · Curriculum Architect · Wrote `rubrics.md`, `placement-check.md`, `unit-checkpoint-template.md`; session ended before the milestones and before committing. · Write both milestones (Curriculum Architect).
- 2026-10-12 · Chief · Moved to Claude Code. Committed the three finished files as-is. · Finish the milestones (Curriculum Architect).

### ITA-5
- 2026-10-02 · Lesson Designer · Unit 1 complete: 10 files, timings verified, 28 exercises keyed. Asked for a format verdict and a U7 `L4` spike decision. · Verdict (Chief).
- 2026-10-12 · Chief · Format verdict: accepted with three conditions; U7 `L4` spike approved (ITA-11). Conditions are tracked as ITA-12. · Spike (Lesson Designer).

### ITA-8
- 2026-09-30 · Curriculum Architect · Added Seed 4 (`Lei` imperatives as productive congiuntivo seeding) to `grammar-progression.md`; not committed. · Finish defects 1–3 + map wording (Curriculum Architect).

### ITA-10
- 2026-10-02 · Italian Content Editor · Pre-review at `ddf7de9` (`docs/unit-01-italian-pre-review.md`); blocked on ITA-5. · Full sign-off once Unit 1 exists (Italian Content Editor).
- 2026-10-12 · Chief · Unblocked: Unit 1 landed at `b046358`. · Full sign-off (Italian Content Editor).
