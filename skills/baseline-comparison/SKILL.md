---
name: baseline-comparison
description: >-
  Strengthens a drafted care-area section of the court-monitoring report by weaving Baseline Report
  comparisons INLINE into the existing narrative — never as an appended block — and only where the
  source documents a genuine then-vs-now story (clear progress or clear persistence). Both halves must
  be sourced: the baseline finding from the Baseline Report, the current finding from the care-area
  source file. Adds baseline context only; never alters findings, evidence, or Compliance
  Determinations. Marks each inline addition so the monitor sees exactly what was added, and keeps all
  drafting aids below the NOTES-TO-THE-MONITOR fence. Use when a monitor asks to add a baseline
  comparison, weave the Baseline into a section, check a draft against the Baseline Report, or verify
  whether an issue was already documented at baseline.
---

# Baseline Comparison

You weave **Baseline Report** comparisons into a drafted care-area section. In the team's filed reports, baseline references appear INLINE at natural points in the narrative — the spine of the then-vs-now story — never as an appended "Comparison to Baseline" block at the end of a section.

This skill does **one narrow thing**: it adds baseline context. It does not draft new findings, change evidence, or set grades. Everything it adds must be sourced on both halves, and every addition is marked so the monitor sees exactly what changed.

---

## 0. Your inputs

You are given:

1. **The drafted section** — from `section-writer` or pasted by the user. This carries the current-window findings, the `Compliance Determination:` paragraph, the status table, and (if present) a `— NOTES TO THE MONITOR (delete before filing) —` fence.
2. **The care-area source file** (`02-source-evidence/<facility>/<NN>-<care-area>.md` on the mounted Drive; attached per-draft in the claude.ai project) — the full names-removed observation detail for this one facility and care area, with a `Record # | obs ID` per observation. This is the ONLY source for the **current** half of any comparison.
3. **The Baseline Report** (June 2025) — in project knowledge. This is the ONLY source for the **baseline** (prior-state) half of any comparison. Read the corresponding care-area portion in full before touching the draft. If the Baseline Report is not available, STOP and ask for it. **Never reconstruct baseline findings from memory.**

The **12-Month Report is NOT a baseline source.** It is a later filed report used elsewhere only for voice, structure, density, and prior-period grade continuity. The current evidence covers a still-later window (months 13–19; Nov 2025–May 2026), so current facts legitimately differ from the 12-Month Report — that is expected, not an error. For prior STATE, the comparison anchor is the **Baseline Report**, not the 12-Month Report.

---

## 1. Both halves sourced — the first rule

A baseline comparison is two claims joined: *what the Baseline Report documented* and *what the source file shows now*. **Write a comparison only when you can ground both halves.**

- The baseline half traces to the Baseline Report's treatment of this care area — quoted or closely paraphrased.
- The current half traces to an item in the care-area source file.

If the Baseline Report did not address a topic, do not manufacture a comparison — **silence is acceptable and often correct.** If the source file does not document the current state of a baseline concern, do not assert progress, persistence, or resolution; flag the gap in NOTES instead. A plausible-sounding then-vs-now sentence with only one half sourced is a fabrication.

---

## 2. Be sparing — only where it earns its place

Baseline comparison is **selective, not comprehensive.** Many filed sections never mention the Baseline Report. Do not seed a baseline reference into every paragraph, and never open a section with a Baseline recap by default — sections open with what is true now.

Use a comparison only where the source documents a **genuine then-vs-now story**, in one of three shapes:

- **Progress** — a baseline concern is now improved → supports a paragraph trending toward Substantially Compliant.
- **Persistence** — a baseline concern remains → supports Partially Compliant / Non-Compliant, and puts on the record that the facility had notice.
- **Continuity of strength** — a baseline positive is sustained → supports Substantially Compliant.

Placement is **inside the relevant `Paragraph NN — Topic.` block** — at the natural point in that block's prose, usually where the thread is first stated — not bolted on at the end of the block or the section. (Sections are paragraph-ordered; weave the comparison into the block whose CD paragraph the then-vs-now story belongs to.) The Baseline Report is typically the subject of the sentence, immediately followed by current status from the source. Never add a comparison to a `NO EVIDENCE` placeholder block — those have no current half to compare against.

---

## 3. The inline pattern (the team's filed phrasings)

Match these shapes; fill them with the actual sourced facts for both halves.

> "The Baseline Report identified concerns with [baseline concern, from Baseline Report]. More recent onsite visits showed that [current state, from source file]."

> "The Baseline Report identified concerns with [X]. These concerns persist, though the monitoring team has noted some improvement: [current specifics, from source file]."

> "The Baseline Report documented [system / positive finding]. This system remains in place, and during recent onsite visits the monitoring team confirmed [current continuation, from source file]."

Keep the team's flat declarative voice (per the section-writer rulebook): no essayistic build ("raises questions about," "potentially interferes"), no consequence-editorializing, no external-literature citation, no contractions in the team's own prose. The comparison states the then and the now and stops.

---

## 4. Process

1. **Read the Baseline Report's treatment of this care area in full.** List its specific concerns and its positive findings, in the Baseline Report's own language.
2. **Map each against the draft's current findings** (which trace to the source file): progressed / persisted / regressed / resolved / new-since-baseline.
3. **Select the few that carry a genuine, both-halves-sourced story** (§1–§2). Discard the rest — including baseline topics the source file is silent on this window (those become NOTES, not prose).
4. **Weave each selected comparison into the existing paragraph at its natural point**, using the team's phrasing (§3). Quote or closely paraphrase the baseline language so the continuity is on the record. Do not restructure the draft or move findings around.
5. **Mark every inline addition** so the monitor sees exactly what was added — see §5.
6. **Record the rest in NOTES** — baseline topics with no current evidence, any tension a comparison surfaces, and your sourcing for each woven half — below the fence (§6).

---

## 5. Marking additions without dirtying the filed prose

The monitor must be able to see what you added **and** still copy clean text into the filing. Reconcile these by keeping the marks **out of the prose itself**:

- Leave the woven sentences as clean, file-ready prose in the section body — no inline highlight tags, no `[ADDED]` brackets, no track-changes cruft in the paragraph.
- In the NOTES block, list each addition under a **"Baseline comparisons woven in"** heading: quote the exact sentence you inserted, name the paragraph/sub-topic it now sits in, and give the two sources (Baseline Report location for the prior half, source-file item for the current half). The monitor reads the list, verifies, then deletes the NOTES block — and the prose above the fence is already clean.

This is the only acceptable way to "mark" additions: visible to the monitor in NOTES, invisible (because clean) in the filed prose. Do not introduce inline scaffolding above the fence.

---

## 6. NOTES TO THE MONITOR — the single fence

All drafting aids live in ONE fenced block at the very end of the section, after the table, labeled exactly:

```
— NOTES TO THE MONITOR (delete before filing) —
```

The drafted section you are editing already carries this fenced block in the section-writer's sectioned format, with eight named subsections (PURPOSE OF THIS SECTION; DETERMINATION RATIONALE; PRIOR-PERIOD GRADE CONTINUITY; MISSING / EXTERNAL DATA TO SUPPLY; SCOPE / OVERLAP NOTES; ANONYMIZATION CONFIRMED; SOURCE-OBSERVATION CROSSWALK; RECONCILIATION QUESTIONS). **Do not create a second fence and do not reorder those subsections.** Fold your baseline work into the existing block:

- Record every woven comparison under a clearly labeled **"Baseline comparisons woven in"** entry placed with the **PRIOR-PERIOD GRADE CONTINUITY** material (to which it is most closely related): quote each sentence you inserted, name the `Paragraph NN` block it now sits in, and give both sources — the Baseline Report location for the prior half and the source-file `Record #/obs ID` for the current half.
- Put baseline topics the source file is silent on this window under **MISSING / EXTERNAL DATA TO SUPPLY**, or as an open item under **RECONCILIATION QUESTIONS** — never as prose.
- Add any source-file observation you newly relied on to the existing **SOURCE-OBSERVATION CROSSWALK**.

Everything above the fence stays clean, file-ready prose — no inline markup, no `[ADDED]` brackets, no observation IDs. The fence label must be exactly `— NOTES TO THE MONITOR (delete before filing) —`. If the draft you were handed has no NOTES block at all, add one in the section-writer's sectioned format rather than inventing a different structure.
