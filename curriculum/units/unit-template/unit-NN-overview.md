# TEMPLATE — Unit overview

> **How to use this file.** Copy to `unit-NN/unit-NN-overview.md`. Every section
> below appears twice: the **shape** (what goes here, and the test it has to
> pass) and a **filled example** taken from Unit 1, so you can see what "done"
> looks like. Delete the shape blocks and the `> ` quoting when you fill it in.
> The finished article is [`../unit-01/unit-01-overview.md`](../unit-01/unit-01-overview.md).

---

```yaml
---
unit: NN
title_it: "<Italian unit title>"
title_en: "<English unit title>"
level: <A2 | A2+ | B1 lower | B1>
lessons: 5
duration_min: 450
lexis_set: NN
main_grammar: ["<the one heavy structure>"]
secondary_grammar: ["<the one light point>"]
recycles: ["<U? structure>", "…"]
---
```

> ⚠️ **Italian awaiting review.** Every Italian word in this file is a Lesson
> Designer **draft**. Review task: ITA-NN.

---

## 1. Can-do goals

> **Shape.** Lift them from the syllabus map — do not rewrite them, and do not
> add any. Three to five, each tagged with its level band, each phrased
> learner-facing ("I can …") so a learner can self-assess at the end of the unit
> with no teacher present. Then map each goal to the lesson that is accountable
> for it, and to the checkpoint item that tests it. A goal with no lesson is a
> promise nothing keeps; a goal no checkpoint item tests is not assessed.

**Filled example (Unit 1)**

| # | Can-do goal | Level | Owned by | Tested by |
| --- | --- | --- | --- | --- |
| 1 | I can introduce myself and describe my daily and weekly routine in enough detail that someone gets a real picture of my life, not just a list of times. | A2 | L1, L2 | Checkpoint C + spoken task |
| 2 | I can describe the people closest to me — what they're like and how I get on with them — using several different character adjectives. | A2 | L3 | Checkpoint B + written task |
| 3 | I can say what I like, need and miss using fixed expressions, even though I can't yet explain how they work. | A2 | L3 | Checkpoint B4–B5 |
| 4 | I can ask someone the same questions back and keep a short conversation about routines going without stalling. | A2+ | L4 | L4 interview carousel, L5 follow-up |

---

## 2. Input text / dialogue

> **Shape.** Name every input in the unit, with: which lesson it sits in, what
> kind of text it is, its length, and **what it has to contain** — the target
> structures it must model, the lexis it must carry, and any receptive seeds the
> grammar progression requires to be planted in it. That last part matters:
> receptive seeding only exists if the chunks are actually in the texts.
>
> This section is a **specification for the Italian Content Editor**, not the
> text itself. The texts live in the lesson files and, if spoken, in
> `unit-NN-audio-script.md`.

**Filled example (Unit 1)**

| Input | Lesson | Type | Length | Must contain |
| --- | --- | --- | --- | --- |
| `Un messaggio vocale da Giulia` | L1 | Voice message, one speaker | ~190 words | All 11 reflexive routine verbs; ≥6 present-tense irregulars; one reciprocal (`ci vediamo`). **No** `piacere` chunks — they are seeded in L3, not before. |
| `Tre persone intorno a me` | L3 | Three short spoken descriptions | 3 × ~60 words | 8 people/relationship items; ≥7 character adjectives; all five `piacere` chunks, unanalysed; `i parenti` in a context that forces the "relatives" reading. |
| `Due profili` | L4 | Two written profiles, one `tu`, one `Lei` | 2 × ~90 words | Same content in both registers; ≥5 question forms; adjective agreement across both genders. |
| `Un ritratto in due minuti` | L5 | Model self-portrait, one speaker | ~230 words | The task's target shape, at the standard the success criterion asks for — no better. |

---

## 3. Lexis set

> **Shape.** One line on the set, then the **split**: which items are taught in
> L1 (set A) and which in L3 (set B), with the count of each. The syllabus's
> thematic subgroups are not automatically the teaching sets — say which split
> you chose and why, because the lexis progression binds you to "set A in L1,
> set B in L3" and nothing finer. Name the unit's false-friend item and the
> recognition-only items that sit outside the thirty.
>
> Full learner-facing list: `unit-NN-lexis.md`.

**Filled example (Unit 1)**

Set 1 — *Routine, carattere, rapporti*, 30 productive items
([`lexis-progression.md` §Unit 1](../../syllabus/lexis-progression.md#unit-1--routine-carattere-rapporti)).

| Teaching set | Lesson | Items | Count |
| --- | --- | --- | --- |
| **A** | L1 | The 11 reflexive routine verbs | 11 |
| **A′** | L2 | The two reciprocals, `vedersi` / `sentirsi` — they belong to the *grammar* stage, because the reciprocal is the same morphology doing a second job | 2 |
| **B** | L3 | The 8 people-and-relationships items + the 9 character adjectives and `andare d'accordo`, `litigare` | 17 |
| | | **Total** | **30** |

Outside the thirty: the five-chunk receptive `piacere` set (L3, unanalysed).
False-friend slot (L3): `i parenti` ≠ *parents*.

---

## 4. Grammar focus

> **Shape.** The one heavy structure and the one light point, straight from the
> syllabus map. Then the part the map does not decide: **what exactly gets
> taught, in what order, inside the heavy structure** — the two or three facts
> the lesson turns on — and **what is explicitly deferred**. Deferral is a
> design act; write it down, or the lesson grows.

**Filled example (Unit 1)**

- **Main — riflessivi (consolidation), with presente indicativo.** Taught in
  this order, because it is the order of difficulty for an English L1 learner:
  1. the pronoun is **obligatory** (`mi sveglio`, never `sveglio` for "I wake
     up") — this is the error that survives longest;
  2. the pronoun **agrees with the subject**, so it changes when the subject
     changes;
  3. **placement**: before the conjugated verb; with a modal, either
     `mi devo alzare` or `devo alzarmi`, and never `devo mi alzare`.
  Plus the reciprocal use (`ci vediamo`, `ci sentiamo`) as a fourth, lighter
  step, and the ten high-frequency present-tense irregulars as maintenance.
- **Secondary — the `piacere` family as unanalysed chunks.** `mi piace / mi
  piacciono / mi interessa / mi serve / mi manca`, taught as fixed expressions
  and **explicitly not explained**. Deliberate seeding for U8.
- **Deferred, and say so to learners if they ask:** reflexives in the past
  (U2); `si` impersonale, which shares the surface form (U4); why `piacere`
  works the way it does (U8).

---

## 5. Pronunciation / intonation point

> **Shape.** The point, from the map; the two or three concrete cases it covers;
> the minimal pairs or contrasts used; and the lesson it sits in (always L3).
> The test: is the feature **meaning-bearing** in the practice, or decorative?
> If getting it wrong changes nothing a listener understands, it will not stick.

**Filled example (Unit 1)**

**Word stress.** L3, via `A9`.
- The penultimate-syllable default.
- `-ano` third-person plurals — `àbitano`, `telèfonano`, `svègliano` — where an
  English-L1 learner reliably stresses the penultimate by analogy and produces
  *abìtano*.
- Truncated infinitives and futures (`caffè`, `perché`, `farò`), stressed final.
- Meaning-bearing pairs: `pàrlano` / `parlerànno`, `àbito` / `abìto`,
  `càpito` / `capitò`, `àncora` / `ancòra`.

---

## 6. Culture note

> **Shape.** The note, from the map; the **behavioural** takeaway — what the
> learner should actually do or say differently, not a fact they now know; and
> which later unit it sets up. Written for someone approaching Italy from
> outside (format brief §1), which mostly means: explain what is *unmarked* in
> Italy, not what is picturesque.

**Filled example (Unit 1)**

**`tu` and `Lei`, and how Italians negotiate the switch.** L4, via `A10`.
Who offers `diamoci del tu` and who waits to be offered it; what `dottore`,
`ingegnere` and `professore` are doing; why an anglophone defaulting to `tu`
reads differently from an anglophone defaulting to first names in English.
- **Behavioural takeaway:** with someone you have not met and who is not
  obviously your peer, start with `Lei`, and let them downgrade it.
- **Sets up:** U7 (`Lei` imperatives), U11 (formal requests).

---

## 7. Production task

> **Shape.** The task itself, spoken and written, from the map — and the
> **success criterion**, which must be countable. "Speaks fluently" is not a
> criterion. "Runs two minutes with no stall longer than five seconds, six
> correct reflexives, two people described with a character adjective each" is,
> and a solo learner can apply it to their own recording.
>
> Also state the **scaffold** and where it is removed. A free-production stage
> with no scaffold and no success criterion is the single most common way a
> lesson plan fails review.

**Filled example (Unit 1)**

- **Spoken:** a two-minute audio self-portrait — who I am, what a normal week
  looks like, who's around me.
- **Written:** a language-exchange profile, ~120 words, same ground, for a
  reader.
- **Success criterion.** The spoken piece runs two minutes with no stall longer
  than five seconds; uses at least six reflexive verbs correctly in the present;
  describes at least two people with a character adjective each.
- **Scaffold and its removal.** L5 supplies a model (`A6` rung 1) and a
  five-frame planner (rung 2). For the recorded attempt the planner is reduced
  to five written words (rung 3). The frames do not appear in the deliverable.

---

## 8. Checkpoint

> **Shape.** One line on what it covers and its pass criterion. The instrument
> itself is `unit-NN-checkpoint.md` and its spec is ITA-4. Proportions are fixed
> by `A12`: ~40% lexis, ~40% the unit's main grammar, ~20% recycled material.
> Unit 1 is the one unit with nothing earlier to recycle, so its recycled
> portion comes from **within** A2.

**Filled example (Unit 1)**

10 minutes, solo, at the start of L5's second half. 25 marks: lexis 10, riflessivi
and presente 10, within-A2 recycling (question forms, adjective agreement) 5.
Pass criterion 18/25, plus a self-rating against each of the four can-do goals.
See [`../unit-01/unit-01-checkpoint.md`](../unit-01/unit-01-checkpoint.md).

---

## 9. Lesson map

> **Shape.** The five lessons on one line each: slot, title, its one can-do
> goal, its method, and the lexis or grammar it carries. This is the table a
> teacher taking over the unit mid-way reads first. Keep the method column
> honest — see `README.md` §2.

**Filled example (Unit 1)**

| Lesson | Title | Slot carries | Method | Its one goal |
| --- | --- | --- | --- | --- |
| [L1](../unit-01/unit-01-lesson-01.md) | La settimana di Giulia | Input; lexis set A; riflessivi receptive | ESA | Understand and give a detailed routine |
| [L2](../unit-01/unit-01-lesson-02.md) | Un giorno tipo | Riflessivi analysed; presente irregulars | PPP | Produce accurate reflexives, incl. with modals |
| [L3](../unit-01/unit-01-lesson-03.md) | Le persone intorno a me | Lexis set B; word stress; `piacere` chunks; false friend | ESA | Describe people with character adjectives |
| [L4](../unit-01/unit-01-lesson-04.md) | Raccontami di te | Recycling (questions, agreement) + culture note | ESA | Ask back and keep the conversation going |
| [L5](../unit-01/unit-01-lesson-05.md) | Il mio ritratto | Production task + checkpoint | TBLT | Perform the two-minute self-portrait |

---

## 10. What this unit recycles, and what it seeds

> **Shape.** Two lists, both taken from `grammar-progression.md`. **Recycles** is
> the L4 contract for this unit — binding. **Seeds** is what later units depend
> on this unit planting, which is the thing most likely to get quietly dropped
> when a lesson runs long.

**Filled example (Unit 1)**

- **Recycles.** Nothing from earlier units — Unit 1 is the entry unit and the
  only one in the course with no spiral obligations. Its L4 recycles *within*
  A2: present-tense question forms and adjective agreement.
- **Seeds.**
  - the five `piacere` chunks, for analysis at `U8 L2` — seven units of
    exposure, and the course's proof case for receptive seeding;
  - `sbrigarsi`, whose imperative is needed at U7;
  - `farsi la doccia` — a reflexive with a direct object, which anticipates
    participle agreement at U6;
  - the `tu`/`Lei` register axis the whole course runs on.
