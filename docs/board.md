# Task board

The in-repo stand-in for the Paperclip board while Paperclip is paused. The
Chief Italian Linguist (the main Claude Code session) is the only editor:
agents end each report with a `Board:` block and the Chief copies it in. When Paperclip resumes,
reconcile this file back onto the Paperclip board, then stop editing it there or
here — one board at a time.

Statuses: `todo` · `in progress` · `blocked` · `in review` · `done`.
New tasks continue the Paperclip numbering from **ITA-18**.

| ID | Title | Owner | Status | Blocked by | Next action |
| --- | --- | --- | --- | --- | --- |
| ITA-1 | Confirm learner L1 (format brief open question) | Chief | done | — | — |
| ITA-2 | Format brief | Chief | done | — | — |
| ITA-3 | 12-unit syllabus map + grammar and lexis progressions | Curriculum Architect | done | — | Accepted in `docs/syllabus-shape-review.md` (ITA-7). |
| ITA-4 | Assessment framework | Curriculum Architect | done | — | Accepted: `docs/assessment-framework-review.md`. Italian for the instruments follows as ITA-15 onward. |
| ITA-5 | Unit template + sample Unit 1 | Lesson Designer | done | — | Accepted with three conditions: `docs/unit-template-format-verdict.md`. Conditions are carried by ITA-12. |
| ITA-6 | Vet the Italian in the three syllabus documents | Italian Content Editor | done | — | Pass with edits at `3961be5`. |
| ITA-7 | Syllabus shape review | Chief | done | — | `docs/syllabus-shape-review.md`. |
| ITA-8 | Apply shape-review defects 1–3 + the `Lei`-imperative strand | Curriculum Architect | in progress | — | Defects 1–3 check; map line 280 "truncated infinitives"; map §5 stale "Receptive seeding" ref + Seed 4; grammar-progression "seven" → six; `i parenti` counting; rule on movement-preposition ownership (U7 L3 vs L4) and the "extended to" reading. |
| ITA-9 | *Not recorded in the repo* | — | ? | — | Check the Paperclip board when it resumes. |
| ITA-10 | Unit 1 Italian sign-off | Italian Content Editor | done | — | Pass with edits, all 10 files: `docs/unit-01-italian-signoff.md`. Cue 1 recording held until ITA-14; cues 2–4 recordable. |
| ITA-11 | U7 `L4` spike: one lesson testing the L4 contract at its heaviest | Lesson Designer | done | — | Passed. Template L4 amendment approved (verdict doc, "Spike result"). Gate: U8 L4 paper stage-map check before U8 is built. |
| ITA-12 | Template amendments (ITA-5 conditions + ITA-11 L4 amendment) | Lesson Designer | in progress | — | `piacere` row; template sync from sign-off §6; checkpoint re-alignment to ITA-4 (incl. Unit 1 "do not move on" → no-blocking); the L4 amendment. Gates Unit 2. |
| ITA-13 | Italian review of the U7 `L4` spike | Italian Content Editor | in progress | — | Review `unit-07-lesson-04.md` once the spike lands. |
| ITA-14 | Unit 1 staging fixes from the Italian sign-off | Lesson Designer | in progress | — | Sign-off §4: reconcile cue 1 length target (~1:50 vs 1:20–1:35; hold on recording), cue 4 word count, L3 s8 step 1 instruction, L2 s2 Q3 count, L1 ex3 key order, L3 ex2 note, L3 extension prompt count. |
| ITA-15 | Write the placement check's Italian | Italian Content Editor | in progress | — | All `⟨…⟩` specs in `assessment/placement-check.md`. Ships before Unit 1 is taught. |
| ITA-16 | Write the Italian for Milestones 1 and 2 | Italian Content Editor | todo | ITA-15 | Per each milestone's Open table. |
| ITA-17 | Verify the CILS/CELI B1 mapping against the publishers' current specs | Chief | todo | — | Before any learner-facing material names the exams. |

Decided 2026-10-12 by the user: **twelve units** (recorded in `docs/format-brief.md` decision log).

Open for the user (ITA-4 review): what a learner who gets "not yet" at Milestone 2 is offered beyond section resits.

---

## Log

Newest entry last within each task. Format: `- YYYY-MM-DD · who · what changed · next action (owner)`.

### ITA-4
- 2026-09-30 · Curriculum Architect · Wrote `rubrics.md`, `placement-check.md`, `unit-checkpoint-template.md`; session ended before the milestones and before committing. · Write both milestones (Curriculum Architect).
- 2026-10-12 · Chief · Moved to Claude Code. Committed the three finished files as-is. · Finish the milestones (Curriculum Architect).

### ITA-4 (cont.)
- 2026-10-12 · Curriculum Architect · Wrote both milestones; aligned rubrics, placement and checkpoint template; all links resolve. · Chief review.
- 2026-10-12 · Chief · Accepted, with rulings on six open items (`docs/assessment-framework-review.md`). · ITA-15 Italian (Italian Content Editor).

### ITA-11
- 2026-10-12 · Lesson Designer · Built U7 L4; 90/90, all four structures produced, culture note as input text. L4 template needs clustering, a ledger and an extended-structure clause; U8/U11 contracts are heavier than U7. · Chief verdict.
- 2026-10-12 · Chief · Passed; template amendment approved into ITA-12; U8 L4 paper check gate. · ITA-12 (Lesson Designer), ITA-13 (Italian Content Editor).

### ITA-5
- 2026-10-02 · Lesson Designer · Unit 1 complete: 10 files, timings verified, 28 exercises keyed. Asked for a format verdict and a U7 `L4` spike decision. · Verdict (Chief).
- 2026-10-12 · Chief · Format verdict: accepted with three conditions; U7 `L4` spike approved (ITA-11). Conditions are tracked as ITA-12. · Spike (Lesson Designer).

### ITA-8
- 2026-09-30 · Curriculum Architect · Added Seed 4 (`Lei` imperatives as productive congiuntivo seeding) to `grammar-progression.md`; not committed. · Finish defects 1–3 + map wording (Curriculum Architect).

### ITA-10
- 2026-10-02 · Italian Content Editor · Pre-review at `ddf7de9` (`docs/unit-01-italian-pre-review.md`); blocked on ITA-5. · Full sign-off once Unit 1 exists (Italian Content Editor).
- 2026-10-12 · Chief · Unblocked: Unit 1 landed at `b046358`. · Full sign-off (Italian Content Editor).
- 2026-10-12 · Italian Content Editor · Full review: pass with edits on all 10 files. Stress pairs, accents, contours, an error-clinic item that was not an error, `conoscente`, `Ing. Ferri` and more fixed in place; pre-review §6 items checked. Cue 1 recording held. · Staging fixes ITA-14, template sync ITA-12 (Lesson Designer); map line 280 ITA-8 (Curriculum Architect).
