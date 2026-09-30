# Course Format Brief

Owner: Chief Italian Linguist · Status: decided, open to correction · Task: ITA-2

This brief fixes the container the A2→B1 curriculum is built into. The syllabus
map, the unit template, and the assessment framework all assume these answers.
Each decision states its reason and how expensive it is to reverse.

---

## 1. Learner profile

We are designing for an **adult learner (18+) whose first language is English**,
already at solid A2, learning Italian for life reasons — work, family, living in
or travelling to Italy — rather than for an exam. Assume roughly two guided
sessions a week, so the course runs about seven to eight months end to end.

Why it matters: L1 drives the whole error-anticipation layer. An anglophone
learner's trouble with `piacere`, auxiliary choice, adjective agreement, and
false friends (`eventualmente`, `attualmente`, `libreria`, `parenti`) is
specific and predictable. Culture notes are written for someone approaching
Italy from outside, not from a neighbouring Romance language.

**Reversibility: cheap now, expensive later.** Widening beyond anglophone
learners costs little today and means reworking every error note after unit 3.

## 2. Delivery mode — self-study-first, teachable live

Every lesson is written so a **solo learner can complete it unaided**. The same
file carries teacher notes that let it run as a live 90-minute class.

Why: no delivery constraint was set, and the self-study-capable version is a
superset of the live one. Writing for a solo learner forces what live teaching
also benefits from — exact instructions, answer keys, worked models, and a
stated success criterion for every task. The reverse does not hold: material
written for a teacher in the room leaves holes a solo learner falls into.

Concretely: **every pair or group activity carries a stated solo equivalent.**
An activity with no solo path is not finished.

**Reversibility: cheap.** Dropping the solo layer later is deletion. Adding it
later is a rewrite.

## 3. Lesson length and load

| | |
| --- | --- |
| Guided lesson | **90 minutes** |
| Self-study per lesson | **45–60 minutes** |
| Lessons per unit | 5 |
| Units | 12 |
| Total | 60 lessons, ~90 guided hours |

Ninety minutes is the standard adult-class block and gives room for a real
lesson arc — short opener, heavy middle, productive close — without the
fatigue of a two-hour session.

On total load, be honest: the usual published estimate for A2→B1 is **150–200
guided hours**, and we are planning 90 guided plus roughly 50 of self-study.
Three things have to hold for that to work, and all three are load-bearing
rather than optimistic: entry is **solid** A2, not weak A2; self-study is **not
optional**, because it carries lexis drilling and receptive practice out of
class time; and grammar is **spiralled**, so each structure is taught once and
recycled free inside later themes. If the placement check shows real learners
entering weaker than assumed, the honest fix is more units — not longer lessons.

Timings are part of every lesson plan. **A lesson whose stage timings do not sum
to 90 minutes is not done.**

**Reversibility: expensive after the sample unit ships.** Lesson length is the
unit of design; changing it re-stages every lesson.

## 4. Materials format

**Markdown in this git repo. Nothing else is a source file.**

- One file per lesson: `curriculum/units/unit-03/unit-03-lesson-02.md`.
- Unit-level material sits beside the lessons: lexis list, checkpoint, unit
  overview, teacher notes.
- Lowercase, hyphenated, zero-padded names throughout.
- Every lesson file opens with a header block:

  ```yaml
  ---
  unit: 3
  lesson: 2
  level: A2+
  duration_min: 90
  can_do: ["Can describe a past routine and contrast it with the present"]
  grammar: ["imperfetto vs passato prossimo"]
  ---
  ```

  This makes the course checkable — coverage, recycling, and level drift can be
  verified mechanically later instead of by reading sixty files.

Why markdown and git: the whole course stays diffable and reviewable. Two
people editing the same unit is a merge, not an email. A `.docx` or a PDF as a
source file breaks all of that.

**Audio:** written as scripts now (`unit-03-audio-script.md`), recorded later.
Scripts mark speaker, pace, and the intonation contours that carry meaning.
Recording is out of scope for v1 — but the scripts must be recordable as
written. Nothing is recorded until the script is content-edited and signed off;
re-recording is the most expensive rework in this project. So that later
recording needs no renaming, each cue names its eventual file up front:
`assets/audio/unit-03/u03-l02-dialogo.mp3`. *Cheap to change while scripts,
expensive once recorded.*

**Images:** not required for v1. Where a visual is genuinely needed, describe it
inline as `> [visual: …]` so it can be commissioned later without guesswork.
When one is commissioned it lands at `assets/images/unit-03/u03-l02-<slug>.png`
(`.svg` for diagrams and tables), is referenced with a relative link, and
carries English alt text. No image may carry meaning that isn't also in the
text — for accessibility, and because images are the costliest asset to replace.

**Reversibility: cheap.** Markdown exports to anything. The inverse is painful.

## 5. Consistency rules

- Every unit follows the same eight-part skeleton: can-do goals → input
  text/dialogue → lexis set (~30 items) → grammar focus → pronunciation/
  intonation point → culture note → production task → checkpoint.
- Activity types come from a shared repertoire rather than being reinvented per
  unit. An activity format used three times is worth more than three novel
  formats — learners stop spending attention on mechanics and start spending it
  on Italian.
- All Italian is written or signed off by the Italian Content Editor. No
  exceptions, including example sentences inside syllabus and assessment
  documents.

## 6. Out of scope for v1

Recorded audio, video, an LMS or platform, a mobile app, printable workbooks,
and exam-prep-only tracks. The deliverable is the course content. Packaging is a
separate decision, and markdown keeps every packaging option open.

---

## Open question flagged to the board

The **anglophone L1 assumption** in §1 is the one decision here that was not
implied by anything already agreed. It is cheap to change now and expensive
after a few units are built. If the intended learners have a different first
language — or a mixed one — say so and this brief gets revised before ITA-3
publishes the syllabus map.
