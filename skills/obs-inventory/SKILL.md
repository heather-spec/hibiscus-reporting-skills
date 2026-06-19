---
name: obs-inventory
description: >-
  Builds the pre-draft observation inventory for one Hibiscus care-area section in a single step: reads
  the care-area source file, organizes its observations by evidence strength into the monitor's ranked
  inventory format (a short narrative plus a strength-sorted table), AND produces the coverage map of which
  Consent Decree paragraphs of the measure carry evidence and which have none. Extracts any [Kate:]
  annotations and surfaces them first. This collapses the monitor's old multi-step "pull observations →
  inventory → coverage map" sequence into one output, ready to annotate and then hand to section-writer.
  Use when a monitor asks for an observation inventory, an evidence inventory, a coverage map, a ranked
  list of observations for a care area, or "what do we have for [section]." Do NOT use to draft the section
  prose (section-writer) or to look up a single obs_id (obs-lookup).
---

# Observation Inventory

You build the **inventory** that comes before a draft: a ranked, evidence-strength-organized view of one care area's observations, plus a coverage map of the measure's Consent Decree paragraphs. The monitor invented this format and it works; your job is to produce it in one step so she is not running a manual sequence of prompts.

This is a **pre-draft analysis tool.** It organizes and maps the source; it does not write report prose, propose grades, or invent anything the source does not contain.

**Load `kate-rules.md` first** (the standing rulebook) so the inventory respects the exclusions and the monitor's rules from the outset.

---

## 0. Your input

**The care-area source file** — the full, names-removed observation detail for one facility and one care area, each observation carrying a `Record # | obs ID` header. This is the only source. If it is missing or covers a different care area than asked, stop and say so.

If the file carries **`[Kate:]`-prefixed annotations** (`kate-rules.md` §5), extract them and present a **"Kate's Annotations"** summary at the very top, before the inventory — quote each note and the observation it attaches to. They are binding instructions for the draft that follows.

---

## 1. Apply the exclusions first

Before ranking, drop any observation on the Exclusions list in `kate-rules.md` (currently the **MDS missed-hospitalization observation**). Keep it visible — list it under a short **"Excluded (resolved outside the report)"** heading with its obs_id and one line — but do not rank it for drafting and do not map it into the coverage map.

---

## 2. The ranked inventory (organized by evidence strength)

Sort the remaining observations into evidence-strength tiers and present them so the monitor sees the strongest evidence first:

- **Strong** — directly observed, dated, specific, corroborated; carries a finding on its own.
- **Moderate** — supportive but partial (single record, second-hand, or needs a companion observation).
- **Thin** — a mention or a one-off; flag for a thin-evidence note rather than a standalone finding.

Output two parts:

1. **A short narrative** (a few sentences) naming the dominant evidence threads for this care area — where the weight of the evidence sits — without drafting any report prose.
2. **A strength-sorted table**, strongest first:

   | Strength | Record # / obs ID | Date | Type | One-line of what it shows | CD ¶¶ |
   |---|---|---|---|---|---|

   Use the source's own dates and types; one row per observation. This table is also the seed of the section's NOTES crosswalk, so keep the Record#/obs IDs exact.

Generalize nothing and editorialize nothing here — the inventory is a faithful index, not a draft. (The report-language rules in `kate-rules.md` apply when section-writer turns this into prose.)

---

## 3. The coverage map (which CD paragraphs have evidence)

Using the Consent Decree reference for the full paragraph list of the measure, map the inventory onto the paragraphs:

| CD ¶ | Topic (from the decree) | Evidence? | Strongest observation(s) |
|---|---|---|---|

- List **every** paragraph in the measure, in ascending order — including the ones with no evidence (mark them **NO EVIDENCE → carry forward**). This is what tells the monitor, and section-writer, which paragraphs will be real blocks and which will be placeholders.
- A paragraph's "Strongest observation(s)" cell points back to the inventory rows, so the draft step inherits the mapping.

---

## 4. Pipeline awareness — hand off to the next step

The monitor's pipeline is: **inventory → annotate in Google Docs → save annotations → draft.** After producing the inventory and coverage map, tell her the next step explicitly:

> "Inventory and coverage map ready. Next: annotate the observations in Google Docs using the `[Kate:]` prefix (red font is fine — the prefix is what survives the plain-text export), save the annotated file, then run section-writer to draft. I will read the `[Kate:]` notes and load `kate-rules.md` and the latest handoff automatically."

Save the inventory to the drafts location if asked, and confirm the write in the `Applied:` format (`kate-rules.md` §6).

---

## 5. Hard rules

1. **One step, two outputs** — the ranked inventory (narrative + strength-sorted table) and the full coverage map, every time.
2. **Apply the `kate-rules.md` exclusions** before ranking; keep excluded observations visible but unranked and off the coverage map.
3. **Surface `[Kate:]` annotations first**, as binding instructions for the draft.
4. **Faithful index, not a draft** — no report prose, no proposed grades, no generalization or editorializing, nothing the source does not contain. Record#/obs IDs stay exact (they seed the crosswalk).
5. **Every paragraph of the measure appears in the coverage map**, no-evidence ones marked carry-forward.
6. **Point to the next pipeline step** (annotate → draft) and confirm any file write.
