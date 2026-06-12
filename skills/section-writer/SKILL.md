---
name: section-writer
description: Drafts one section of the Hibiscus court report from the evidence report, producing THREE style options to choose from or combine. Use when the user asks to draft, write, or generate a report section (e.g. "draft Section A for Menlo Park", "write the care plans section"). Requires the facility's evidence report in the project files. Never makes compliance determinations; cites every claim with (obs_id, date).
---

# Section Writer

You draft one section of a federal-court compliance monitoring report (DOJ Consent Decree Case 2:24-cv-09577-JXN-JSA, NJ Veterans Memorial Homes) from the evidence report pinned in this project.

## Inputs

1. **Which section** (CD Section letter A–M, or a named topic like "care plans" — map it to the section).
2. **Which facility** (Menlo Park or Paramus). If not stated, ask.
3. **The evidence report** — find the file named `evidence-report-<facility>-<date>.md` in the project files. Use the one matching the facility. Read ONLY the matching section's paragraphs.

## Process

1. Read the relevant section of the evidence report. Note every paragraph with evidence, the volume (implications vs bright spots), and the (obs_id, date) citations.
2. Draft the section THREE ways (the team picks or combines):

   **Option 1 — Evidentiary-Compressed.** Tightest version. Leads with the dominant finding, groups related paragraphs, every sentence carries a citation. Reads like testimony.

   **Option 2 — Narrative-Connected.** Connects findings into a story of what monitors observed across the period. Slightly longer, smoother transitions, still fully cited.

   **Option 3 — Theme-Forward.** Organizes around the underlying problems rather than paragraph order (for Menlo Park, the dominant themes are DOCUMENTATION concerns and ASSESSMENT concerns — open with whichever the section's evidence supports). Paragraph references woven in.

3. Each option ends with a **Compliance Designation line** for the section, using only this scale: `Evidence consistent with the requirements` / `Mixed evidence` / `Evidence inconsistent with the requirements` / `Insufficient evidence to assess`. Never "compliant"/"non-compliant".
4. After the three options, add a short **"What differs"** note (2-3 sentences) so the reader can choose quickly.

## Hard rules

- Every factual claim cites (obs_id, date) from the evidence report. No citation → omit the claim.
- Bright spots are reported as observed positive practices, never as proof of compliance.
- [RESIDENT] placeholders stay as-is. Never invent or guess resident identity.
- Do not compare to the Baseline report — that is the separate `baseline-comparison` skill, applied after the section is chosen.
- Run the voice-check vocabulary rules mentally before finalizing (see `voice-check` skill): no "spirit of", "pervasive", "systemic failure", "must improve", "we conclude", or compliance verdicts.
- Length per option: 300–600 words. Do not pad. If evidence is thin, say so plainly.

## Output format

```
# Section <letter> — <section name> — <facility>
## Option 1: Evidentiary-Compressed
...
**Compliance designation:** ...
## Option 2: Narrative-Connected
...
**Compliance designation:** ...
## Option 3: Theme-Forward
...
**Compliance designation:** ...
## What differs
...
```
