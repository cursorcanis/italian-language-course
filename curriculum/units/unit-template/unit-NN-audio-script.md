# TEMPLATE — Unit audio script

> **How to use this file.** Copy to `unit-NN/unit-NN-audio-script.md`. Recording
> is out of scope for v1 (format brief §4) — but **the scripts must be
> recordable as written**, and nothing is recorded until the Italian Content
> Editor has signed it off, because re-recording is the most expensive rework in
> this project.
>
> Until a recording exists, the teacher reads the script aloud and the
> self-study learner reads it silently once and then covers it. Say so in the
> lesson file; do not leave a learner waiting for audio that does not exist.
>
> Shape first, then a filled example from Unit 1. Finished article:
> [`../unit-01/unit-01-audio-script.md`](../unit-01/unit-01-audio-script.md).

---

```yaml
---
unit: NN
cues: N
recorded: false
---
```

> ⚠️ **Italian awaiting review.** Every Italian word in this file is a Lesson
> Designer **draft**. **Nothing here may be recorded** until the Italian Content
> Editor has signed off. Review task: ITA-NN.

---

## Shape

### The cue index

Every cue names its **eventual asset path up front**, so that later recording
needs no renaming (format brief §4):

| Cue | Asset path | Lesson | Speakers | Length | Purpose |
| --- | --- | --- | --- | --- | --- |
| 1 | `assets/audio/unit-NN/uNN-lNN-<slug>.mp3` | L1 | 1 | ~1:30 | Main input |

Paths are lowercase, hyphenated, zero-padded. `uNN-lNN-<slug>` — the unit, the
lesson, and a short Italian slug (`messaggio`, `dialogo`, `ritratto`).

### Each cue

Six things, every time:

1. **Header** — cue number, asset path, length target, lesson and stage it
   serves.
2. **Speakers** — name, age bracket, region, and whether the accent is
   standard. Regional spread across the course is the Italian Content Editor's
   call; the script states the intention so they can correct it.
3. **Pace** — `normal` (≈140 wpm at A2, ≈160 from B1), `slow` for a first
   encounter, or `natural` where the point of the recording is that it is fast.
   Where a lesson needs two speeds, that is **two takes of one cue**, not two
   cues.
4. **What this recording must contain** — the checklist from the unit overview:
   target structures, lexis items, receptive seeds. A recording that misses a
   seeded chunk breaks a later unit, and it is cheap to check here and expensive
   to check after recording.
5. **The script**, with paragraph numbers for timestamped re-listening, and
   **intonation contours marked only where they carry meaning** — a rising
   question that has no question word, an incredulous echo, a list that is not
   finished. Marking every contour is noise; marking the meaning-bearing ones is
   the point of writing scripts instead of just texts.
6. **Notes to the voice talent** — the two or three things that will be got
   wrong if not said. Usually: don't over-enunciate the doubles, don't slow down
   at the end, leave the pause where it is marked.

### Marking conventions

| Mark | Means |
| --- | --- |
| `↗` | rising contour, on the syllable that follows |
| `↘` | falling contour |
| `→` | level / suspended, list not finished |
| `//` | pause, ~1 second |
| `///` | pause, ~2 seconds (gap for a learner to answer) |
| **bold** | contrastive stress |
| `[...]` | stage direction to the voice talent, not read aloud |

---

## Filled example (Unit 1, cue 1)

### Cue 1 — `assets/audio/unit-01/u01-l01-messaggio.mp3`

**Serves.** L1 stages 4, 5, 6. **Length target** 1:20–1:35.
**Speakers.** Giulia, 30s, Bologna, standard with a light northern colour.
**Pace.** Two takes: `normal` for stages 4–5, `slow` for stage 6.
**Must contain.** All 11 reflexive routine verbs · ≥6 present-tense irregulars ·
one reciprocal (`ci vediamo`) · **no** `piacere` chunks (they are seeded in L3;
putting them here would spend the seed a lesson early).

**Script** `[ITA?]`

> **[1]** Ciao Mark! Sono Giulia. // Allora, mi hai chiesto com'è la mia
> settimana↗ // Ti racconto. ///
>
> **[2]** Durante la settimana mi sveglio alle sei e mezza, ma non mi alzo
> **subito**: resto a letto dieci minuti. // Poi mi faccio la doccia, mi vesto →
> e faccio colazione in piedi, in cucina. ↘

**Notes to voice talent.** [1] The `com'è la mia settimana↗` rises because she
is quoting his question back, not asking her own — if it falls it sounds like she
is asking him. [2] `subito` takes contrastive stress; the whole point of the
sentence is the gap between waking and getting up. Keep the list contour level
on `mi vesto` — she has not finished listing yet.
