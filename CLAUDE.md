# Hibiscus Court Reports — Working Instructions (canonical, versioned copy)

> **What this file is.** This is the versioned master of the **workspace `CLAUDE.md`** for the Hibiscus drafting team. The live copy lives at the root of the Cowork working folder (the Drive-mounted `Hibiscus Court Reports/` folder) so it **auto-loads at the start of every session** — Cowork skills have no session-start hook, so the standing rules ride in through this file instead. Keep this copy and the workspace copy in sync; when the rules change, update `kate-rules.md`, this file, and the workspace `CLAUDE.md` together. For anyone working on the plugin itself: these are the rules the skills must enforce.

This folder is the shared workspace for drafting the court-appointed monitor's compliance report for the New Jersey Veterans Homes under the federal Consent Decree. Everyone on the monitoring team works here in Cowork. These instructions govern every drafting session.

## Read first, every session
- **Kate's standing rules below** — non-negotiable; they override any older guidance (including the playbook) where they conflict.
- **`00-instructions/HIBISCUS-REPORT-PLAYBOOK.md`** — the rulebook. Follow it for voice, structure, anonymization, determinations, and the NOTES-to-the-monitor convention.
- **`00-instructions/gold-standard-sections.md`** — annotated real sections showing exactly what an excellent section looks like. Before drafting a care area, study the exemplar closest in shape, match its register and structure, and fill it with the facts from the source file. (Ordering is now concerns-first / positives-last — see rule 6.)
- The `hibiscus-reporting` plugin's **`kate-rules.md`** holds the full rule detail and the complete banned-phrases table with replacements.

## Kate's standing rules — ALWAYS ON

These are the monitor's non-negotiable rules. Follow every one in every draft without being asked — they are the corrections that kept recurring between sessions. The skills enforce them; `kate-rules.md` has the full detail.

**Hard rules**
1. **No specific unit/wing names in prose** — use "the facility," "the unit," "one unit." A specific unit name may appear only in the NOTES crosswalk, tied to a citation.
2. **Month and year only in prose** ("during the March 2026 observation"). Exact day/month/year dates appear only in the NOTES crosswalk.
3. **DVA, never DMAVA.**
4. **Do not re-expand the pre-defined acronyms** — use the abbreviation only: **ACEO, DON, LPN, EMR, TAR, DVA, CMS, CFR.** (Other terms of art — SBAR, MDS, Braden Scale, QAPI, PBJ, Facility Assessment — still get a brief first-use definition.)
5. **POS = physician order set** — never "physician order summary," never "point of service."
6. **Concerns first, positive findings LAST** in every paragraph block. Problem, then credit — never lead with the positive.
7. **Generalize medications and lab values** — "multiple cardiac medications," "worsening" — unless the exact medication or value is the direct subject of the finding.
8. **No consequence-editorializing (P0)** — state the finding and stop. If the last sentence of a block can be deleted without losing a factual finding, delete it.
9. **Exclude resolved observations** — the **MDS missed-hospitalization observation** is not drafted into any section (see the exclusions list in `kate-rules.md`).
10. **Translate clinical shorthand** — "query" → "recommended evaluation for"; name the actual visit pattern, never "across early visits."
11. **"Not observed," never "unprecedented."**

**Voice guards** — suppress on sight:
- **Editorializing / wrap-up sentences** that draw a conclusion or speculate about downstream harm. The report states findings and stops.
- **Attribution voice** — wording that brands staff incompetent or negligent. Critique the documentation, system, or process, not the person.
- **Escalation language** — "more concerning," "systemic gap," "breadth of undocumented omissions," "unprecedented," "egregious," "alarming." Use the specific count or extent instead, or delete.
- **Floor:** never soften a serious patient-safety or resident-dignity finding into vagueness — those stay plain and grave.

**Banned phrases** — never use; replace:
- "it is important to note that" → delete; start with the finding
- "this suggests" / "this raises concerns about" / "this pattern indicates" → state the finding, then stop
- "raises questions about whether" → state the finding directly
- "systemic gap" / "more concerning" / "breadth of undocumented omissions" → describe the specific finding
- "unprecedented" → "not observed" / "not documented"
- "we will continue to monitor" → delete unless the framework requires it
- "no bright spots were identified during that observation" → omit
- "across early visits" → the actual observation pattern
- "query hospital transfer" → "recommended evaluation for hospital transfer"
- "DMAVA" → "DVA"  ·  "physician order summary" → "physician order set"

**After every file edit**, confirm plainly: `Applied: [change] in [file]. Lines [X–Y] modified.` (or `Proposed (not yet applied):`). Treat any `[Kate:]` annotation in a source file as a binding instruction.

## Use the installed skills
The `hibiscus-reporting` plugin provides the skills. Use them:
- **obs-inventory** — build the ranked evidence inventory + coverage map for a care area before drafting.
- **section-writer** — draft one care-area section.
- **voice-check** — check a draft against the team's voice and Kate's standing rules before finalizing.
- **baseline-comparison** — weave Baseline Report comparisons inline, sparingly.
- **exec-summary-writer** — the front matter (Executive Summary, Implementation, Introductions), written LAST.
- **format-cleanup** — assemble + format the finished report, strip the NOTES blocks.
- **obs-lookup** — trace an observation by Record # / obs ID.
- **session-handoff** — at session start load the rules + latest handoff; at session end write the handoff doc.

## The folder
- `01-reference/` — the two prior filed reports (voice/structure/grade-continuity model — NOT a source of current facts; our evidence is a later period), the verbatim Consent Decree paragraphs, and the lookup CSVs.
- `02-source-evidence/<facility>/<NN>-<care-area>.md` — **the drafting source of truth.** Full names-removed observation detail for one facility + care area. Each observation carries a `Record # | obs ID`. This is what you draft from.
- `03-drafts/<facility>/` — work in progress.
- `04-final/<facility>/` — reconciled, file-ready sections and the assembled report.

## The drafting workflow
1. Pick a care area + facility. Read its source file, e.g. `02-source-evidence/menlo-park/06-falls.md`.
2. (Optional) Run **obs-inventory** to build the ranked inventory + coverage map, then annotate it in Google Docs with the `[Kate:]` prefix.
3. Run **section-writer** to draft that section from the source file. Output is clean filing prose, then a fenced `— NOTES TO THE MONITOR (delete before filing) —` block.
4. Run **voice-check** on the draft.
5. Save the result to `03-drafts/<facility>/<NN>-<care-area>.md`.
6. A monitor does the **reconciliation pass** (see below).
7. Move the reconciled, NOTES-stripped section to `04-final/<facility>/`.
8. When all sections of a facility are final: **exec-summary-writer** for that facility's front matter, then **format-cleanup** to assemble.

## Non-negotiable rules (the rulebook has the detail)
- **Draw only from the source file.** Never invent a fact, number, date, quote, or name. Every finding must trace to an observation in that file — and to the source-observation crosswalk you put in the NOTES block.
- **No PHI.** Source files have patient names removed ([RESIDENT] placeholders). Residents stay anonymous in prose; staff are referenced by role; never write a real patient name anywhere in this folder.
- **The NOTES fence is absolute.** Prose above `— NOTES TO THE MONITOR (delete before filing) —` is clean, file-ready text — no observation IDs, no `[DATA NEEDED]` tags, no grade rationale. All of that, plus the source-observation crosswalk, goes below the fence.
- **Determinations are proposals.** The Compliance Determination table is the AI's proposal, anchored to current findings + the prior period's grade. The monitors confirm or change every grade. Never assert a grade the NOTES flag as uncertain.
- **Data that isn't in the observations** (CMS MDS Quality Measure %, PBJ staffing tables, Emergency-Plan inventories, audit %) lives in the team's other documents — flag the specific need in NOTES; never invent the figure.

## The monitor reconciliation pass (a draft is a FIRST draft, not a filing)
For each drafted section, a monitor must: read the NOTES block; verify each finding against the source-observation crosswalk; fill in the external data the NOTES flag; confirm or correct every compliance grade; then delete the NOTES block. What remains is the filing text.
