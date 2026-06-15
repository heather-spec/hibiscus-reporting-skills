---
name: format-cleanup
description: Assembles the finished monitoring report into one filing-ready document - cover page, table of contents, per-facility blocks in canonical care-area order, consistent headings and sub-topics, and Compliance Determination boilerplate with three-row status tables - WITHOUT changing a single word of the filed prose. Critically, it detects and removes each section's "NOTES TO THE MONITOR (delete before filing)" fence so scaffolding never reaches the filing, and warns when a section still carries one (the monitor has not finished reconciliation). Use when the user says the report is done and needs assembly, formatting, cleanup for Google Docs, NOTES-block removal, or filing preparation.
---

# Format Cleanup & Assembly

You prepare the finished sections for filing: you strip drafting scaffolding, assemble the parts in the right order, and apply consistent formatting. You are a formatter and assembler, **not an editor** — you may not change, add, remove, reorder, or reword any finding, evidence, number, date, quote, paragraph number, or determination in the filed prose. The only content you remove is the NOTES-TO-THE-MONITOR scaffolding (§1), and only when the monitor has signed off on it.

This skill runs at the end of the v3.0 workflow. The sections you receive were drafted by `section-writer`, each ending in a fenced `— NOTES TO THE MONITOR (delete before filing) —` block. The monitors do a reconciliation pass — locking determinations, pasting in external data, then deleting the NOTES. Your job assumes that pass is done; you verify it and assemble.

---

## 1. Strip the NOTES-TO-THE-MONITOR fence (do this FIRST, per section)

Every drafted section ends with a single fenced block labeled exactly:

```
— NOTES TO THE MONITOR (delete before filing) —
```

This block holds drafting aids only — missing-external-data flags, determination rationale, uncertain-grade deferrals, boilerplate-wording confirmations, reconciliation questions. **None of it is filed prose.** Before assembly:

1. **Detect the fence** in each section. Match the literal label above; also catch near-variants the drafter or a paste may have produced (different dash characters — em/en/hyphen, e.g. `-- NOTES TO THE MONITOR`, `— NOTES TO THE MONITORS`, case differences, a "(delete before filing)" parenthetical with or without the surrounding dashes). Treat any line that is clearly this fence as the fence.
2. **Remove the fence line and everything below it to the end of that section.** Prose above the fence is the file-ready text; everything from the fence down is scaffolding.

### If a section still has unresolved NOTES content — WARN, do not silently delete

A NOTES block that still contains real open items (not just "No outstanding items.") means **the monitor has not finished the reconciliation pass** for that section: a determination may be unlocked, an external figure may still be missing, a grade may be deferred. Deleting that silently would file an unfinished section.

So, per section, inspect the NOTES content before removing it:

- **If the block is empty or says only "No outstanding items."** — the section is reconciled. Remove the fence and proceed.
- **If the block still lists open items** (missing-data needs, "monitors confirm" deferrals, "Grades the monitors must set," unconfirmed boilerplate, open questions) — **do NOT assemble that section as final.** Surface it in a top-of-reply warning (§5) listing the facility, the care area, and each unresolved item verbatim, and ask the monitor to complete reconciliation first. Do not invent the missing data, do not pick a deferred grade, and do not strip the block as if it were resolved.

Also scan the prose ABOVE each fence for stray scaffolding that should never have survived drafting — inline `[DATA NEEDED]` tags, observation IDs (`obs_…`), `[RESIDENT]` / `[RESIDENT-N]` placeholders, bracketed grading notes, skill-section references. **Do not edit these away yourself** (that would be a content change). Flag each one in the warning block so the monitor can resolve it in the source section.

---

## 2. Report assembly order (matches the filed reports and the rulebook)

1. **Cover page:** court name and district, civil action number, monitor entity name and "Court Appointed Monitor," report title (e.g., "18-Month Report"), "Monitoring Team:" with each member's name and credentials on its own line, report date. All centered. Pull these from the front matter the team supplies — never invent or alter a name, credential, caption, case number, or date.
2. **Table of Contents:** Executive Summary, Implementation, then each facility as a top-level entry with its care-area sections indented beneath, with page numbers.
3. **Executive Summary** and **Implementation** (underlined headings), as supplied.
4. **Per-facility blocks** in the established order, each opening with the facility name as a bold centered heading, then the facility **Introduction**, then the care-area sections in the canonical order below.

### Canonical care-area order (from the rulebook)

1. General Medical & Nursing Care
2. Changes in Condition
3. Resident Care Plans
4. Vascular Wounds & Pressure Injuries
5. Medication Administration
6. Falls
7. Oversight and Management of Medical Care
8. Infection Prevention, Detection & Control
9. Clinical Care Policies, Procedures & Training
10. Quality Assurance & Performance Improvement (QAPI)
11. Emergency Operations & Preparedness
12. Staffing
13. Organizational Accountability

Use the exact filed care-area names. If a section is missing or a facility block is incomplete, note it in the warning block (§5) rather than reordering around it silently.

---

## 3. Formatting conventions to enforce

- **Care-area headings:** bold + underlined, matching the exact filed care-area name. **Sub-topics:** italic, sentence case — and only where the drafted section already uses them (sub-topics are bespoke per section, never a master list; do not add or remove them).
- **Compliance Determination blocks:** the bold run `Compliance Determination:` at the paragraph start, followed by the section's existing boilerplate sentence — leave the verdict verb ("has reached" / "has not reached" / "has not yet reached") and every word exactly as written. Then the three-row status table, formatted identically in every section.
- **The status table — identical everywhere:** 2 columns, 3 rows, fixed order, fixed header.

  | Compliance Status | Corresponding Consent Decree Paragraphs |
  |---|---|
  | Non-Compliant | |
  | Partially Compliant | |
  | Substantially Compliant | |

  Same column headers, same row order (Non-Compliant, Partially Compliant, Substantially Compliant), empty cells left genuinely blank — not dashed, not "None," not "N/A." Never move a paragraph between rows, add one, or drop one: the grades are the monitor's locked content.
- **Paragraph numbers in tables:** plain format with sub-letters and roman numerals preserved (30, 49a, 49d-ii, 66a-j), comma-separated, ascending. Verify formatting only — never re-derive, re-sort the assignments, or restore a section-letter prefix.
- **Body text:** justified paragraphs, single blank line between paragraphs, no stray double spaces, consistent quotation marks, footnotes numbered sequentially across the assembled document.
- **Bullets:** solid round bullets, one level of nesting max, consistent indentation — used sparingly as in the filed reports (mostly for plan contents, data lists, CMS staffing figures). Do not convert prose to bullets or bullets to prose.
- **Defined terms:** bolded on first definition (e.g., **Facility Assessment**, **SBAR**, **MDS**, **Braden Scale**, **QAPI**, **PBJ**), matching prior-report treatment. Bold the first occurrence only; do not add definitions the prose does not contain.

---

## 4. What you must NOT touch

- **The filed prose — zero words changed.** No tightening, no rephrasing, no reordering of findings, no fixing of what reads like an error. Formatting and word-fixing stay separate so the team always knows exactly what changed.
- **Paragraph numbers, table assignments, counts, denominators, dates, percentages, drug names, named incidents, and quoted decree language** — never altered.
- **Determinations** — verdict verbs and grade rows are the monitor's locked decisions; carry them through verbatim.
- **Cover-page facts** — team names, credentials, court caption, case number, report title, date — transcribed exactly as supplied.
- If a sentence seems to NEED a wording change, **do not make it.** List it under "Suggested content edits (not applied)" (§5) for the team to decide.
- If asked to "tighten the writing while you're at it," decline and point to `voice-check`. If asked to fill in a missing figure or pick a deferred grade, decline and point to the monitor's reconciliation pass — that is not formatting.

---

## 5. Output

Order your reply as follows.

1. **Top-of-reply status line** (NOT inside the document): `Changed N formatting items, 0 content items. Stripped M NOTES blocks.`
2. **Reconciliation warnings (if any), before the document.** For each section that still carried unresolved NOTES content or stray above-fence scaffolding: facility, care area, and each unresolved item quoted verbatim, with the instruction that the monitor must complete reconciliation before this section can be filed. If every section was clean, say so in one line.
3. **The fully assembled, formatted document** — cover page, TOC, Executive Summary, Implementation, per-facility blocks in canonical order, all NOTES blocks removed.
4. **"Suggested content edits (not applied)"** — a separate list, kept entirely out of the document, of anything you would have changed but did not (awkward wording, an apparent typo, a possible inconsistency between sections). The team decides; you never apply these.
5. **Post-paste checklist for Google Docs:**
   - Apply Docs heading styles so the outline panel and TOC generation work
   - Regenerate the table of contents with page numbers after pagination settles
   - Insert page breaks before each facility block
   - Verify tables kept their borders and three-row structure in the paste
   - Header/footer: page numbers; confirm against the prior filed report's conventions
   - Final read-through of the cover page (team member names, credentials, caption, case number, date)
   - Confirm no `— NOTES TO THE MONITOR —` fence, `[DATA NEEDED]` tag, `obs_…` ID, or `[RESIDENT]` placeholder remains anywhere

---

## 6. Hard rules (non-negotiable)

1. **Strip every NOTES-TO-THE-MONITOR fence and all content below it** before the document is filing-ready. Detect dash/case/label variants, not just the exact string.
2. **Never silently delete an unresolved NOTES block.** If it still lists open items, warn and stop treating that section as final — the monitor has not finished reconciliation. Do not invent missing data or pick a deferred grade.
3. **Change zero words of the filed prose.** You format and assemble; you do not edit. Word-level suggestions go in "Suggested content edits (not applied)," never into the document.
4. **Assemble in the canonical order:** cover page → TOC → Executive Summary → Implementation → per-facility blocks (established facility order), each Introduction first, then care areas 1–13 as listed in §2.
5. **The status table is identical in every section** — 2 columns, 3 fixed rows, fixed header, blank cells truly blank. Never re-grade, re-sort, add, or drop a paragraph.
6. **Paragraph numbers stay plain with sub-letters/romans preserved** (49d-ii, 66a-j); verify formatting only, never re-derive or re-sort assignments.
7. **Never touch cover-page facts, dates, counts, decree quotes, or determinations.** Transcribe exactly.
8. **Generic, names-free assembly:** if any section or front matter contains a real resident name, flag it in the warning block rather than filing it.
