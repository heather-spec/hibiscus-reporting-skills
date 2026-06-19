# Hibiscus Report Writing — Cowork Skills Plugin

Report-drafting skills for a federal-court compliance monitoring team operating under a consent decree (NJ Veterans Homes, DOJ Consent Decree). **v5.0 — the paragraph-ordered standard, governed by the monitor's cumulative rulebook.**

> **v5.0 changes:** every skill now reads **`kate-rules.md`** (the monitor's standing rules) and enforces it. New rules baked in: no specific unit names in prose, month/year only (exact dates only in the crosswalk), **DVA not DMAVA**, no re-expansion of pre-defined acronyms, POS = physician order set, generalized medications/lab values, an excluded-observations list, clinical-shorthand translation, a banned-phrases table, and a strengthened ban on consequence-editorializing. **Paragraph ordering is reversed: concerns first, positive findings LAST** (the old "credit-first" framing is retired). Two new skills — `obs-inventory` and `session-handoff` — collapse the monitor's manual pipeline and carry context across sessions.

## The skills

| Skill | What it does | When to use |
|---|---|---|
| `obs-inventory` | Reads the care-area source file and produces, in one step, the **ranked evidence inventory** (narrative + strength-sorted table) AND the **coverage map** of which CD paragraphs have evidence; extracts `[Kate:]` annotations | Before drafting, to scope a section |
| `section-writer` | Drafts ONE care-area section in the **paragraph-ordered** standard: a coverage line, then one `Paragraph NN — Topic.` block per consent-decree paragraph (synthesized from the source file; `NO EVIDENCE` placeholders for empty paragraphs), the Compliance Determination, the three-row status table, and a sectioned NOTES-to-the-monitor block. Concerns first, credit last | Drafting any care-area section |
| `voice-check` | Checks a draft against the v5.0 standard — paragraph-ordered structure, synthesized blocks, flat declarative voice, scaffolding below the fence, **and every rule in `kate-rules.md` (banned phrases, ordering, unit names, dates, DVA, acronyms, generalization)** — and returns issues + a clean rewrite | Before finalizing a section |
| `baseline-comparison` | Weaves Baseline Report comparisons INLINE into the relevant paragraph block, only where a both-halves-sourced then-vs-now story exists | Selectively, per section |
| `exec-summary-writer` | Writes the Executive Summary, Implementation, and per-facility Introductions LAST, after the body sections are final | After the body is done |
| `obs-lookup` | Traces obs_ids and lists evidence by CD paragraph / facility from the project CSVs; flags excluded observations and surfaces `[Kate:]` annotations. Pure lookup, no interpretation | Verifying citations, finding evidence |
| `format-cleanup` | Assembles + formats the finished report for Google Docs without changing any words; strips the NOTES fences, warns on any unresolved NOTES / `NO EVIDENCE` block, and runs a final Kate's-rules scan | Last step before paste-into-Docs |
| `session-handoff` | At session start loads `kate-rules.md` + the latest handoff; at session end writes a self-contained handoff doc and appends any new standing rules to `kate-rules.md` | Start and end of every session |

## The intended workflow (streamlined)

```
session-handoff (START: load kate-rules.md + latest handoff)
   → obs-inventory (ranked inventory + coverage map, in one step)
   → annotate observations in Google Docs with the [Kate:] prefix, save
   → section-writer (one paragraph-ordered draft per care area; reads [Kate:] notes + rules)
   → voice-check (per section; enforces kate-rules.md)
   → baseline-comparison (selectively, where a real then-vs-now exists)
   → monitor reconciliation pass (lock grades, fill external data, resolve NO EVIDENCE, delete NOTES)
   → exec-summary-writer (LAST, after all sections final)
   → format-cleanup (whole document; final Kate's-rules scan)
   → paste into Google Docs
   → session-handoff (END: write handoff doc, update kate-rules.md)
```

## `kate-rules.md` — the cumulative rulebook

[`kate-rules.md`](./kate-rules.md) is the always-on rulebook every skill reads. It holds the monitor's hard rules, the banned-phrases table, the excluded-observations list, the pre-defined acronyms, and the `[Kate:]` annotation convention. `session-handoff` appends new standing rules to it as the monitor establishes them, so the rules she used to repeat every session now load automatically. **Rules are never deleted from it.**

### The `[Kate:]` annotation convention

The monitor annotates observation files in Google Docs (red font, inline notes), then exports to plain text — which loses the color. The `[Kate:]` prefix is the official annotation method that survives the export: any skill reading an observation or inventory file extracts every `[Kate:]` note, surfaces a "Kate's Annotations" summary, and treats each as a binding instruction.

## Project files these skills expect

The skills draft from the per-care-area source files and reference the prior filed reports + CD text. In Cowork these live on the mounted Drive folder (`Hibiscus Court Reports`):

- `02-source-evidence/<facility>/<NN>-<care-area>.md` — **drafting source of truth**, full names-removed observation detail for one facility + care area, with a `Record # | obs ID` per observation. One file in, one section out.
- `01-reference/consent-decree-paragraphs.md` — verbatim CD text; supplies each block's topic and the full paragraph list of the measure (including no-evidence paragraphs).
- `01-reference/` prior filed reports (Baseline June 2025, 12-Month January 2026) — VOICE / DENSITY / GRADE-CONTINUITY model only, never a source of current facts (our evidence is a later period).
- `01-reference/observation-index-…csv` / `evidence-by-paragraph-…csv` — lookup indexes for `obs-lookup` and tracing.
- `00-instructions/gold-standard-sections.md` — the controlling paragraph-ordered exemplar; bundled with `section-writer` too.
- `kate-rules.md` — the cumulative rulebook every skill reads; bundled at the plugin root and mirrored to `00-instructions/` on the Drive. `handoffs/HANDOFF-<section>-<date>.md` carries cross-session context (`session-handoff`).

All files have patient names removed. Original records stay in the team's secure vault — ask the team lead for un-redacted lookups. (The earlier `evidence-report-<facility>-<date>.md` summaries are DEPRECATED for drafting — they compressed clinical detail to ~2% and caused thin, fabrication-prone drafts.)

## Ground rules baked into every skill

- **Making compliance determinations is the monitor's job.** The section proposes a grade per paragraph, anchored to current findings + the prior period's grade; the monitors confirm or change every grade in the reconciliation pass. Draft grades are PROPOSALS, never asserted autonomously, and the table never contradicts the NOTES.
- **Evidence is narrated, never cited in the prose.** Observation IDs and Record #s appear ONLY in the NOTES crosswalk — never in the filed text. Every substantive finding still traces to a crosswalk line; an untraceable finding does not belong in the draft.
- **Write only from the source file.** No invented facts, numbers, dates, or quotes. External data not in the observations (CMS QM %, PBJ tables, audit results) is flagged in NOTES for the monitor to supply, never made up.
- **Flat declarative voice.** No essayistic build, no consequence-editorializing, no "spirit of," no charged adjectives, no external-literature citation unless it is in the source — counts and specifics instead of intensity words.
- **Concerns first, positive findings last.** Within every paragraph block, deficiencies and concerns lead; corrective effort and genuine credit close the block. (This reverses the retired credit-first framing.)
- **Names-free, unit-free, generalized.** Residents anonymous; staff by role/title; no specific unit/wing names in prose; medications and lab values generalized unless the exact one is the finding's subject; `[RESIDENT]` placeholders never altered or guessed at; monitoring-team names only on the cover page.
- **The monitor's standing rules always apply.** Every skill reads [`kate-rules.md`](./kate-rules.md): no unit names, month/year only, DVA not DMAVA, no re-expansion of pre-defined acronyms, POS = physician order set, the excluded-observations list, the banned-phrases table, and file-change confirmation after every edit.
- **The NOTES fence is absolute.** All drafting aids live below `— NOTES TO THE MONITOR (delete before filing) —`, organized into the eight named subsections; the prose above is clean, file-ready text. Exact dates and any citation-tied unit name live only in the NOTES crosswalk, never in the prose.
