# Unit Template — how a unit is built

Owner: Lesson Designer · Task: ITA-5 · Status: for review by Chief Italian Linguist

This folder is the skeleton every one of the twelve units fills in. It is not a
style guide to read once — it is a set of files to **copy** into `unit-NN/`,
rename, and fill. Each template file carries a filled-in example of every
section, taken from Unit 1, so the template teaches by showing rather than by
describing.

The container is fixed by [`docs/format-brief.md`](../../../docs/format-brief.md)
(ITA-2). What each unit teaches, in what order, is fixed by
[`curriculum/syllabus/a2-b1-syllabus-map.md`](../../syllabus/a2-b1-syllabus-map.md)
(ITA-3) and its two companions. This folder fixes only **how a lesson is built
and written down**. If the syllabus and this template disagree, the syllabus
wins and the template is wrong — raise it with the Curriculum Architect rather
than quietly re-designing the unit.

---

## 1. What a unit folder contains

Copy these seven files into `unit-NN/`, substituting the zero-padded unit
number. Lowercase, hyphenated, zero-padded, per format brief §4.

| File | Owner | What it is |
| --- | --- | --- |
| `unit-NN-overview.md` | Lesson Designer | The eight-part skeleton for this unit on one page: can-do goals, input, lexis, grammar, pronunciation, culture, production task, checkpoint. The teacher's map of the unit and the learner's contents page. |
| `unit-NN-lesson-01.md` … `-05.md` | Lesson Designer | Five staged 90-minute lesson plans. One file per lesson. Self-contained: a teacher reads one file and runs the lesson. |
| `unit-NN-lexis.md` | Lesson Designer (structure) · Italian Content Editor (the Italian) | The unit's ~30 productive items as a learner-facing list, split into the L1 and L3 teaching sets, plus recognition-only items and the false-friend slot. |
| `unit-NN-checkpoint.md` | Lesson Designer, to the ITA-4 spec | The ~10-minute end-of-unit check run inside L5, with its key and its pass criterion. |
| `unit-NN-audio-script.md` | Lesson Designer (brief) · Italian Content Editor (the Italian) | Every audio cue in the unit as a recordable script: speaker, pace, intonation, and the eventual asset path. |
| `unit-NN-teacher-notes.md` | Lesson Designer | Unit-level notes that would be repeated in all five lessons if they lived in the lesson files: this unit's error profile, its register decisions, its known weak spots. |

**Eight parts, seven files.** The eight-part skeleton in the format brief is a
*content* checklist, not a file list. `unit-NN-overview.md` states all eight and
says which lesson carries each; the lesson files deliver them.

Nothing else goes in a unit folder. Answer keys live inside the lesson file
beside their exercise, not in a separate keys file — a teacher running a lesson
should never need a second file open.

---

## 2. The lesson-slot convention

Fixed by the syllabus map. Binding.

| Slot | Carries | Method that usually fits |
| --- | --- | --- |
| **L1** | Input and theme entry. Lexis set A. The unit's new structures appear **receptively only** — heard and read before they are analysed. | ESA (Engage–Study–Activate), where *Study* is text work, not grammar analysis |
| **L2** | The unit's one heavy structure, analysed and practised under control. | PPP, with the *Presentation* built out of guided discovery from L1's text |
| **L3** | Lexis set B, skills work, the pronunciation/intonation point, the secondary (light) grammar point, and the false-friend slot. | ESA |
| **L4** | Recycling of named earlier structures inside *this* unit's theme, plus the culture note. | ESA |
| **L5** | The production task and the unit checkpoint. | TBLT |

Two consequences the lesson files must respect:

- **L1 never explains the target form.** If L1 has a paradigm table in it, L1 is
  wrong. Noticing tasks that get learners to *collect* forms are correct; tasks
  that get them to *name* forms belong in L2.
- **L4 is not more practice of this unit's grammar.** Its content is dictated by
  the [`grammar-progression.md` §Per-unit L4 contract](../../syllabus/grammar-progression.md#per-unit-l4-contract).
  An L4 that drops its listed structures breaks the spiral for every later unit.

---

## 3. The lesson file header

Format brief §4 fixes the first five keys. This template adds five more, purely
additively, so coverage and recycling stay mechanically checkable.

```yaml
---
unit: 1
lesson: 1
level: A2
duration_min: 90
can_do: ["I can describe my daily and weekly routine in detail"]
grammar: ["riflessivi (receptive)", "presente indicativo (receptive)"]
# --- additions, ITA-5 ---
slot: L1                      # L1 | L2 | L3 | L4 | L5
method: ESA                   # ESA | PPP | TBLT — stated deliberately, see §4
lexis_set: A                  # A | B | — | recycled
recycles: []                  # e.g. ["U1 riflessivi", "U3 comparativi"]
selfstudy_min: 50             # 45–60 per format brief §3
---
```

Rules for the header:

- `duration_min` and the stage timings in the body **must** sum to the same
  number. A lesson that fails this is not done (format brief §3).
- `can_do` holds the **one** goal this lesson is accountable for, phrased
  learner-facing. A lesson with four can-do goals has none.
- `recycles` is empty only in Unit 1. Everywhere else, an empty `recycles` on an
  L4 file is a bug.

---

## 4. The nine things every lesson file must contain

In this order. The lesson template file shows each one filled in.

1. **Header block** (§3).
2. **Italian-review banner** — see §6. Delete only when the Italian Content
   Editor has signed off.
3. **At a glance** — the lesson's one goal, what the learner can do by the end,
   materials, and the teacher's prep time. Prep must be honest: if it is
   "read this file", say so.
4. **Stage map** — a table of stage / minutes / interaction pattern / purpose,
   with the total on the last row. This is the thing a teacher glances at with
   three minutes to go before class.
5. **Stages in full** — each with:
   - a **purpose** in one line (why this stage exists; cut the stage if you
     can't write it),
   - a **timing**,
   - a named **interaction pattern** — lockstep, pairs, small group, solo,
     mingle. An unnamed pattern becomes lockstep by default, which is the least
     useful one;
   - the **exact instruction to give**, in quotation marks, as a teacher would
     say it. Not "explain the task";
   - a **concept-check question** (CCQ) with its expected answer, for any stage
     where a learner could plausibly do the wrong task;
   - the **materials** inline — the sentences, the grid, the cards. A stage that
     says "use the gap-fill" without the gap-fill is unfinished.
6. **Exercises with answer keys**, keys immediately after each exercise. Open
   tasks carry a **model answer** or a **rubric**, never neither.
7. **Teacher notes** — the two or three errors this lesson will *predictably*
   produce from an English-L1 learner, and what to do about each; the
   error-correction stance per stage; one way to shorten the lesson and one way
   to extend it.
8. **Self-study version** — a real 45–60-minute solo route through the same
   material, with a solo equivalent for **every** pair or group stage. "Do this
   alone" is not a solo equivalent.
9. **After the lesson** — the homework, and one line on what the next lesson
   does with it.

---

## 5. The activity repertoire

Activity **formats** are shared across the course and referenced by code from
the lesson files: see [`activity-repertoire.md`](activity-repertoire.md).

A format used in ten units is worth more than ten novel formats. Learners who
recognise the mechanics of a task spend their attention on the Italian instead
of on the instructions, and a teacher who has run `A7 Information gap` twice
needs one line of set-up rather than a paragraph.

**Rule:** if a lesson needs a format that is not in the repertoire, add it to
the repertoire with a code, or use one that is. Do not invent a one-off.

---

## 6. Italian content — the banner and the review gate

All Italian is written or signed off by the **Italian Content Editor** (format
brief §5). Until that sign-off, every file containing Italian carries this
banner directly under its header block:

```markdown
> ⚠️ **Italian awaiting review.** Every Italian word in this file — dialogue,
> reading text, example sentences, exercise items, answer keys — is a Lesson
> Designer **draft**, not finished copy, and is marked `[ITA?]` at the section
> level. Do not teach from it or record it until the Italian Content Editor has
> signed off. Review task: ITA-NN.
```

- Mark each Italian-bearing section with `[ITA?]` in its heading so a reviewer
  can find every one by grep, and so nothing is missed because it looked like
  structure rather than content.
- When sign-off lands, delete the banner and the `[ITA?]` marks in the same
  commit, and say in the commit message which review task passed it.
- **A file marked finished with unreviewed Italian in it is not finished.** This
  is the single most common way this project could ship something wrong.

The template files in *this* folder contain Italian too — inside their filled
examples, which are lifted from Unit 1. That Italian is draft like any other and
is covered by the same review task, **ITA-10**. When Unit 1's Italian is signed
off, the examples here are updated to match it in the same pass; a filled example
that disagrees with the finished unit is worse than no example.

---

## 7. The bar for done

A lesson is done when a teacher who has never met you could run it tomorrow
morning with no preparation beyond reading the file.

Checklist — all of it, not most of it:

- [ ] Stage timings sum to `duration_min`.
- [ ] Every stage has a purpose, a timing, a named interaction pattern, and the
      exact instruction in quotation marks.
- [ ] Every stage where the task could be misread has a CCQ with its answer.
- [ ] Every exercise has a key. Every open task has a rubric or a model answer.
- [ ] Every pair or group stage has a stated solo equivalent.
- [ ] Teacher notes name two or three predictable errors and what to do.
- [ ] One shortening and one extension are named.
- [ ] Every free-production stage has a scaffold **and** a success criterion.
- [ ] All Italian is signed off, or the banner is present and the review task
      exists and is linked.
- [ ] You have read the lesson once as the teacher, start to finish, and could
      walk in and run it.

Not done, specifically: timings that don't sum; an exercise with no key; a
"free production" stage with no scaffolding and no success criterion;
unreviewed Italian in a file marked finished; a pair activity with no solo path.

**Never ships:** anything copied or closely adapted from a published textbook or
exam paper. Model the task *type*; write original content.

---

## 8. Files in this folder

| File | Use |
| --- | --- |
| [`unit-NN-overview.md`](unit-NN-overview.md) | Copy → `unit-NN/unit-NN-overview.md` |
| [`unit-NN-lesson-NN.md`](unit-NN-lesson-NN.md) | Copy five times → `unit-NN-lesson-01.md` … `-05.md` |
| [`unit-NN-lexis.md`](unit-NN-lexis.md) | Copy → `unit-NN/unit-NN-lexis.md` |
| [`unit-NN-checkpoint.md`](unit-NN-checkpoint.md) | Copy → `unit-NN/unit-NN-checkpoint.md` |
| [`unit-NN-audio-script.md`](unit-NN-audio-script.md) | Copy → `unit-NN/unit-NN-audio-script.md` |
| [`unit-NN-teacher-notes.md`](unit-NN-teacher-notes.md) | Copy → `unit-NN/unit-NN-teacher-notes.md` |
| [`activity-repertoire.md`](activity-repertoire.md) | Do **not** copy. One shared file, referenced by code from every lesson. |

The worked reference implementation of all of it is
[`../unit-01/`](../unit-01/).

---

## 9. Lexis presentation — the decision, and why

This section closes the open item
[`lexis-progression.md` §Open](../../syllabus/lexis-progression.md#open-and-who-owns-it):
*"Glossary format, item presentation, and whether items are front-loaded in `L1`/`L3`
or distributed"* — owned by Lesson Designer, in ITA-5. Binding from here on.

**1. Items are front-loaded into two teaching sets, not distributed.** Set A is
taught in `L1`, set B in `L3`, and a unit may carve out a small **set A′** for
`L2` where an item is inseparable from the grammar point (Unit 1 puts `vedersi`
and `sentirsi` in `L2`, because the reciprocal is the unit's own morphology doing
a second job).

Why front-loading wins over a trickle of six items a lesson:

- **A lesson needs enough lexis to make its task possible.** `L1`'s output stage
  asks for a routine at length; eleven reflexive verbs delivered at once make
  that sayable, and three a lesson do not. Distributed lexis produces lessons
  whose production stage is bottlenecked on vocabulary the learner meets
  tomorrow.
- **Spacing is what matters for retention, and front-loading buys *more* of it,
  not less.** An item taught in `L1` is recycled in `L2`, `L4` and `L5` and
  tested at the checkpoint — four spaced encounters. An item introduced in `L4`
  gets one encounter and a checkpoint item. Front-loading is what makes the
  "met in" column in `unit-NN-lexis.md` have anything in it.
- **It gives the unit a shape a learner can feel:** `L1` is "my week", `L3` is
  "my people". Two sets, two themes, two lessons.

The cost, stated plainly: `L1` and `L3` each carry a 13–15-minute lexis stage,
which is the heaviest single stage in either lesson, and the one most likely to
overrun. Each unit's teacher notes must name it as such.

**2. The glossary format is `unit-NN-lexis.md`, four sections, fixed columns:**
*Italian · English · example sentence · met in* — the shape set out in
[`unit-NN-lexis.md`](unit-NN-lexis.md). Three things in that shape are
load-bearing:

- **The example sentence is compulsory and must be sayable about the learner's
  own life.** `Mi sveglio alle sette meno un quarto` teaches the item; *"to wake
  up: svegliarsi"* glosses it. An item with no example sentence has been listed,
  not taught.
- **The "met in" column is a check, not decoration.** An item whose only entry is
  the lexis-presentation stage has not been taught, and the column makes that
  visible without reading five lesson files.
- **Citation form is the form the learner should store** — infinitive, article
  where gender is not predictable, masculine singular for adjectives — matching
  `lexis-progression.md` exactly, so that document and this one can be diffed.

**3. Recognition-only items are listed but never counted or tested.** They sit in
their own section with a one-line note where they are deliberately unexplained,
so a learner who meets `mi serve` in a text can look it up and still be told, in
writing, that it is not yet their job to build it.
