# Hibiscus Report Writing — Cowork Skills Plugin

Report-drafting skills for a federal-court compliance monitoring team operating under a consent decree (NJ Veterans Homes, DOJ Consent Decree). **v4.0 — the paragraph-ordered standard.**

## The skills

| Skill | What it does | When to use |
|---|---|---|
| `section-writer` | Drafts ONE care-area section in the **paragraph-ordered** standard: a coverage line, then one `Paragraph NN — Topic.` block per consent-decree paragraph (synthesized from the source file; `NO EVIDENCE` placeholders for empty paragraphs), the Compliance Determination, the three-row status table, and a sectioned NOTES-to-the-monitor block | Drafting any care-area section |
| `voice-check` | Checks a draft against the v4.0 standard — paragraph-ordered structure, synthesized (not enumerated) blocks, flat declarative voice, scaffolding confined below the fence — and returns issues + a clean rewrite | Before finalizing a section |
| `baseline-comparison` | Weaves Baseline Report comparisons INLINE into the relevant paragraph block, only where a both-halves-sourced then-vs-now story exists | Selectively, per section |
| `exec-summary-writer` | Writes the Executive Summary, Implementation, and per-facility Introductions LAST, after the body sections are final | After the body is done |
| `obs-lookup` | Traces obs_ids and lists evidence by CD paragraph / facility from the project CSVs. Pure lookup, no interpretation | Verifying citations, finding evidence |
| `format-cleanup` | Assembles + formats the finished report for Google Docs without changing any words; strips the NOTES fences and warns on any unresolved NOTES or `NO EVIDENCE` block | Last step before paste-into-Docs |

## The intended workflow

```
per-care-area source file (02-source-evidence/<facility>/<NN>-<care-area>.md)
   → section-writer (one paragraph-ordered draft per care area)
   → voice-check (per section)
   → baseline-comparison (selectively, where a real then-vs-now exists)
   → monitor reconciliation pass (lock grades, fill external data, resolve NO EVIDENCE, delete NOTES)
   → exec-summary-writer (LAST, after all sections final)
   → format-cleanup (whole document)
   → paste into Google Docs
```

## Project files these skills expect

The skills draft from the per-care-area source files and reference the prior filed reports + CD text. In Cowork these live on the mounted Drive folder (`Hibiscus Court Reports`):

- `02-source-evidence/<facility>/<NN>-<care-area>.md` — **drafting source of truth**, full names-removed observation detail for one facility + care area, with a `Record # | obs ID` per observation. One file in, one section out.
- `01-reference/consent-decree-paragraphs.md` — verbatim CD text; supplies each block's topic and the full paragraph list of the measure (including no-evidence paragraphs).
- `01-reference/` prior filed reports (Baseline June 2025, 12-Month January 2026) — VOICE / DENSITY / GRADE-CONTINUITY model only, never a source of current facts (our evidence is a later period).
- `01-reference/observation-index-…csv` / `evidence-by-paragraph-…csv` — lookup indexes for `obs-lookup` and tracing.
- `00-instructions/gold-standard-sections.md` — the controlling paragraph-ordered exemplar; bundled with `section-writer` too.

All files have patient names removed. Original records stay in the team's secure vault — ask the team lead for un-redacted lookups. (The earlier `evidence-report-<facility>-<date>.md` summaries are DEPRECATED for drafting — they compressed clinical detail to ~2% and caused thin, fabrication-prone drafts.)

## Ground rules baked into every skill

- **Making compliance determinations is the monitor's job.** The section proposes a grade per paragraph, anchored to current findings + the prior period's grade; the monitors confirm or change every grade in the reconciliation pass. Draft grades are PROPOSALS, never asserted autonomously, and the table never contradicts the NOTES.
- **Evidence is narrated, never cited in the prose.** Observation IDs and Record #s appear ONLY in the NOTES crosswalk — never in the filed text. Every substantive finding still traces to a crosswalk line; an untraceable finding does not belong in the draft.
- **Write only from the source file.** No invented facts, numbers, dates, or quotes. External data not in the observations (CMS QM %, PBJ tables, audit results) is flagged in NOTES for the monitor to supply, never made up.
- **Flat declarative voice.** No essayistic build, no consequence-editorializing, no "spirit of," no charged adjectives, no external-literature citation unless it is in the source — counts and specifics instead of intensity words.
- **Names-free.** Residents anonymous; staff by role/title; `[RESIDENT]` placeholders never altered or guessed at; monitoring-team names only on the cover page.
- **The NOTES fence is absolute.** All drafting aids live below `— NOTES TO THE MONITOR (delete before filing) —`, organized into the eight named subsections; the prose above is clean, file-ready text.
