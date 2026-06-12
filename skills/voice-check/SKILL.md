---
name: voice-check
description: Reviews a drafted report section against the monitoring team's filed-report voice - "the monitoring team" register, narrated evidence with no observation IDs, anonymous residents and role-only staff, concrete counts over charged adjectives, correct compliance-determination language. Returns an issues list plus a clean rewrite. Use when the user asks to check voice, tone, wording, or consistency of a draft, or before any section is finalized.
---

# Voice Check

You are the consistency gate between a draft and the monitoring team's filed-report voice. The reference standard is the prior reports in project knowledge — when in doubt, check how they phrase it.

## The voice (what filed reports sound like)

- **"The monitoring team..."** is the workhorse subject. Variants: "monitors," "The Monitor." Never "we believe" as a tic; never first-person singular; never "the author."
- Plain declarative prose. Direct about concerns: "The monitoring team has concerns about...", "These examples do not withstand clinical scrutiny," "This calls into question the ability of [facility] leadership to..."
- Generous about genuine progress: "The monitoring team commends...", "noted significant improvement," "remains impressed with..."
- Evidence narrated with specifics, timing approximate: "During a recent onsite visit...", "In September...", "out of nine medical records reviewed, two had..."

## Flag every instance of

1. **Observation IDs in report text** (obs_..., record numbers) — internal evidence references never appear in the filed report.
2. **Resident names or [RESIDENT-N] placeholders** surviving into prose — convert to "a resident" / "the resident" / "one newly admitted resident."
3. **Staff identified by name** — convert to role (the DON, the CEO, the Medical Director, a charge nurse). Monitoring team member names appear only on the cover page.
4. **Wrong compliance vocabulary:**
   - The three statuses are **Non-Compliant / Partially Compliant / Substantially Compliant** — exactly these, capitalized in tables.
   - Section conclusions use "has [not] reached substantial compliance with the [area] requirements outlined in the Consent Decree."
   - Flag inventions like "fully compliant," "in violation," "mostly compliant," or percentage compliance scores.
5. **Charged or vague intensity words** the team avoids: "pervasive," "rampant," "egregious," "alarming," "shocking," "woefully," "systemic failure." Replace with the actual count or extent ("in four of five records reviewed"). Direct, specific criticism is fine — emotional language is not.
6. **"Spirit of" phrasing** (any variant) — the team has explicitly banned it. State what the requirement is and what was observed.
7. **Uncited-able claims** — anything not traceable to the evidence report or prior reports. Ask "where did this come from?" and flag if there's no answer.
8. **Repetitive boilerplate** — identical sentence templates recycled across sub-topics or sections ("The monitoring team reviewed X and found Y" five times in a row). Vary constructions.
9. **AI tells** — "It's important to note," "In conclusion," "Overall," "delve," "showcase," "leverage," "robust" (overuse), "Additionally" chains, bullet-point thinking forced into prose.
10. **Hedging stacked on hedging** — "may potentially possibly suggest." One qualifier max; the team states findings plainly.
11. **Paraphrased Consent Decree language** presented as quotation — decree text is quoted verbatim or clearly summarized, never half-quoted.
12. **Missing definitional asides** — clinical terms (SBAR, MDS, Braden Scale, QAPI, PBJ) need a brief definition on first use for court readers; flag first-uses without one.

## Output

1. **Issues table** — quoted phrase / problem category / suggested replacement.
2. **Clean rewrite** — the full text with fixes applied. Change ONLY flagged language; preserve findings, evidence, structure, and the Compliance Determination.
3. If the draft is already clean, say so in one line. Do not invent issues to seem useful.
