# Units

One folder per unit (`unit-01/` … `unit-12/`), plus `unit-template/` — the
skeleton every unit follows:

1. Can-do goals (CEFR-referenced)
2. Input text or dialogue
3. Lexis set (~30 items)
4. Grammar focus
5. Pronunciation / intonation point
6. Culture note
7. Production task
8. Checkpoint

Each unit is five lessons of ~90 minutes. A unit folder holds one file per
lesson plus the unit-level materials (lexis list, checkpoint, teacher notes).

Owners: Lesson Designer (structure and activities), Italian Content Editor
(all Italian-language content).

---

## Start here

| | |
| --- | --- |
| [`unit-template/README.md`](unit-template/README.md) | **Read this first.** What a unit folder contains, the binding `L1`–`L5` slot convention, the lesson file header, the nine things every lesson file must have, the Italian review gate, and the bar for done as a checklist. |
| [`unit-template/activity-repertoire.md`](unit-template/activity-repertoire.md) | The thirteen shared activity formats, referenced by code (`A7`) from every lesson. One shared file — do **not** copy it into a unit folder. |
| [`unit-01/`](unit-01/) | The worked reference implementation of all of it. Read `unit-01-lesson-01.md` for an ESA lesson and `-02.md` for a PPP one. |

To build a new unit: copy the six `unit-NN-*.md` template files into `unit-NN/`,
rename, and fill. Each one carries the **shape** (what goes here and the test it has
to pass) followed by a **filled example** from Unit 1, so the template teaches by
showing rather than describing.

**Eight parts, seven files.** The eight-part skeleton above is a *content* checklist,
not a file list: `unit-NN-overview.md` states all eight and says which lesson carries
each, and the lesson files deliver them.

## Status

| Unit | State |
| --- | --- |
| `unit-template/` | Complete. For review by Chief Italian Linguist — this is the format decision, not just a folder. |
| `unit-01/` | Complete: five lessons, lexis list, checkpoint, audio scripts, teacher notes. **All Italian is draft** and marked `[ITA?]`, pending Italian Content Editor sign-off (ITA-10). |
| `unit-02/` … `unit-12/` | Not started. Blocked on the template being approved — building eleven units against an unapproved format is the expensive way to find out it is wrong. |
