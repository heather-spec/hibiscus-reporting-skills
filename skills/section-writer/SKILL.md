---
name: section-writer
description: >-
  Drafts one care-area section of the court-monitoring report (the federal
  consent-decree compliance report on the state veterans homes) in the team's
  paragraph-ordered standard: the section walks the measure's Consent Decree
  paragraphs in number order, gives each one a labeled block
  ("Paragraph 33 — Assessment and documentation. ...") that synthesizes that
  paragraph's evidence, marks any paragraph with no evidence as a NO EVIDENCE
  placeholder, then closes with the Compliance Determination, the three-row
  status table, and a sectioned NOTES-TO-THE-MONITOR block. Matches the filed
  report's flat declarative voice. Use when a monitor asks to draft, write, or
  revise a single care-area section (e.g. General Medical & Nursing Care,
  Vascular Wounds & Pressure Injuries, Medication Administration, Falls, QAPI,
  Infection Prevention, Staffing, Emergency Operations, Resident Care Plans,
  Changes in Condition, Clinical Care Policies, Oversight of Medical Care,
  Organizational Accountability) for a given facility and reporting period. Also
  use when asked to produce the Compliance Determination paragraph and status
  table for a section, weave a Baseline Report comparison in, or fix a draft
  that "editorializes," "goes into too much detail," "isn't organized by
  paragraph," or "has bracket tags in the prose." Produces ONE section. Do NOT
  use for the Executive Summary, Introduction, or full-report assembly.
---

# Section Writer

You draft a single care-area section of the court-monitoring report so it is **indistinguishable from the team's filed reports**. The reader is a federal court. The author is "the monitoring team." The section is **paragraph-ordered**: it walks the measure's Consent Decree paragraphs in number order, gives each one a labeled, synthesized block, then closes with a `Compliance Determination:` paragraph, a three-row status table, and — after a hard fence — a sectioned NOTES-TO-THE-MONITOR block.

Three failures are equally fatal: a draft that **invents facts the source does not contain**; a draft that **editorializes, argues, or pads** instead of stating findings flatly; and a draft that **buries the section in record-by-record detail** instead of synthesizing each paragraph's evidence. This skill exists to prevent all three.

**Study `gold-standard-sections.md` (bundled with this skill) before drafting.** It is the concrete model — the paragraph-ordered exemplar, the NO EVIDENCE placeholder in action, the sectioned NOTES block, and the voice library. Match its structure, density, and register; fill it with the facts from the source file at hand.

---

## Kate's Rules — read these FIRST, follow them without being asked

These are the monitor's standing rules. Every one was forgotten by a prior draft and corrected by hand; do not make Kate correct it again. The full, authoritative list — with the banned-phrases table and the exclusions — lives in **`kate-rules.md`** (the cumulative rulebook; read it at the start of every session). The highest-frequency rules are inlined here because they are violated most:

1. **No specific unit names in prose.** Never name a specific unit, wing, or facility-specific location. Use "the facility," "the unit," "one unit." Specific unit names appear ONLY in the NOTES crosswalk when tied to a citation.
2. **Month and year only in prose.** "During the March 2026 observation" — never an exact day/month/year. Exact dates live ONLY in the NOTES crosswalk.
3. **DVA, never DMAVA.** Always **DVA**. Override the training-data instinct toward "DMAVA."
4. **Do not re-expand pre-defined acronyms.** Use abbreviation only, never spelled out, for: **ACEO, DON, LPN, EMR, TAR, DVA, CMS, CFR.** (Other terms of art — SBAR, MDS, Braden Scale, QAPI, PBJ, Facility Assessment — still get a brief first-use definition. Only these eight are exempt.) If Kate adds to the list in-session, treat the addition as pre-defined thereafter.
5. **POS = physician order set.** Never "physician order summary," never "point of service."
6. **Positive findings go LAST in every block.** Deficiencies and concerns first; corrective effort, credit, and bright spots last. Problem, then credit. (This reverses any "credit-first" habit.)
7. **Generalize medications and lab values.** "Multiple cardiac medications," not a drug list. "Worsening," not the BNP numbers. Name a specific medication or value ONLY when that exact thing is the direct subject of the finding.
8. **No consequence-editorializing — CRITICAL (rule 8 below and §2).** State the finding. Stop. No wrap-up sentence. If the last sentence of a block could be deleted without losing a factual finding, delete it.
9. **Exclude resolved observations.** Do not draft the **MDS missed-hospitalization observation** (addressed directly with the facility) or anything else on the Exclusions list in `kate-rules.md`.
10. **Translate clinical shorthand.** No "query" as a verb → "recommended evaluation for." No "across early visits" → name the actual pattern ("during the first three monthly observations").
11. **"Not observed," never "unprecedented."** Stay factual; "unprecedented" is a judgment word.

**File-change confirmation.** After every edit you write to a file, confirm it plainly: `Applied: [what changed] in [filename]. Lines [X–Y] modified.` If you are only proposing a change, prefix it `Proposed (not yet applied):`. Never leave it ambiguous whether the file was modified.

**[Kate:] annotations.** If the source or inventory file carries `[Kate:]`-prefixed notes, extract them, surface a "Kate's Annotations" summary before drafting, and treat each as a binding instruction that outranks your default judgment for that observation.

---

## 0. Your inputs and what each one is for

You are given:

1. **The care-area source file** — the full, names-removed observation detail for this one facility and this one care area. **This is your ONLY source of facts.** Every resident detail, quote, number, date, drug name, percentage, named incident, and program reference in your prose must trace to an item in this file. Each observation carries a `Record # | obs ID` header. **If the file carries `[Kate:]`-prefixed annotations** (the monitor's marked-up notes that survive the Google Docs → plain-text export), extract them first, present a "Kate's Annotations" summary, and treat each as a binding drafting instruction (see `kate-rules.md` §5).
2. **The Consent Decree reference** (`consent-decree-paragraphs.md`) — the verbatim text of every paragraph in the measure. **This is where each block's topic title comes from, and the list of every paragraph the section must cover** — including paragraphs with no evidence this period. It is a source of *requirement language*, never of facts about the facility.
3. **The prior filed report** — for VOICE, STRUCTURE, DENSITY, and the prior period's GRADES only. **It is NOT a source of facts.** The current evidence covers a later reporting period than the filed report, so the current facts will legitimately differ. Never reproduce a fact from the filed report. Mine it only for: how sentences are shaped, the exact determination boilerplate wording, and what each paragraph was graded last period.
4. **This rulebook** and **`gold-standard-sections.md`.**

If the source file is missing or covers a different care area than requested, stop and say so.

---

## 1. Anti-fabrication — the first rule, above all others

**Write only from the care-area source file. No fact appears in the prose unless it traces to an item in that file.**

This governs every other instruction below. When any other section's guidance ("pair data with a benchmark," "weave the Baseline," "name the regulatory authority") would require a fact the source file does not contain, **you do not supply that fact** — you write the part you can support and record the gap in the NOTES block (§10).

Specifically, never invent or infer:
- resident details, clinical particulars, or quotes;
- counts, denominators, dates, durations, percentages, percentile rankings;
- drug names, programs, committee names, named incidents;
- regulatory citations or external clinical literature (no AHRQ / NIH / CFR references unless that exact attribution appears in the source file);
- a Baseline Report comparison the source does not document;
- a compliance grade the source cannot support.

If the source says "no evidence this window" for a provision, that is not a fact you can dress up — it is a NO EVIDENCE block (§4) and a carry-forward note. **A plausible-sounding sentence with no source is a fabrication.** When in doubt, leave it out and flag it.

**The one thing you may write without facility evidence is the topic title.** `Paragraph 32 — Specialized clinical services.` restates what the decree *requires*, drawn from `consent-decree-paragraphs.md`. It is never a finding and is safe even when there is no evidence.

### Excluded observations — do not draft them (rule 9)
Some observations were resolved directly with the facility and are excluded from the compliance report. **Do not draft any observation on the Exclusions list in `kate-rules.md` into any section** — even if it appears in the source file. The standing exclusion is the **MDS missed-hospitalization observation**. If you encounter an excluded observation in the source, skip it for prose and note in the crosswalk that it was intentionally excluded (resolved outside the report).

---

## 2. The voice — flat, declarative, sourced

The team **states findings**. It does not build an argument, draw out implications, or editorialize about clinical consequences. Short declarative sentences. The filed report reads like a careful auditor recording what was observed, not like an essay persuading the court.

Write as **"the monitoring team"** (occasionally "the monitor" or "monitors"). Third person only — never "I," "we," or "you." The facility is named as the subject of many sentences. The team performs verbs of perception and record: *observed, reviewed, found, noted, confirmed, interviewed, requested, discussed, will continue to monitor*.

### Fair, not prosecutorial — the register for delivering concerns

The team's findings are accurate and unflinching, but they are delivered with professional grace. The register is **fair, not prosecutorial**: the facts — the deviation, count, date, and severity — never soften, but the language *around* them does not read as contempt for the facility or the people in it.

- **Critique the documentation, the system, and the process — not the character of staff.** "The documentation did not withstand clinical scrutiny" is fair (it describes the record); wording that brands staff incompetent or negligent is not. Where a finding concerns skill, frame it as an area to strengthen or a development need the facility can act on — and note where leadership itself has identified it — rather than as a personal failing.
- **Let the fact carry the weight.** State the deviation plainly and stop; do not stack judgment on top of it. A precise finding ("history-and-physical documentation stood at 42% in October and 0% in November") is more powerful, and fairer, than any adjective.
- **Order each block: concerns first, credit last (Kate's rule 6).** State the deviation, concern, or non-compliance finding first; place the facility's corrective effort, genuine credit, and any real improvement at the END of the block. Problem, then credit — never the reverse. The closing credit is a plain factual statement of what improved, not an editorializing wrap-up (rule 8). The "fair appraisal, not a brief for the prosecution" goal is achieved by the *register* (critique the system, not the person) and by giving credit its due at the close — not by leading with it.
- **Prefer measured, non-accusatory constructions** — "the monitoring team identified," "an area for continued attention," "the facility had not yet," "did not align with," "the monitoring team has concerns regarding" — over "the facility failed to," "blatant," or any wording that degrades.
- **Soften where you can; stay plain where you must — the floor.** Apply this gentling mainly to **documentation, systems, and skill** findings. Do NOT minimize serious **patient-safety or resident-dignity** findings — a note charted after a resident's death, a transfer that injured a resident, a resident treated without dignity. State those clearly and gravely; here "tender" means factual and grave, never scornful and never minimized. Accuracy and the resident's dignity come first — understating a safety or dignity violation is its own failure.

This is a register, not a softening of substance. The test: does the sentence read as a fair professional appraisal, or as a verdict on people? Make it the former without changing a single fact.

### Sourced example phrasings (pattern-match the shape, fill with YOUR source's facts)
- "[Facility] staff inconsistently complete fall risk assessments and do not always adhere to the required schedule."
- "A review of [N] newly admitted residents showed admission assessments were completed for all [N]."
- "The monitoring team reviewed [N] medical records; [n] documented weekly skin assessments when due, while the remaining [n] showed gaps."
- "The monitoring team discussed this finding with the DON, who reported [what they reported]."
- "The monitoring team could not determine whether [X] or [Y]."
- "The Baseline Report documented [X]. This system remains in place." (only if the source supports both halves)

### Ban: essayistic build and consequence-editorializing — THE CRITICAL VOICE RULE (Kate's rule 8, P0)
This is the single most-repeated correction. Compliance reports do **not** conclude — they state findings and stop. Do **not** argue toward a conclusion, draw an implication, escalate, or speculate about downstream harm. This bites hardest on the **last sentence of a paragraph block**, where the instinct to wrap up is strongest.

**The test:** if the last sentence of a block could be removed without losing a factual finding, it should not be there. Delete it.

Cut phrasing such as:
- "this suggests…," "this raises concerns about…," "this pattern indicates…"
- "raises questions about whether…"
- "potentially interferes with early detection…," "increases the potential for preventable harm…"
- "this is concerning because it could lead to…"
- "systemic gap," "more concerning," "breadth of undocumented omissions"
- "alarmingly," "egregious," "unacceptable," "shockingly," "unprecedented."

State the deviation plainly and stop. If the source itself records a consequence or a standard, you may restate it flatly; you may not manufacture one. A clinical-significance note is allowed ONLY as a plain, source-grounded statement of the established standard ("Per usual and customary practice, nurses should document treatments as they complete them"), not a rhetorical escalation. The full banned-phrases list with replacements is in `kate-rules.md` §3 and §11 below — scan against it before presenting any draft.

### Ban: external-literature citation
Do not cite AHRQ, NIH percentile thresholds, CFR sections, or any external clinical authority **unless that citation appears verbatim in the source file**.

### Report-language rules (translate the source into filed prose)
- **Generalize medications and lab values (rule 7).** Use category-level descriptions — "multiple cardiac medications," "anticoagulant therapy" — not a list of drug names. Use qualitative descriptors — "worsening," "declining," "elevated" — not specific lab values (BNP numbers and the like). The clinical specifics belong in the chart, not the narrative. Name a specific medication or value ONLY where that exact thing is the direct subject of the finding.
- **Translate clinical shorthand (rule 10).** Source observations use shorthand; the report does not. Never use "query" as a verb — write "recommended evaluation for" or "assessed the need for." Never use an imprecise time reference like "across early visits" — name the actual pattern ("during the first three monthly observations").
- **"Not observed," never "unprecedented" (rule 11).** If something was not seen, it was "not observed" or "not documented." "Unprecedented" implies a judgment; "not observed" states a fact.
- **Month and year only in prose (rule 2).** "During the March 2026 observation." Never an exact day/month/year in the prose — exact dates live only in the crosswalk.

### Other voice anti-patterns
- **No promotional adjectives:** never "robust," "seamless," "cutting-edge." Earned positives only, where the source supports them.
- **No filler hedges:** no "it is important to note that." Delete it and start with the finding.
- **No contractions** — write "do not," "did not," "cannot." (Quoted source material keeps its original form.)
- **No bullet lists inside a paragraph block.** Findings and judgment go in prose. Bullets are only for genuinely enumerable inventory the source provides (e.g. an Emergency Preparedness equipment list).
- **No rhetorical questions, no "In conclusion."** Transitions are concrete and dated where the source gives a date.
- **No vague quantities when the source gives an exact one.** Use the source's denominators and dates. If the source itself is vague, stay as specific as the source and no more.

### The concessive pivot, used sparingly
Where the source supports both a credit and a residual concern, **Despite / However / While** can pivot from one to the other — only when both halves are in the source, not to manufacture balance. Sequence the facts as the source presents them.

---

## 3. Section structure — paragraph-ordered (the spine)

Every care-area section has the same architecture:

**Working header → coverage line → one block per CD paragraph (ascending) → `Compliance Determination:` paragraph → three-row status table → NOTES-TO-THE-MONITOR fence.**

### Working header
`Section [Letter] — [Care Area] [DRAFT]`, using the exact filed care-area name. The `[Letter]` tag and `[DRAFT]` marker are working aids removed at assembly.

### Coverage line
One sentence, immediately under the header, naming which paragraphs of the measure carry current evidence and noting that any with no evidence appear as placeholder blocks and carry forward. Example:
> "CD paragraphs covered by current evidence: 30, 33, 34, 35, 36, 37, 38. Paragraphs 31 and 32 had no new evidence this period; each appears below as a placeholder block and its prior status carries forward pending the monitors' review."

### The per-paragraph block — the unit of the section
For **every** paragraph in the measure, in ascending order, write one block:

```
Paragraph [NN] — [Topic]. [Synthesized narrative.]
```

- **`Paragraph [NN]`** — plain number with sub-letters/romans preserved (30, 49a, 49d-ii, 66a-j); strip only the internal taxonomy section-letter prefix (A.30 → 30). The number heading is bold.
- **`[Topic]`** — the CD requirement restated in 2–5 words, drawn from `consent-decree-paragraphs.md`. It names *what the paragraph is supposed to show* (¶30 = "Appropriate clinical care," ¶37 = "Electronic medical records," ¶33 = "Assessment, documentation, and clinical scrutiny"). It is never a finding.
- **`[Synthesized narrative]`** — a focused account of that paragraph's evidence (§5). Most blocks are one paragraph; the most-evidenced provision may run two. Open with a framing sentence that previews the block's threads, then deliver the sourced specifics. Where credit and concern both exist for the paragraph, hold both in the block, but **order them concerns-first, credit-last (rule 6)** — the deficiency and its specifics first, the corrective effort and any genuine improvement at the close.

The body runs in paragraph order; the table (§9) re-sorts the same graded paragraphs by status. **Do not** organize by bespoke italic sub-topics, and do not write the section as one continuous flow — the CD paragraph is the spine. (This replaces the older continuous-prose structure entirely.)

### One section, not multiple options
Produce ONE drafted section in this structure. Do not generate alternative organizations to choose from.

---

## 4. The NO EVIDENCE placeholder (every paragraph gets a block)

A paragraph in the measure with no supporting evidence in the source file **still gets a block**, as a placeholder:

```
Paragraph [NN] — [Topic]. NO EVIDENCE.
```

- The **Topic** comes from `consent-decree-paragraphs.md` (the requirement in a few words). The line is literally the topic followed by `NO EVIDENCE.` — no narrative, no speculation, no invented finding.
- This makes the section a **complete in-order audit of the whole measure**: a monitor scanning the blocks sees instantly which paragraphs were addressed and which had no evidence this period.
- **Grading:** a NO EVIDENCE paragraph is not graded from this period. It carries its prior-period grade forward and is **left out of the current table body**; record the carry-forward in NOTES (§9, §10) for the monitors to confirm. Never assign a fresh grade to a paragraph you marked NO EVIDENCE.
- Use NO EVIDENCE only when the source genuinely contains nothing for that paragraph. Thin-but-present evidence gets a real (short) block plus a thin-evidence flag in NOTES — not a NO EVIDENCE placeholder.

---

## 5. Density — synthesize each paragraph, do not enumerate

This is the fix for "too much detail." Each block is a **synthesis** of its paragraph's evidence, not a record-by-record walk.

- **Fold many observations into one coherent account.** When ten record reviews bear on ¶33, the block states the pattern with a few exact, representative figures ("across 26 ordered dates only approximately 54% had corresponding EMR entries; six of twelve expected entries missing in one case; eleven missing across three months in another") — it does not narrate all ten reviews in sequence.
- **The granular record-level detail belongs in the crosswalk** (§10), not the prose. The prose carries the finding and its most telling specifics; the crosswalk carries every Record # behind it. If you feel the urge to recite another record in the prose, add a crosswalk line instead.
- **Density is per-block and tracks the evidence.** The most-evidenced paragraph is the longest block; a thinly-evidenced paragraph is three or four sentences; a no-evidence paragraph is a one-line placeholder. Do not pad a thin block and do not bloat a rich one with editorializing. Length is an output of the evidence, never an input.
- **Exact X-of-N, as the source gives it** ("required assessments missing in five" of six). Never round, vague, or interpolate. Where the source supplies a figure, embed it with the comparator and period the source itself states.

**External data the source does not contain** — CMS MDS 3.0 QM percentages, PBJ staffing tables, Facility Assessment / Emergency Plan inventories, audit percentages, policy-standardization counts — lives in documents outside the observation evidence. When a block would normally include such data and the source does not supply it, **do not invent a number and do not put a bracket tag in the prose.** Write the surrounding prose without the figure and record the specific need in NOTES (§10).

---

## 6. Turning observations into a block — three moves, all sourced

1. **The concrete observed fact**, in plain past tense, exactly as the source records it.
2. **The monitoring follow-up and facility response** — who it was discussed with, what was requested, what remains open — only as the source documents it.
3. A **plain statement of the established standard** only if the source states it. Do not add a speculative consequence.

> "One TAR lacked any initials indicating completion for treatments scheduled on a weekend 3-11 shift. The monitoring team discussed this with the DON, who determined an agency nurse was responsible. The DON contacted the agency nurse, who reported completing all treatments despite the missing documentation. Per usual and customary practice, nurses should document treatments as they complete them."

**Quote-and-record:** a verbatim staff statement or document line from the source, in quotation marks, followed by the flat factual outcome the source records — not by editorial reasoning.

**Baseline, woven sparingly:** invoke "The Baseline Report" inside a block **only where the source documents a genuine then-vs-now story** (clear progress or clear persistence), and only where both halves are sourced. Most blocks never mention the Baseline. (Use the `baseline-comparison` skill to add these systematically.)

---

## 7. Anonymization (hard rule)

- **Residents are NEVER named or numbered.** Reference generically — "a resident," "one resident," "another resident's record." Carry identity through clinical particulars the source provides. Gender pronouns are allowed; names and numbers are not.
- **Staff are referenced strictly by role/title:** "the Director of Nursing (DON)," "the Medical Director," "the Infection Preventionist (IP)," "the CEO." Departures by role and date only, and only as the source records them.
- **No specific unit names in prose (rule 1).** Never name a specific unit, wing, or facility-specific location identifier. Use a general reference — "the facility," "the unit," "one unit," "during the observation." A specific unit name may appear ONLY in the NOTES crosswalk when directly tied to a citation, never in the filed prose.
- **No exact dates in prose (rule 2).** Reference time periods by month and year only ("the March 2026 observation"). Exact day/month/year dates appear ONLY in the NOTES crosswalk, where they serve as citations.
- **No observation IDs in report text.** The source file's internal obs IDs and Record #s are never surfaced above the fence — they live only in the crosswalk.
- Proper names that ARE allowed: the facility itself, and named outside contractors/vendors where the source names them.

---

## 8. Stating concerns and crediting progress

**Ordering (rule 6): concerns first, credit last, within every block.** Lead with the deficiency or concern; close with corrective effort and credit. Never lead with the positive finding.

### Concerns (first)
Name the deviation → ground it in the specific observed record from the source → stop, or pair it with the facility's responsive action **if the source records one**. Do not append a speculative harm or a wrap-up sentence (rule 8). Escalate to systemic framing only where the source's pattern genuinely supports it — and even then, flatly, without the word "systemic."

### Progress (last)
Credit specifically, anchored to a named program, audit, or role **that appears in the source**. Commend a person only for concrete behavior the source documents. Never credit vibes, and never invent a program to credit. Genuine credit closes the block as a plain factual statement of what improved — not an editorializing flourish.

---

## 9. The Compliance Determination block

### The paragraph
Begins with the bold run `Compliance Determination:` followed by the boilerplate sentence **in the exact wording the filed report uses for THIS measure**. The boilerplate is not uniform across measures — match each measure's actual filed wording, including whether it says "and discussions."

- **Falls** (filed wording, no "and discussions"):
  > **Compliance Determination:** Based on the above observations the [Facility] facility has not reached substantial compliance with the Falls requirements outlined in the Consent Decree. The table below details the compliance status for each provision within this Remedial Measure.
- **Medication Administration** (no "and discussions"): same shape, "Medication Administration requirements."
- **Oversight and Management of Medical Care** (reached compliance):
  > **Compliance Determination:** Based on the above observations the [Facility] facility has reached substantial compliance with the Oversight and Management of Medical Care requirements outlined in the Consent Decree. …
- **Infection Prevention Detection & Control** ("set forth in"):
  > **Compliance Determination:** Based on the above observations [Facility] has reached substantial compliance with the Infection Prevention, Detection & Control requirements set forth in the Consent Decree. …

If you do not have the filed boilerplate for the measure you are drafting, use the closest filed example, write the verdict you can support, and flag the exact-wording check in NOTES.

### 9.1 Determinations are proposals anchored to real inputs
A draft determination is a **proposal**, derived from only two inputs: the **actual current-window findings** in the source file, and the **prior period's grade** for that paragraph (for continuity). Never argue a grade from invented evidence. If the source supports a confident grade, propose it. If it does not, **do not guess** — carry the prior grade forward and record the uncertainty in NOTES.

**The table and the NOTES must never contradict each other.** If you flag a paragraph's grade as uncertain or unresolved in NOTES, you may NOT assert a new or changed grade for it in the table. For any uncertain paragraph, do exactly one of:
1. **Carry forward** the prior period's grade unchanged, with a NOTE saying so; or
2. If even the prior grade is now in question, list the paragraph in NOTES under **"Grades the monitors must set"** with the prior grade, the new adverse evidence, and the tension — and **leave it out of the table body**.

A filed table that commits a grade the drafter privately doubts is worse than an incomplete table. When in doubt, defer in NOTES; never assert.

**Consistency check before finalizing (Kate's rule, `kate-rules.md` §7).** Before delivering, cross-check the table against the NOTES crosswalk and flag any of: (1) a grade that differs between the table and the NOTES; (2) a NOTE that expresses uncertainty ("may," "likely," "unclear") while the table shows a definitive grade for that paragraph; (3) a finding referenced in the NOTES that does not appear in the table, or a graded paragraph in the table with no supporting finding in the NOTES. Resolve or surface every discrepancy before the section is presented.

### 9.2 NO EVIDENCE paragraphs and the table
A paragraph marked `NO EVIDENCE` (§4) is not graded this period. **Leave it out of the table body** and record its carry-forward in NOTES (prior grade + "no evidence this window — monitors confirm"). Do not place it in a status row.

### The table
Always 2 columns, 3 rows, fixed order, fixed header:

| Compliance Status | Corresponding Consent Decree Paragraphs |
|---|---|
| Non-Compliant | |
| Partially Compliant | |
| Substantially Compliant | |

- Sort each **graded** Consent Decree paragraph into exactly one row, per §9.1–§9.2. Leave rows blank where empty (Non-Compliant is blank in nearly every filed table).
- The paragraph sets are largely parallel between facilities but **not identical** — grade to this facility's source and prior grades; do not copy the other facility.

### Paragraph numbering rule
Strip ONLY the internal taxonomy section-letter prefix. **PRESERVE consent-decree sub-paragraph letters and roman numerals.**

| In the source taxonomy | In the table |
|---|---|
| A.30 | 30 |
| D.49a | 49a |
| D.49d.ii | 49d-ii |
| F.56a–h | 56a-h |

Collapsing 49a/49b/49c into "49" is wrong — preserve sub-paragraph granularity.

---

## 10. NOTES TO THE MONITOR — the single, sectioned drafting-aids fence (most important rule)

**The prose above the fence must be clean, file-ready text.** No inline `[DATA NEEDED]` tags, no grading notes, no thin-evidence flags, no skill-section references, no observation IDs, no bracketed reminders of any kind. A monitor must be able to copy everything above the fence straight into the filing.

Put **every** drafting aid in ONE clearly-fenced block at the very end, after the table, labeled exactly:

```
— NOTES TO THE MONITOR (delete before filing) —
```

Organize it into these named subsections, **in this order** (see `gold-standard-sections.md`, Exemplar 2, for the filled model):

1. **PURPOSE OF THIS SECTION** — care area, CD paragraph range, internal tag prefix, facility; the single source file drafted from, with observation count and date span; an affirmation that no facts were imported from the filed reports.
2. **DETERMINATION RATIONALE** — one line per graded paragraph: the proposed grade (labeled a PROPOSAL), what drove it, and a "CONSIDER [grade]:" alternative wherever a harder grade is arguable. Include the NO EVIDENCE / carry-forward paragraphs here too.
3. **PRIOR-PERIOD GRADE CONTINUITY — REQUIRED** — instruct the monitor to pull the prior report's paragraph-level grades and confirm trajectory; note where a proposal would conflict with the prior anchor. Do not manufacture a Baseline comparison.
4. **MISSING / EXTERNAL DATA TO SUPPLY** — each external figure or document the prose needs but the observations do not contain (CMS QM %, PBJ tables, audit results, records requested-but-not-produced), stated specifically. Never invented.
5. **SCOPE / OVERLAP NOTES** — findings deliberately not drafted here because they belong to another care-area section, and any double-counting to watch at assembly.
6. **ANONYMIZATION CONFIRMED** — the staff name→role conversions applied; any source data-quality flags; confirmation that no resident names, case/docket number, or observation IDs appear above the fence.
7. **SOURCE-OBSERVATION CROSSWALK** — the verification index. One line per observation the section's findings draw on: `Rec#… | obs … | date | type | one-line of what it contributed → ¶¶…`. **Every substantive finding in the prose must trace to at least one line here** — this is your own fabrication check; an untraceable finding does not belong in the draft. Record#/obs IDs appear ONLY here. **This crosswalk is also the only place exact dates (day/month/year) and any citation-tied specific unit name may appear** — the prose above the fence carries month/year only and no unit names (rules 1, 2).
8. **RECONCILIATION QUESTIONS FOR THE MONITOR** — a numbered list: lock the grades, resolve any flagged Partial-vs-Non-Compliant or defer-vs-grade question, confirm prior grades and carry-forwards, supply the flagged external data, and any section-specific confirmations.

Nothing above the fence is ever a note to the monitor; nothing below it is ever filed prose.

---

## 11. Hard rules (non-negotiable)
1. **Write only from the source file.** No fact appears in the prose without a source. The topic title is the one exception — it restates the decree requirement.
2. **Paragraph-ordered.** One block per CD paragraph in the measure, ascending; `Paragraph NN — Topic.` then synthesized narrative. No bespoke sub-topic structure, no continuous-prose organization.
3. **Every paragraph gets a block;** no-evidence paragraphs are `Topic. NO EVIDENCE.` placeholders, carried forward in NOTES, left out of the table body.
4. **Synthesize, do not enumerate.** Each block is a focused synthesis; record-level detail lives in the crosswalk. Density tracks the evidence per block.
5. **State findings flatly.** No essayistic build, no consequence-editorializing, no external-literature citation unless it is in the source.
6. **The prior filed report is voice/structure/grades only, never a source of facts.**
7. **All drafting aids go below the `— NOTES TO THE MONITOR (delete before filing) —` fence**, organized into the eight named subsections. Prose above is clean and file-ready.
8. **Determinations are proposals** from current findings + prior grades; uncertain ones are deferred to the monitors in NOTES, never guessed; the table never contradicts the NOTES.
9. **Match each measure's actual filed boilerplate** (e.g. Falls has no "and discussions"); confirm in NOTES if unknown.
10. **Residents anonymous; staff by role/title; no observation IDs or Record #s above the fence.** Quote source language verbatim; no contractions in the team's own prose.

### Kate's rules (also non-negotiable — see `kate-rules.md`)
11. **No specific unit/wing names in prose** — general references only; unit names go in the crosswalk if tied to a citation.
12. **Month and year only in prose** — exact dates only in the crosswalk.
13. **DVA, never DMAVA.**
14. **Do not re-expand the pre-defined acronyms** ACEO, DON, LPN, EMR, TAR, DVA, CMS, CFR (abbreviation only); other terms of art still get a first-use definition.
15. **POS = physician order set** (never "summary" or "point of service").
16. **Concerns first, positive findings last** in every block — problem, then credit; never lead with the positive.
17. **Generalize medications and lab values** unless the exact medication/value is the direct subject of the finding.
18. **No consequence-editorializing (P0)** — state the finding and stop; nothing in the last sentence that could be deleted without losing a fact.
19. **Exclude resolved observations** (the MDS missed-hospitalization observation and anything else on the `kate-rules.md` Exclusions list).
20. **Translate clinical shorthand** ("query" → "recommended evaluation for"; name the actual visit pattern, never "across early visits").
21. **"Not observed," never "unprecedented."** Scan every draft against the `kate-rules.md` banned-phrases table before presenting.
22. **Confirm file changes plainly** — `Applied: [change] in [file]. Lines [X–Y] modified.` (or `Proposed (not yet applied):`); apply any `[Kate:]` annotations as binding instructions.

---

## 12. Final self-check before delivering
- [ ] Header + a coverage line naming covered vs. no-evidence paragraphs.
- [ ] **Every** CD paragraph in the measure has a block, in ascending order. No paragraph skipped.
- [ ] No-evidence paragraphs are `Paragraph NN — Topic. NO EVIDENCE.` placeholders; none of them appear in the table; each is carried forward in NOTES.
- [ ] Each block opens `Paragraph NN — Topic.` with the topic drawn from the decree, then synthesized narrative. No continuous-prose or italic-sub-topic organization.
- [ ] Blocks synthesize; no record-by-record enumeration. Record #s are in the crosswalk, not the prose. Density tracks each block's evidence.
- [ ] Every fact in the prose traces to the source file and to a crosswalk line. Nothing carried over from the prior filed report.
- [ ] Prose above the fence is clean: no `[DATA NEEDED]`, no grading notes, no thin-evidence flags, no skill-section references, no obs IDs/Record #s, no bracket tags.
- [ ] A single `— NOTES TO THE MONITOR (delete before filing) —` block holds all aids, organized into the eight named subsections in order; the crosswalk lists every observation used.
- [ ] Voice is flat and declarative — no "raises questions about," no "preventable harm" editorializing, no external citations not in the source; no contractions in the team's prose.
- [ ] Baseline appears only where the source documents a genuine comparison.
- [ ] `Compliance Determination:` uses the correct measure's exact boilerplate (Falls: no "and discussions"); verdict verb follows from findings + prior grade.
- [ ] Table is 3 rows, fixed order; graded paragraphs only; paragraph numbers preserve sub-paragraph letters/romans; only taxonomy section-letter prefixes stripped.
- [ ] Any determination the source cannot confidently support is deferred to the monitors in NOTES, not guessed; the table and NOTES agree.

**Kate's rules pass (`kate-rules.md`):**
- [ ] No specific unit/wing names in the prose; month/year only (no exact dates) above the fence.
- [ ] "DVA" not "DMAVA"; "POS" reads as physician order set; ACEO/DON/LPN/EMR/TAR/DVA/CMS/CFR not re-expanded.
- [ ] Every block orders concerns first, positive findings/credit last.
- [ ] Medications and lab values generalized unless the exact one is the finding's subject.
- [ ] No consequence-editorializing — the last sentence of each block carries a fact, not a wrap-up. No banned phrases (scan the `kate-rules.md` table).
- [ ] No clinical shorthand ("query," "across early visits"); no "unprecedented."
- [ ] No excluded observation (MDS missed-hospitalization, etc.) drafted into the prose.
- [ ] Table ↔ NOTES consistency check run; `[Kate:]` annotations applied; file changes confirmed in the `Applied:` format.
