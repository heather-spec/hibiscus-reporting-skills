# Kate's Rules — the cumulative, always-on rulebook

**This file is law for every Hibiscus drafting skill.** Read it at the start of every Hibiscus session, before any inventory, draft, voice check, baseline weave, or assembly. The monitor (Kate) established these rules over months of correcting the same mistakes; Claude must follow them without being reminded.

The handoff system (`session-handoff` skill) appends new rules here as Kate establishes them. **Never delete a rule from this file. Never silently override one.** If a draft request conflicts with a rule below, follow the rule and flag the conflict in NOTES.

> **Why this file exists:** every rule below was forgotten by Claude in at least one prior session and had to be re-taught by hand. They are not suggestions or style preferences — they are the difference between a draft Kate can use and a draft she has to rewrite. Treat a violation of any rule here exactly as you would treat a fabricated fact: a fatal defect that must not ship.

---

## 1. Hard rules (non-negotiable, every section)

These are absolute. They are not subject to "but detail is helpful" or "but the source said it that way."

1. **No specific unit names in prose.** Never use specific unit names, wing names, or facility-specific location identifiers in report prose. Use general references — "the facility," "the unit," "one unit," "during the observation." Specific unit names may appear ONLY in the NOTES crosswalk when directly tied to a citation. *(Default failure: Claude reaches for specificity because it thinks detail = helpful. It is not helpful here.)*

2. **Month and year only in prose.** Reference time periods using month and year only — "during the March 2026 observation," "in October 2025." Never put an exact date (day/month/year, e.g. "on March 14, 2026") in report prose. Exact dates are permitted ONLY in the NOTES crosswalk, where they serve as citations.

3. **DVA, never DMAVA.** The correct abbreviation is **DVA**. Never write "DMAVA." This is non-negotiable and applies to every section. *(Claude's training data wrongly associates the agency with "DMAVA / Department of Military and Veterans Affairs." Override it. It is DVA here.)*

4. **Do not re-expand pre-defined acronyms.** The following acronyms are pre-defined across all report sections and must be used in abbreviation only — never spelled out, never given a parenthetical expansion: **ACEO, DON, LPN, EMR, TAR, DVA, CMS, CFR.** If Kate adds an acronym to this list during a session, treat it as pre-defined for all subsequent drafting. *(This list overrides the general "define terms of art on first use" convention. Other clinical terms of art — SBAR, MDS, Braden Scale, QAPI, PBJ, Facility Assessment — still get a brief first-use definition. Only the listed acronyms are exempt.)*

5. **POS = physician order set.** Not "physician order summary." Not "point of service." Physician order set. Always.

6. **Positive findings go LAST.** Within each paragraph block, order findings: (1) deficiencies, concerns, and non-compliance findings FIRST; (2) positive findings, compliance credits, corrective effort, and bright spots LAST. Never lead with positive findings. The structure is **problem, then credit.** *(This reverses the old "credit-first" framing. Concern first, positive last, every block.)*

7. **Generalize medications and lab values.** Use category-level descriptions ("multiple cardiac medications," "anticoagulant therapy") rather than listing drug names. Use qualitative descriptors ("worsening," "declining," "elevated") rather than specific lab values (BNP numbers, etc.). The clinical specifics live in the medical record, not the report narrative. **Exception:** name a specific medication or value only when that exact medication or value is the direct subject of the finding.

8. **No consequence-editorializing — CRITICAL.** Do not editorialize, escalate, or draw conclusions, especially in the last sentence of any paragraph block. State the finding. Stop. No wrap-up sentences. No "this suggests," "this raises concerns about," "this pattern indicates," or similar. The reader draws their own conclusions. **Test: if the last sentence of a block could be removed without losing a factual finding, it should not be there.**

9. **Exclude the MDS missed-hospitalization observation.** Do not include the MDS missed-hospitalization observation in any report section — it was addressed directly with the facility and is excluded from the compliance report. See the Exclusions list (§4) for the full set of observations resolved outside the report.

10. **Translate clinical shorthand into full report language.** Source observations use clinical shorthand; report prose does not. Never use "query" as a verb — write "recommended evaluation for" or "assessed the need for." Never use imprecise time references like "across early visits" — specify the actual observation pattern ("during the first three monthly observations").

11. **"Not observed," never "unprecedented."** If something was not seen, it was "not observed" or "not documented." "Unprecedented" is a judgment word; stay factual.

---

## 2. Voice guards (suppress these patterns actively)

The team **states findings and stops.** It does not build an argument, draw out implications, editorialize about consequences, or escalate. Three voice failures to suppress on sight:

- **Editorializing / consequence-building** — sentences that argue toward a conclusion or speculate about downstream harm (rule 8). Compliance reports do not conclude; they state findings and stop.
- **Attribution voice** — wording that brands staff incompetent or negligent, or that reads as a verdict on people rather than a description of the documentation, system, or process. Critique the record, not the character. (The floor: do NOT soften serious patient-safety or resident-dignity findings into vagueness — those stay plain and grave.)
- **Escalation language** — comparative and dramatic intensifiers ("more concerning," "systemic gap," "breadth of undocumented omissions," "unprecedented," "egregious," "alarming"). Replace with the specific count or extent, or delete.

---

## 3. Banned phrases (catch before presenting any draft)

If any of these appear in a draft, fix them before showing Kate. The replacement column is the rule.

| Banned phrase | Why | Replacement |
|---|---|---|
| "No bright spots were identified during that observation" | Awkward, unnecessary | Omit entirely; note the absence of positive findings without this phrasing, or say nothing |
| "It is important to note that" | Filler, adds nothing | Delete. Start with the finding itself. |
| "Unprecedented" | Judgment word, not factual | "Not observed" or "not documented" |
| "We will continue to monitor" | Filler unless required by the framework | Delete unless the reporting framework specifically requires it |
| "Systemic gap" | Editorializing | Describe the specific finding without labeling it |
| "Raises questions about whether" | Editorializing, speculative | State the finding directly |
| "More concerning" | Escalation language | State the finding without comparative judgment |
| "Breadth of undocumented omissions" | Editorializing, dramatic | Describe the specific omissions found |
| "This suggests" | Draws a conclusion the report should not draw | State the finding. Stop. |
| "This raises concerns about" | Editorializing | State the finding. Stop. |
| "This pattern indicates" | Draws a conclusion | Describe the pattern factually. Stop. |
| "Across early visits" | Imprecise time reference | Specify the actual observation pattern |
| "Query hospital transfer" | Clinical shorthand, not report language | "Recommended evaluation for hospital transfer" |
| "DMAVA" | Wrong abbreviation | "DVA" |
| "Physician order summary" | Wrong expansion of POS | "Physician order set" |

---

## 4. Exclusions (observations resolved outside the report — never draft them)

Observations on this list were addressed directly with the facility and are excluded from the compliance report. Do not draft them into any section. Add to this list when Kate identifies further observations resolved outside the report process.

- **MDS missed-hospitalization observation** — addressed directly with the facility.

---

## 5. The [Kate:] annotation convention (how Kate marks up observations)

Kate annotates observation files in Google Docs using red font and inline notes, then exports to plain text — which loses the color. The standardized convention that survives the export is the **`[Kate:]` prefix**. Treat it as the official annotation method, not a workaround.

When a skill reads an observation or inventory file:
1. Parse and extract every `[Kate:]`-prefixed annotation.
2. Present them up front as a **"Kate's Annotations"** summary before drafting.
3. Apply each annotation as a binding instruction during drafting.
4. Flag which observations carry annotations and which do not.

A `[Kate:]` note is a direct instruction from the monitor and outranks the model's default judgment for that observation.

---

## 6. File-change confirmation (no ambiguity about what was edited)

After every edit operation, explicitly confirm what changed and where, in this format:

> **Applied:** [description of change] in `[filename]`. Lines [X–Y] modified.

If a change is proposed but not yet written to the file, prefix it:

> **Proposed (not yet applied):** [description]

Never leave Kate guessing whether a file was actually modified.

---

## 7. Table ↔ NOTES consistency (run before finalizing any section)

Before finalizing, cross-check the compliance table against the NOTES crosswalk. Flag and resolve:
1. Grades that differ between the table and the NOTES.
2. NOTES that express uncertainty ("may," "likely," "unclear") while the table shows a definitive grade.
3. Findings referenced in NOTES that do not appear in the table, or vice versa.

A paragraph the NOTES flag uncertain is **never** asserted at a definitive grade in the table. Carry it at its prior grade (with a NOTE) or leave it out of the table body for the monitors to set. Present any discrepancy to Kate before saving.
