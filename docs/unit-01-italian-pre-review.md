# Unit 1 — Italian pre-review

**Reviewer:** Italian Content Editor · **Issue:** ITA-10 (Italian sign-off for
Unit 1) · **Date:** 2026-10-02 · **Branch:** `main`

---

## Why this document exists

ITA-10 asks me to sign off the Italian in `curriculum/units/unit-01/`. **That
directory does not exist yet** — on `main` at `47d7cca`, or in the working tree.
The unit template is being drafted in parallel under ITA-5 and is still
uncommitted. There is nothing to sign off, so ITA-10's verdict is deferred.

What *does* exist is the **specification Unit 1 will be written from**: the
pronunciation point and lexis set in `curriculum/syllabus/a2-b1-syllabus-map.md`
and `curriculum/syllabus/lexis-progression.md`, and the Unit 1 *filled examples*
in the in-flight template. Those specs contain Italian defects that would be
copied straight into Unit 1 — including into the audio script, which is the most
expensive file in the project to rework once recorded.

So this is a pre-review: fix these before Unit 1 is written, not after I review
it. **Required fix** = an error. **Suggestion** = a preference; keep your version
if you disagree.

I have deliberately **not** edited the template in place. It is uncommitted and
held by a live concurrent run; a surgical edit would be silently lost on the next
whole-file write, and committing another agent's unfinished draft is not mine to
do. Everything below carries exact replacement text instead.

---

## 1. The minimal pairs — two of the four are invalid

Current spec (`unit-template/unit-NN-overview.md` §5, filled example):

> Meaning-bearing pairs: `pàrlano` / `parlerànno`, `àbito` / `abìto`,
> `càpito` / `capitò`, `àncora` / `ancòra`.

### Required fix 1.1 — `abìto` is not an Italian word

`abito` has exactly one pronunciation: **`àbito`** (the noun *suit, outfit*; also
*abitare* 1sg *I live*). There is no `abìto`. The pair as written asks a learner
to produce a non-word and tells them it means something.

The intended contrast was presumably `àbito` / `abitò`. Do not use it — see 1.2.

**Replace with `pàpa` / `papà`** — *the Pope* / *dad*. Both A1-frequency, both
real, differing in stress alone, and it does double duty with the final-stress
bullet below. This is the single best stress pair in the language for this level.

### Required fix 1.2 — `capitò` is passato remoto, which this course never teaches

`grammar-progression.md` §Deferred is explicit: passato remoto has "near-zero
spoken payoff", is seeded as **recognition only in U12**, and is **never
produced**. A Unit 1 pronunciation drill that has learners *say* `capitò` — and
`abitò`, under the discarded 1.1 reading — contradicts that in the course's first
unit.

**Replace with `càpito` / `capìto`**: *capitare* 1sg (*I turn up, I happen by*)
vs the participle of *capire* (*understood*). A true minimal pair, both members
real, and the second is the chunk every learner already says — `Ho capìto`.

Level note, stated rather than hidden: `capìto` is passato prossimo morphology,
which is `U2 L2`. In the fixed chunk `Ho capito` it is pre-A2 and safe. Gloss it
as the chunk, not as a tense. This is a one-unit forward reach on a formula
learners arrive with; `capitò` is a ten-unit reach on a tense they will never be
taught to produce.

### Required fix 1.3 — `pàrlano` / `parlerànno` is not a minimal pair

Four syllables against five, single `n` against double, present against future.
It differs in more than stress, so it cannot demonstrate that stress alone
carries meaning. It is also `futuro semplice`, which is `U10 L2` — nine units
away.

**Delete it.** It is redundant anyway: the `-ano` bullet directly above already
makes the 3pl point correctly, and makes it better. Mis-stressing `pàrlano`
produces **\*parlàno**, a non-word — so that point is a *production* contrast
against a non-word, not a minimal pair, and the file should say so. Listing it
under "meaning-bearing pairs" miscategorises the one thing in the section that is
most worth getting right.

### Suggestion 1.4 — optional fourth pair

`i prìncipi` (*princes*) / `i princìpi` (*principles*). Genuine, no verb
morphology at all. Offered rather than required: `princìpi` is abstract for A2
and earns its place only if L3 has room. Three pairs that work beat four with a
passenger.

### Resulting pair set

| Pair | Gloss | Why it holds |
| --- | --- | --- |
| `àncora` / `ancóra` | anchor / still, again | Both high-frequency, both A2, no morphology. Unchanged — this one was always right. |
| `pàpa` / `papà` | the Pope / dad | A1 both sides; also carries the final-stress point. |
| `càpito` / `capìto` | I turn up / understood | Highest payoff: `Ho capito` is already in the learner's mouth. |
| *(optional)* `prìncipi` / `princìpi` | princes / principles | Suggestion only. |

---

## 2. Accents — `svègliano` is wrong, and the convention is unstated

### Required fix 2.1 — `svègliano` → `svégliano`

The stressed vowel in *svegliare* / *la sveglia* is **closed `é`**: `svéglia`,
`svégliano`. The template writes `svègliano` with an open `è`.

Two other sources already have it right — `a2-b1-syllabus-map.md:279` writes
`svégliano`, and so does the ITA-10 brief. The template is the outlier.

`àbitano` and `telèfonano` are both correct as written (*telèfono* does take an
open `è`); no change there.

### Required fix 2.2 — `ancòra` → `ancóra`

The adverb takes a **closed `ó`** (< *hanc hōram*, the same `ó` as in *óra*).
`àncora` the anchor is correct.

### Required fix 2.3 — state what the accents mean

This matters more than 2.1 and 2.2 and it propagates to eleven more units. The
spec silently mixes two different kinds of accent:

- **Obligatory spelling**, on final syllables: `caffè`, `perché`, `città`,
  `papà`, `capitò`. Written always, by every Italian, in every text.
- **A didactic reading aid**, on non-final syllables: `àbito`, `àncora`,
  `telèfonano`, `svégliano`. **Never written in normal Italian.**

An A2 learner shown `àbito` with no note will conclude that is how the word is
spelled, and will write it that way for a year. Add one line to §5, and repeat it
wherever stress marks appear in the lesson files and the audio script:

> Accents on a non-final syllable (`àbito`, `svégliano`) are a reading aid for
> this exercise and are never written in ordinary Italian. Accents on a final
> syllable (`caffè`, `perché`, `papà`) are part of the spelling and are always
> written.

Once that note exists, the didactic marks should still reflect real vowel quality
(hence 2.1 and 2.2) — the learner will hear the quality on the recording whatever
the page says.

---

## 3. The final-stress bullet is mislabelled and reaches into U10

Current:

> Truncated infinitives and futures (`caffè`, `perché`, `farò`), stressed final.

Two problems. `caffè` is a noun and `perché` a conjunction — neither is a
truncated infinitive. And `farò` is `futuro semplice`, `U10 L2`.

The category that actually fits all three is **parole tronche**: words with
obligatory final stress. Truncated infinitives (`andar via`, `far finta`) are a
real and separate phenomenon, worth its own slot in a later unit, not a label for
these examples.

**Required fix 3.1 — relabel and re-exemplify:**

> **Parole tronche** — words with obligatory final stress, where the written
> accent is part of the spelling: `caffè`, `perché`, `città`, `però`, `così`,
> `papà`, `lunedì`.

All seven are A1–A2 and high-frequency. `farò` is dropped: a learner who asks
what it means has to be told about a tense nine units away.

**For the Chief:** `a2-b1-syllabus-map.md:279-280` carries the same wording
("truncated infinitives/futures") and is the source of the defect. That file is
under concurrent edit on ITA-8, so I have not touched it. The map's phrasing
needs the same correction.

---

## 4. Lexis — the filled example drops items the syllabus mandates

In `unit-template/unit-NN-lexis.md`, filled example:

### Required fix 4.1 — Set B is 19 items, not 17

`Set A` 11 + `Set B` 17 = 28. The syllabus set is **30**, split 11 reflexive
verbs + 8 people/relationships + 11 character adjectives. Folding B and C
together gives **19**. The file's own rule two sections up is the right one:
"Counts must total the syllabus's thirty. If your split does not add to thirty,
the split is wrong, not the syllabus."

### Required fix 4.2 — `mi interessa` is missing from the `piacere` seed

The receptive set is **five** chunks: `mi piace / mi piacciono`, `mi interessa`,
`mi serve`, `mi manca`. The template's recognition-only table lists four rows and
has dropped `mi interessa`. ITA-10 names all five as a hard requirement of the L3
input. Add the row.

### Required fix 4.3 — a U7 imperative in a U1 example sentence

> `permaloso` — Mio fratello è un po' permaloso: non scherzare sul lavoro.

`non scherzare` is the **negative `tu` imperative**, which is `U7`. It also reads
oddly: *sul lavoro* is ambiguous between *about his job* and *at work*.

**Replace with:**

> Mio fratello è un po' permaloso: meglio non scherzare sul suo lavoro.

`meglio non + infinitivo` is A2-safe, is what a speaker would actually say here,
and keeps the sentence's point — which is that `permaloso` has a consequence for
how you talk to the person. `un po'` is correct as written: apostrophe, not
accent.

### Passing unchanged

The other example sentences hold and are worth keeping as the model for the
remaining 27:

- *Mi sveglio alle sette meno un quarto.* — natural, and specific rather than
  decorative.
- *Non mi alzo subito: resto a letto dieci minuti.* — says something true about a
  person. This is the bar.
- *Mi faccio la doccia la sera, non la mattina.* — carries the
  reflexive-with-direct-object point without announcing it.
- *Il mio coinquilino è molto disponibile.* — correct; flattest of the five.
- *Vado molto d'accordo con i miei vicini.* — idiomatic.

The `i parenti` / `i genitori` false-friend row is correct. The
recognition-only framing of the `piacere` chunks — "learn it as a phrase, we take
it apart in Unit 8" — is exactly right and should not be softened.

---

## 5. Verdicts

### Files ITA-10 assigns me

| File | Verdict |
| --- | --- |
| `unit-01/unit-01-audio-script.md` | **Not reviewable — does not exist.** |
| `unit-01/unit-01-lesson-01.md` … `-05.md` | **Not reviewable — do not exist.** |
| `unit-01/unit-01-lexis.md` | **Not reviewable — does not exist.** |
| `unit-01/unit-01-checkpoint.md` | **Not reviewable — does not exist.** |
| `unit-01/unit-01-overview.md` | **Not reviewable — does not exist.** |

Nothing is recorded, and ITA-5 does not close, until these come back to me.

### Specs reviewed in their place

| Source | Verdict |
| --- | --- |
| `unit-template/unit-NN-overview.md` §5, Unit 1 pronunciation point | **Fail** — 1.1, 1.2, 1.3, 2.1, 2.2, 2.3, 3.1. Two of four pairs invalid; one non-word. |
| `unit-template/unit-NN-lexis.md`, Unit 1 filled example | **Pass with edits** — 4.1, 4.2, 4.3. Example-sentence quality is good. |
| `syllabus/lexis-progression.md` §Unit 1 | **Pass.** Unchanged from the ITA-6 sign-off at `3961be5`. |
| `syllabus/a2-b1-syllabus-map.md` §Unit 1 | **Pass with one edit** — §3 above, the "truncated infinitives/futures" wording. Chief's, via ITA-8. |

---

## 6. Still owed on ITA-10, once Unit 1 exists

Carried forward so nothing is lost: the `piacere` seed must be in L3 and absent
from the L1 voice message; the two L4 profiles must contrast `tu` and `Lei`
naturally in both directions rather than by substitution; the `A8` error-clinic
items must be wrong in the way an English-L1 learner is actually wrong, and the
unflagged items must really be correct; the `↗ ↘ → // ///` contours and the
~190-word and ~230-word scripts must be checked for speakability at A2 pace; and
every sentence written to satisfy the "must contain" checklist gets read aloud,
with anything that sounds like a list rather than a person handed back for
re-staging.
