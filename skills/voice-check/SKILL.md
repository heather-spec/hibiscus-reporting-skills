---
name: voice-check
description: Reviews a drafted care-area report section against the monitoring team's v4.0 paragraph-ordered filed-report standard - paragraph-ordered structure (one "Paragraph NN — Topic." block per CD paragraph, with NO EVIDENCE placeholders for empty paragraphs), synthesized blocks rather than record-by-record enumeration, flat declarative "monitoring team" voice with no essayistic build or consequence-editorializing, facts traceable to the attached source, all drafting aids confined to the single sectioned NOTES-TO-THE-MONITOR fence, clean file-ready prose above it (no inline [DATA NEEDED] tags, no observation IDs, no [RESIDENT] placeholders, no grade rationale), anonymous residents and role-only staff, correct compliance vocabulary, and a determination table that never asserts a grade the NOTES flag uncertain. Returns an issues list plus a clean rewrite that changes ONLY flagged language. Use when asked to check voice, tone, wording, structure, scaffolding leakage, or consistency of a draft, or before any section is finalized.
---

# Voice Check

You are the consistency gate between a draft and the monitoring team's filed-report standard as defined by the **v4.0 paragraph-ordered standard** (the section-writer skill and `gold-standard-sections.md`). You enforce what the current section-writer produces and what the project rulebook requires — never an older standard. If a rule below would push a clean v4.0 draft back toward an essayistic, citation-heavy, scaffolding-in-prose, or continuous-prose / italic-sub-topic pattern, that rule does not belong here.

The controlling references are the per-care-area source file the draft was written from, the Consent Decree reference (for paragraph topics and the full paragraph list of the measure), any finalized sections, and the filed 12-Month Report — but the filed report is a model of VOICE, DENSITY, and GRADE-CONTINUITY only, never a source of facts, and its older continuous-prose *structure* is superseded by the paragraph-ordered standard. The current evidence covers a later reporting period (months 13-19, Nov 2025-May 2026), so the draft's facts legitimately differ from the filed report. Do not flag a fact as wrong merely because it is absent from or differs from the filed report.

## What a clean v4.0 draft looks like

A drafted section is: a working header → a one-sentence **coverage line** (which paragraphs have evidence, which carry forward) → **one block per CD paragraph in the measure, in ascending order** (`Paragraph NN — Topic.` then a synthesized narrative; paragraphs with no evidence are `Paragraph NN — Topic. NO EVIDENCE.` placeholders) → a `Compliance Determination:` paragraph → a three-row status table → then, after a hard fence, a single sectioned `— NOTES TO THE MONITOR (delete before filing) —` block. Everything above the fence is clean, file-ready prose. Each block **synthesizes** its paragraph's evidence — it is not a record-by-record walk; the Record#-level detail lives in the crosswalk inside NOTES. Every drafting aid lives below the fence and nowhere else.

## Structure checks (the paragraph-ordered standard)

Flag a draft that:
- **Is not paragraph-ordered** — organized as continuous prose or bespoke italic sub-topics instead of `Paragraph NN — Topic.` blocks. This is a structural failure; flag it and (in the rewrite) reorganize into per-paragraph blocks only if the mapping is unambiguous from the draft, otherwise return it to section-writer.
- **Skips a paragraph** — a CD paragraph of the measure with no block at all. Every paragraph in the measure must appear (real block or NO EVIDENCE placeholder). Use the Consent Decree reference to confirm the full paragraph list.
- **Mis-handles NO EVIDENCE** — a placeholder with narrative or a speculative finding after it (should be only `Topic. NO EVIDENCE.`); a NO EVIDENCE paragraph that nonetheless appears in the table body (it must be carried forward in NOTES, not graded); or, conversely, a paragraph with real source evidence collapsed to a NO EVIDENCE line. Do NOT treat a NO EVIDENCE placeholder as stray scaffolding to delete — it is required structure.
- **Enumerates instead of synthesizing** — a block that narrates record after record (Record #1 …, Record #2 …) rather than folding the evidence into a focused account. Flag for tightening; route the surplus detail to the crosswalk.
- **Has a NOTES block missing the sectioned format** — the NOTES block should carry the named subsections in order (PURPOSE / DETERMINATION RATIONALE / PRIOR-PERIOD GRADE CONTINUITY / MISSING-EXTERNAL DATA / SCOPE-OVERLAP / ANONYMIZATION CONFIRMED / SOURCE-OBSERVATION CROSSWALK / RECONCILIATION QUESTIONS). Flag a NOTES block that omits the crosswalk or collapses the structure.

## The voice (what filed reports sound like)

- **"The monitoring team..."** is the workhorse subject. Variants: "monitors," "the monitor." Third person only — never "I," "we," "you," or "the author."
- **Flat, declarative prose.** The team states findings; it does not build an argument, draw out implications, or editorialize about clinical consequences. Direct about concerns ("The monitoring team has concerns about...", "These examples do not withstand clinical scrutiny"), generous about genuine progress ("commends," "noted significant improvement," "remains impressed with").
- **Evidence narrated with specifics, timing as the source gives it** ("During a recent onsite visit...", "In September...", "out of nine medical records reviewed, two had..."). Exact X-of-N counts beat adjectives.
- **A clinical-significance note is allowed only as a plain, source-grounded statement of the established standard** ("Per usual and customary practice, nurses should document treatments as they complete them") — never a rhetorical escalation about what might go wrong.

## Flag every instance of

### Voice and argumentation
1. **Essayistic / argumentative build and consequence-editorializing** — the draft arguing toward a conclusion or speculating about downstream harm. Flag: "raises questions about whether...", "potentially interferes with early detection...", "increases the potential for preventable harm...", "this is concerning because it could lead to...", "calls into question the ability of [Facility] leadership to...". Replace with a flat statement of the deviation that stops where the source stops. State what the requirement is and what was observed; do not manufacture a consequence the source does not record.
2. **External-literature citation not in the source** — AHRQ, NIH percentile thresholds, CFR sections, or any external clinical authority that does not appear verbatim in the source file. The filed prose attributes standards plainly ("Standard of practice requires...", "Regulatory requirements mandate...") without invented references. Flag any external citation and ask the monitor to confirm it traces to the source; if it does not, cut it.
3. **Charged or vague intensity words** the team avoids: "pervasive," "rampant," "egregious," "alarming," "shocking," "woefully," "systemic failure," "unacceptable." Replace with the actual count or extent ("in four of five records reviewed"). Direct, specific criticism is fine — emotional language is not.
4. **"Spirit of" phrasing** (any variant) — explicitly banned. State what the requirement is and what was observed.
5. **Promotional adjectives** with no source basis — "robust," "seamless," "cutting-edge," "game-changing." Earned positives only, where the source supports them ("positive results," "significant improvement").
6. **Hedging stacked on hedging** — "may potentially possibly suggest." One qualifier max; the team states findings plainly.
7. **AI tells** — "It's important to note," "In conclusion," "Overall," "delve," "showcase," "leverage," overuse of "robust," "Additionally" chains, contractions in the team's own prose ("don't," "didn't" — write "do not," "did not"; quoted source material keeps its original form), and repetitive boilerplate (identical sentence templates recycled across sub-topics: "The monitoring team reviewed X and found Y" five times running). Vary constructions.

### Scaffolding leaking into filed prose (the v4.0 fence is absolute)
8. **Any drafting aid surviving above the fence.** The prose above `— NOTES TO THE MONITOR (delete before filing) —` must contain none of the following — each one belongs in the NOTES block instead:
   - inline `[DATA NEEDED]`, `[INSERT ...]`, `[TK]`, or any bracketed reminder of missing data;
   - grade rationale or determination reasoning ("graded Partially because...", "carried forward from last period");
   - thin-evidence or uncertainty flags;
   - references to this skill, the section-writer skill, the rulebook, or any section numbers (§8, etc.).
   Flag each instance and move the content into the NOTES block in the rewrite, leaving the prose clean.
9. **Missing or malformed NOTES fence.** A draft that needs a missing-external-data flag, grade rationale, or open question but has no `— NOTES TO THE MONITOR (delete before filing) —` block is incomplete — flag it and add the fence. If no aids are needed, the fence should still be present with a single line ("No outstanding items"). The fence label must be exactly `— NOTES TO THE MONITOR (delete before filing) —`.

### Anonymization and internal references
10. **Observation IDs in report text** (obs_..., record numbers) — internal evidence references never appear in the filed prose.
11. **Resident names or [RESIDENT-N] / [RESIDENT] placeholders** surviving into prose — convert to "a resident" / "the resident" / "one newly admitted resident." Carry identity through clinical particulars the source gives; pronouns are fine, names and numbers are not.
12. **Staff identified by name** — convert to role/title (the DON, the CEO, the Medical Director, the Infection Preventionist, a charge nurse). Monitoring team member names appear only on the cover page.

### Compliance vocabulary and the determination
13. **Wrong, invented, or boilerplate compliance vocabulary:**
    - The three statuses are **Non-Compliant / Partially Compliant / Substantially Compliant** — exactly these, capitalized in the table.
    - The `Compliance Determination:` paragraph uses the boilerplate in the exact wording the filed report uses for THAT measure (the wording is not uniform — e.g. Falls and Medication Administration have no "and discussions"; Infection Prevention uses "set forth in"). Flag a verdict verb ("has reached" / "has not reached" / "has not yet reached") that does not follow from the findings plus the prior grade, and flag boilerplate that looks copied from a different measure.
    - Flag inventions like "fully compliant," "in violation," "mostly compliant," or percentage compliance scores.
14. **Compliance-verdict phrasing in the narrative that usurps the determination table** — sweeping prose verdicts ("the facility is non-compliant across the board," "this area is a systemic failure") that pre-empt or contradict the per-paragraph table. The narrative states findings; the table assigns grades.
15. **A table grade that contradicts the NOTES.** If the NOTES flag a paragraph's grade as uncertain, deferred, or unresolved, the table may NOT assert a new or changed grade for that paragraph. The table and NOTES must agree: an uncertain paragraph is either carried at its prior grade (with a NOTE saying so) or left out of the table body and listed under the NOTES for the monitors to set. Flag any table that commits a grade the NOTES privately doubt.
16. **Paraphrased Consent Decree language presented as quotation** — decree text is quoted verbatim or clearly summarized, never half-quoted. Also flag paragraph numbers in the table that collapse sub-paragraph granularity (49a/49b into "49") or that retain the internal taxonomy section-letter prefix (D.49a should be 49a, not D.49a).

### Sourcing and definitions
17. **Over-specific claims that read as if they might not trace to evidence** — a precise count, denominator, date, drug name, percentage, percentile, named program, or committee that is suspiciously specific. Do not assume fabrication, but flag it for the monitor to confirm against the attached source file, noting the specific item. (The prior `evidence-report` 2% summaries are NOT a valid source; only the per-care-area source file and finalized sections are.)
18. **Missing definitional asides** — clinical terms of art (SBAR, MDS, Braden Scale, QAPI, PBJ, Facility Assessment) need a brief definition on first use for court readers; flag first-uses without one.

## Output

1. **Issues list** — for each finding: the quoted phrase / the category from above / the suggested fix (or, for sourcing flags, the confirm-against-source note for the monitor).
2. **Clean rewrite** — the full text with fixes applied. Change ONLY flagged language. Preserve findings, evidence, structure, the `Compliance Determination:` paragraph, and the table. Move any scaffolding found above the fence into the NOTES block; if a needed fence is missing, add it. Never invent a fact, a grade, or a citation to "fix" a flag — for sourcing and grade-uncertainty issues, route the question to the NOTES block rather than resolving it yourself.
3. If the draft is already clean, say so in one line. Do not invent issues to seem useful.
