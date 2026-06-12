# Hibiscus Report Writing — Cowork Skills Plugin

Report-drafting skills for a federal-court compliance monitoring team
operating under a consent decree.

## The skills

| Skill | What it does | When to use |
|---|---|---|
| `section-writer` | Drafts one report section THREE ways (Evidentiary-Compressed / Narrative-Connected / Theme-Forward) from the evidence report, with a compliance designation per option | Drafting any body section |
| `exec-summary-writer` | Writes the executive summary LAST, anchored on the facility's underlying themes (defined in the project rulebook). Refuses to run until all body sections are final | After the body is done |
| `baseline-comparison` | Compares a finalized section to the actual Baseline report and appends a "Comparison to Baseline" subsection | Selectively, per section, after choosing a draft |
| `voice-check` | Scans drafts for forbidden vocabulary (compliance verdicts, "spirit of", "pervasive", etc.) and returns issues + clean rewrite | Before finalizing anything |
| `obs-lookup` | Traces obs_ids and lists evidence by CD paragraph/facility from the project CSVs. Pure lookup, no interpretation | Verifying citations, finding evidence |
| `format-cleanup` | Formats the finished report for Google Docs without changing any words (replaces the Gemini step) | Last step before paste-into-Docs |

## The intended workflow

```
evidence report (pinned)
   → section-writer (per section, pick/combine from 3 options)
   → voice-check (per section)
   → baseline-comparison (selectively)
   → exec-summary-writer (LAST, after all sections final)
   → voice-check (on the summary)
   → format-cleanup (whole document)
   → paste into Google Docs
```

## Project files these skills expect

Pin these in the Cowork project (latest versions live in the team's S3 vault under `names-removed/`):

- `evidence-report-<facility>-<date>.md` — drafting source of truth, one per facility
- `observation-index-names-removed-<date>.csv` — observation browser
- `evidence-by-paragraph-names-removed-<date>.csv` — evidence sorted by CD paragraph
- The Baseline report (needed by `baseline-comparison`)
- Optional: `observations-names-removed-<date>.json` — full text drill-down

All files have patient names replaced with [RESIDENT] placeholders. Original
records stay in the team's secure vault — ask the team lead for un-redacted lookups.

## Ground rules baked into every skill

- Monitors describe evidence; the court decides compliance. No verdicts, ever.
- Every claim cites (obs_id, date).
- No "spirit of", "pervasive", or charged adjectives — counts instead of intensity words.
- [RESIDENT] placeholders are never altered or guessed at.
