# Unit template — format verdict

Reviewer: Chief Italian Linguist · Task: ITA-5 · Date: 2026-10-12
Reviewed: `curriculum/units/unit-template/` and `curriculum/units/unit-01/` at
`b046358` (Lesson Designer).

## Verdict

**Accepted as the course format, with three conditions.** The template
scales to twelve units. Units 2–12 are built to it.

What earns the acceptance:

- **The lesson-slot convention (template README §2) is the right contract.** It
  turns the syllabus map's per-unit row into five lesson jobs that a writer
  cannot blur. L1 never explains; L2 carries the one heavy structure; L4 is
  dictated by the progression, not chosen. The cognitive-load and
  input-before-output rules from the syllabus are now enforced at file level, not
  just stated.
- **Its checks are mechanical, not a matter of taste.**
  - I re-added all five Unit 1 stage maps myself: 90, 90, 90, 90, 90.
  - The extra header keys (`slot`, `method`, `recycles`) make coverage greppable.
  - The `[ITA?]` banner turns the review gate into something that can be found.
- **The activity repertoire is the right economy.** Thirteen formats, each
  with a solo equivalent and a correction stance, means a teacher in Unit 9 needs
  one line of set-up rather than a paragraph.
- **The teacher notes tell the truth.** §4 lists seven weak spots, and the first
  is the one I would have raised: Unit 1's L4 proves nothing about the L4
  contract. A sample unit that names its own limits is worth more than one that
  looks finished.
- **The lexis front-loading decision (README §9) is argued, not asserted.** It
  is correct on spacing grounds.

## Decision — the U7 `L4` spike: yes

Build **`curriculum/units/unit-07/unit-07-lesson-04.md` alone**, before Units
2–6. It is roughly a fifth of a unit's cost. It tests the one thing Unit 1
cannot: whether a 90-minute L4 can actually recycle four named earlier
structures, including clitic attachment to imperatives, inside a new theme
without becoming a grammar revision class.

- Build it against the syllabus map's U7 row and the `grammar-progression.md`
  per-unit L4 contract. Units 2–6 don't exist yet; the spec is enough.
- **Pass:**
  - the timings sum to 90;
  - every listed L4 structure is elicited in production, not merely mentioned;
  - the culture note survives;
  - the self-study route is real.
- **If it fails,** the fix goes into the template's L4 rules before Unit 2 is
  started. That is the point of doing it now.
- Its Italian is draft until the Italian Content Editor passes it, as usual.

## Conditions on the acceptance

1. **The `piacere` seed warning (weak spot 2).** Add a fixed row to
   `unit-NN-teacher-notes.md` §Register/§Weak spots, mandatory for U2–U7:
   "`piacere` chunks are recognition-only until `U8 L2`; do not explain the
   construction." It costs one line per unit and protects a seven-unit seed.
2. **The checkpoint is revised against ITA-4.** When the assessment framework
   lands (milestones in progress), the template checkpoint and
   `unit-01-checkpoint.md` are re-aligned to `assessment/unit-checkpoint-template.md`
   in one pass. Weak spot 4's 18/25 boundary is provisional until then.
3. **The template examples follow the Unit 1 Italian sign-off (ITA-10).** Per
   README §6, the filled examples in the template are updated to match the
   signed-off Unit 1 in the same pass. A template that disagrees with its own
   reference unit is worse than no example.

Weak spot 7 (`i parenti` counting) stays with the Curriculum Architect. Weak
spot 3 (no recorded audio) is accepted for v1; cue 3 goes first in the
recording queue when recording is in scope.

## What this hands on

| To | What |
| --- | --- |
| **Lesson Designer** | ITA-11: the U7 `L4` spike. ITA-12: conditions 1–3, with 2 waiting on ITA-4 and 3 waiting on ITA-10. Units 2–6 start after ITA-11 passes. |
| **Curriculum Architect** | Finish ITA-4; condition 2 depends on it. |
| **Italian Content Editor** | ITA-10 as briefed; condition 3 depends on it. |
| **User** | Ratified twelve units on 2026-10-12 (format brief decision log). |

---

## Spike result (ITA-11) — 2026-10-12

**Passed.** `curriculum/units/unit-07/unit-07-lesson-04.md` meets all four
criteria. The stage map re-adds to 90, which I checked. All four contract
structures are produced, and each has a ledger entry. The culture note became
the input text, so it cannot be cut quietly.

**The L4 template amendment the Lesson Designer proposed is approved in full**
and goes into the template under ITA-12 before Unit 2 starts:

- README §2: an "extended structure" clause, contract structures grouped into
  task-clusters of two or three, and the culture note placed as or beside the
  L4 input text.
- README §4: a compulsory **contract ledger** in every L4 file. Never cut the
  only production site of a bolded structure. The same rule goes into the
  teacher-notes "to shorten" shape.
- README §3: mandated `recycles` entries are marked `(mandated)`.
- `activity-repertoire.md` `A2`: an "L4 recycling use" line.

**This corrects the original verdict.** U7 is not the heaviest L4 contract:
U8 (6 of 7 entries bolded) and U11 (5 of 8) are. The spike proves the format
for contracts of up to about four structures, which covers U2–U7. Before U8 is
built, its L4 gets a paper stage-map check, recorded as a gate on the board.
Unit 2 can start once ITA-12 lands.
