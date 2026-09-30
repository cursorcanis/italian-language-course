# Shape Review — A2→B1 Syllabus Map and Companions

Reviewer: Chief Italian Linguist · Task: ITA-7 · Date: 2026-09-30
Reviewing: `curriculum/syllabus/a2-b1-syllabus-map.md`,
`grammar-progression.md`, `lexis-progression.md` at commits `7de5160`,
`55879bd`, `c1de2b9` (ITA-3, Curriculum Architect).

> **ITA-6 landed during this review,** at commit `3961be5`: the Italian passes,
> with one orthographic fix (`Le confermo`) and one substantive change to Set 6
> (below). Every finding in this document was re-verified against `3961be5` and
> all three defects survive it unchanged. The editor's commit also swept this
> file in with `git add -A`, so the review's own history sits under that commit
> rather than its own — noted, not worth rewriting.

---

## Verdict

**Accepted.** ITA-3 is closed. The grid is the spine of the course and it holds.
Three documentation defects are listed below; none of them changes a design
decision, and all three are prose fixes.

The thing that makes this deliverable unusually strong is that its claims are
*located* rather than asserted — `U7 L4`, not "later in the course". That is
what made the review below possible at all, and it is the property downstream
work should preserve.

---

## What I re-verified independently

Every check below was re-run from the files rather than taken from ITA-3's
summary.

| Claim | Method | Result |
| --- | --- | --- |
| Every internal link and anchor across the three documents resolves | Reimplemented GitHub's heading slugger; resolved all relative links | **0 failures** |
| Every lexis set is exactly 30 | Parsed all 36 subgroup tables; compared declared count to actual rows | **12/12 at 30**, every subgroup matches its declared figure |
| The map's quoted subgroup figures match the lexis document | Compared per unit | **12/12 match** |
| Stated spacing figures are the arithmetic of the located encounters | Computed `recycle − intro`, `free − recycle` from every row | **30/30 correct** |
| No structure is recycled before it is introduced, or freely produced before it is recycled | Ordering check on every row | **30/30 correct** |
| Every located recycle point is named in the per-unit `L4` contract | Keyword-matched each master-table recycle point against its unit's contract row | **28/28 resolve** |
| Exactly one main grammar point per unit | Parsed the grid and all twelve unit sections | **12/12** |

So the checkable claims are, with the three exceptions below, actually true.
That is rare enough to say out loud.

---

## Defect 1 — count drift in `grammar-progression.md`

Three stated numbers are each off by one:

| Stated | Actual |
| --- | --- |
| "Twenty-nine structures" (master table) | **30 rows** |
| "Seventeen of the twenty-nine structures have both intervals at two units or more" | **18** |
| "eleven widen or hold flat" | **12** |

All three are consistent with a single row — **Avverbi in `-mente`** (spacing
`2, 2`) — having been added *after* the spacing-audit prose was written. That
matches ITA-3's own note that `U10 L4` was amended late to name the `-mente`
adverbs.

**Fix:** 29 → 30, seventeen → eighteen, eleven → twelve. No design change.

**Why it matters:** this document's entire value is that its claims are
checkable. A reader who counts the table and gets a different number stops
trusting the claims they did not count.

---

## Defect 2 — the map's load check names the wrong units

`a2-b1-syllabus-map.md` §Verification → Load check says:

> Units 1, 2, 3, 4 and 6 carry a main point that is **consolidation** of A2
> material, and are the only units carrying two secondary points.

Against the map's own grid, neither half of that is right:

- **Consolidation mains are U1, U2 and U4 only.** U3's main is *pronomi
  relativi `che`/`cui`* **(new)**; U6's is *pronomi diretti + `ne`* **(new)**.
  §2 of the same document already says "Units 1, 2 and 4" — so the two sections
  contradict each other.
- **Two secondary points appear in seven units,** not five: U2, U3, U5, U7, U8,
  U10, U12. Single secondary points: U1, U4, U6, U9, U11.

The claim that has to survive — *exactly one main grammar point per unit* — is
true, 12 out of 12. But the wrong list conceals the load picture the Lesson
Designer actually needs:

**The four units where one-heavy-point-per-unit is under real strain are U5, U7,
U8 and U12** — each carries a *new heavy* main point **plus two** secondary
points. U7 is the sharpest case: imperativo across four persons, affirmative and
negative, with clitic attachment, *plus* `si` passivante, *plus* prepositions of
movement, in five lessons. U12 is the second: congiuntivo presente plus
argumentative connectives plus concession, in the last unit of the course.

**Fix:** correct the list, and name U5, U7, U8 and U12 as the four units to
stage most carefully. This is a note to ITA-5, not a re-sequencing.

---

## Defect 3 — the false-friend strand is counted as outside the thirty, but sits inside it

`lexis-progression.md` states twice that the twelve false-friend items "sit
**outside** the thirty", and the coverage check lists *Productive items 360* and
*False-friend strand 12* as separate rows — which reads as 372 taught items.

Checked all twelve against their unit's own subgroup tables: **eleven of the
twelve are members of their unit's 30.** `i parenti` is in Set 1's people
subgroup, `la patente` in Set 7's offices subgroup, `attualmente` in Set 12's
connectives subgroup, and so on. The one genuine exception is
`i preservativi`, and only since `3961be5` — ITA-6 moved `i conservanti` into
the Set 6 production slot and left `i preservativi` in the strand table as a
written recognition note. So the "outside the thirty" claim describes exactly
one of the twelve items it covers.

Inside is the better design for the other eleven — one item doing two jobs beats
an extra item per unit — so the fix is the prose, not the sets.

**Fix:** "woven into the thirty and tagged as strand items, with one exception
(`i preservativi`, recognition-only)", and a coverage check that reads 360 total
plus one, eleven of the 360 carrying a strand tag.

**Why it matters:** ITA-5 sizes glossaries and ITA-4 sizes checkpoints off these
figures. "Thirty plus one" sends a designer hunting for a thirty-first item that
does not exist.

---

## A mitigation both documents are missing — and it is the strongest one available

Unit 7 teaches `mi dica`, `si accomodi`, `scusi`, `senta` as lexical
imperatives, and the map is explicit that they are taught "not as a first
congiuntivo". That is the right call for U7.

But those forms **are** congiuntivo presente, third person singular — and the
learner *produces* them from U7 to the end of the course. By `U12 L2`,
congiuntivo morphology is not cold. It has been in the learner's mouth for five
units, in the one place an anglophone uses it without noticing.

Neither document uses this. `grammar-progression.md` Seed 2 seeds only the
opinion-verb chunks (`penso che sia`, `spero che vada`), which seed the
*function*. The `Lei` imperatives seed the *form* — and do it **productively**,
which is stronger than every receptive seed in the course.

Two changes follow:

1. Add the `Lei` imperative set as a **fourth strand** in §Receptive seeding,
   flagged as *productive form-seeding*, U7 → U12.
2. Make `U12 L2` open by exploiting it — *you have been saying `mi dica` since
   Unit 7; here is what it actually is* — rather than presenting congiuntivo
   cold.

This is also the honest reason the twelve-unit container survives. See below.

---

## Decision 1 — twelve units or fourteen: **hold twelve**, escalated for ratification

Recommendation: **twelve.** Escalated to the board because this fixes the
product's advertised length (~90 guided hours, 7–8 months) and because
reaffirming it is a decision about `docs/format-brief.md` (ITA-2), which is mine
to bring and the board's to settle.

The architect's statement of the problem is correct and I am not softening it:
seven structures reach free production only at Milestone 2, and congiuntivo
presente and the connettivi argomentativi get two encounters rather than three.
The spiral is a *load-bearing* assumption behind the brief's ~90 guided hours
against a published 150–200, and it visibly thins in the last quarter.

Four reasons I still hold twelve:

1. **The shortfall lands where the course has already capped its claim.**
   Congiuntivo at B1 is a first look — recognition plus supported production
   after a closed set of opinion verbs — and the B1 descriptors do not ask for
   it as a system. Connettivi argomentativi are assessed for cohesion, not
   accuracy. A third encounter buys movement toward mastery; we are not claiming
   mastery of either. Fifteen guided hours to widen spacing on the two
   structures we have deliberately capped is buying the wrong thing.
2. **Congiuntivo's form is not cold at U12** — the `Lei`-imperative point above.
   That turns "two encounters" into *five units of productive form exposure,
   seven of receptive function exposure, then two analytical encounters*. A
   materially different and far more defensible object.
3. **The connettivi shortfall is soft.** They are an extension of the U5
   narrative connectives, which have a full three-encounter spiral, and they are
   taught explicitly *against* them (`però` → `tuttavia`, `così` → `quindi`). A
   learner meeting them at U12 is re-registering a strand they already own, not
   learning a structure from nothing.
4. **The brief already names the trigger for going longer, and it is data.**
   ITA-2 §3: *"If the placement check shows real learners entering weaker than
   assumed, the honest fix is more units."* Fourteen units is the right response
   to evidence — weak entry, or milestone data showing the tail failing. It is a
   heavy response to a spacing principle applied a priori.

**What holding twelve costs, stated plainly:** the late structures will be
weaker at the end of the course than the front-half structures, and Milestone 2
carries structural weight rather than only assessment weight. That cost is real
and ITA-4 inherits it.

Three conditions, not decorative:

- **Milestone 2 must *elicit*, not permit,** the seven tail structures.
  `grammar-progression.md` §What this hands to ITA-4 is binding on ITA-4.
- **Unit 12's `L4` stays a whole-course recycling lesson.** The moment it becomes
  congiuntivo practice, the argument above collapses. The architect is right
  that densifying Unit 12 is not an alternative to fourteen units — it trades
  cognitive load for distributed practice at a net loss.
- **The placement check ships before Unit 1 is taught,** and its results come
  back to me. It is what makes the ~90-hour figure falsifiable rather than
  optimistic, and it is the trigger for reopening this decision.

If the board prefers fourteen, now is the moment: today it is one document
revision. After ITA-5 ships a template and ITA-4 builds the milestones, it is a
re-plan of the entire back half.

---

## Decision 2 — ITA-5 starts now, with one constraint

**Yes.** The grid is stable, and lesson staging does not depend on the Italian
wording still in vetting. Three things bind:

1. **The sample unit must come from Units 1–6.** This makes ITA-5 safe under
   either answer to the container question: the front half of a twelve- and a
   fourteen-unit course is identical, and only the tail re-spaces.
2. **No Italian from these documents is typeset into learner-facing material**
   until ITA-6 signs it off. Where the template needs Italian, mark it
   provisional.
3. **The per-unit `L4` contract is binding.** `L4` re-works *named earlier*
   structures; it is not extra practice of the current unit's point. And see
   Defect 2: U5, U7, U8 and U12 are the units where the 90-minute staging will
   be tightest.

---

## Decision 3 — Unit 7's bureaucracy subgroup: keep it, unchanged

Right for this product, and the assumption it makes is the brief's assumption,
not a smuggled one. Format brief §1 fixes the learner as an adult anglophone
learning Italian "for life reasons — work, family, living in or travelling to
Italy."

It also assumes less residency than the question implies. Of the eleven items in
subgroup C, only **two** are residency-specific — `la residenza` and
`l'ufficio anagrafe`. The other nine (`lo sportello`, `il modulo`, `compilare`,
`la marca da bollo`, `la fila`/`la coda`, `il numeretto`, `l'appuntamento`,
`la tessera sanitaria`, `la patente`) serve a visitor or a long-stay traveller
just as well.

Payoff over frequency is the correct trade here, and subgroup A shows it paying
off immediately: `obliterare` on the sign versus `timbrare` in people's mouths
is exactly the distinction a frequency list misses and a €50 fine teaches.

One small addition: keep an explicit note that `la residenza` and
`l'ufficio anagrafe` are for the resident case, so a self-study learner who is
only visiting knows why they are in the set.

---

## Decision 4 — sequencing departures from the brief's list: approved in full

All seven additions (§3) and all five reorderings (§4) are approved. Three worth
singling out:

- **Pronomi combinati at U9, before futuro and condizionale.** The best
  sequencing call in the document. Combinati depend on direct (U6) and indirect
  (U8) pronouns and on no tense at all, so following textbook order would place
  them at U11–12 with nowhere left to recycle them. Prerequisite freshness over
  inherited order is the right instinct, and it is the reason the U8→U9 interval
  of one unit is acceptable rather than sloppy.
- **Futuro (U10) before condizionale (U11), on the shared irregular stems.**
  Correct, and worth stating in the learner-facing material too: the conditional
  then costs a set of endings rather than a second set of stems.
- **Imperativo at U7 as the home for clitic attachment.** Approved, and it earns
  more than the map claims for it — it is also the course's productive seed for
  congiuntivo morphology (above).

**`si` impersonale early at U4** is approved with a note: the riflessivi clash
is handled by distance and by addressing it head-on at `U4 L3`, which is right,
but `U4 L3` is also where the map puts the unit's secondary point. The Lesson
Designer should not let the clash discussion get compressed out of that slot —
it is the whole reason the early placement is safe.

---

## What this hands on

| To | What |
| --- | --- |
| **Curriculum Architect** | Defects 1–3 and the `Lei`-imperative strand, applied in one pass together with ITA-6's returns (follow-up issue). Then ITA-4, under the three conditions in Decision 1. |
| **Lesson Designer** | ITA-5 unblocked, sample unit from U1–U6, `L4` contract binding, U5/U7/U8/U12 staged most carefully. |
| **Italian Content Editor** | ITA-6 done and accepted. `i preservativi` settled below. |
| **Board** | Ratify twelve units, or choose fourteen. |

**`i preservativi` (U6 false-friend strand)** — owned by me per
`lexis-progression.md`. ITA-6's resolution stands: `i conservanti` takes the
Set 6 production slot, `i preservativi` stays in the strand table as a written
recognition item, never in dialogue or audio. That is the better answer than
either of the two the question offered. The item belongs in the course — it is a
high-cost false friend and the product is for adults (brief §1: 18+), so
dropping it to spare a self-study learner's blushes would be squeamishness
dressed as editorial judgement. But the *production* slot in a market-stall
lexis set is the wrong home for it, and `i conservanti` earns that slot on its
own merits: `senza conservanti` is on every Italian food label. Recognition
where recognition is what's needed, production where production pays. Closed.
