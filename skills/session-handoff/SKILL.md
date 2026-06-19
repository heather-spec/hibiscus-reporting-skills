---
name: session-handoff
description: >-
  Carries Hibiscus court-report drafting context across Claude sessions so the monitor never re-teaches
  the same rules, acronyms, observation selections, or grade trends. Two jobs: at session START, load
  the cumulative kate-rules.md and the most recent handoff document before any drafting; at session END
  (or when the monitor signals she is wrapping up), generate a self-contained handoff document to a known
  location AND append any rules the monitor established this session to kate-rules.md. Use when a Hibiscus
  session begins, when the monitor says she is finishing a section or wrapping up, when she asks for a
  handoff / resume document, or when she establishes a new standing rule mid-session. Do NOT use to draft
  a section (section-writer) or build an observation inventory (obs-inventory).
---

# Session Handoff

Context loss between sessions is the monitor's single biggest time sink. Claude sessions do not carry state, so a fresh session knows nothing the last one established — voice preferences, acronym definitions, which observations were selected, compliance-grade trends, the rules the monitor had to repeat. She invented a manual handoff workaround; this skill makes it automatic and pairs it with the cumulative `kate-rules.md` so the standing rules load every time without being asked.

This skill does **two things**: **session-start intake** (load context) and **session-end handoff** (save context + update the rulebook). It never drafts prose and never invents facts — it records what this session actually established.

---

## 1. Session-start intake (do this BEFORE any drafting)

When a Hibiscus session begins — the first time the monitor asks for an inventory, a draft, a voice check, a baseline weave, or any section work — load context first:

1. **Read `kate-rules.md`** (the cumulative rulebook at the plugin root / in `00-instructions/` on the mounted Drive). These rules are always-on; they govern every skill. Surface a one-line confirmation: "Loaded Kate's rules (N hard rules, M banned phrases, K exclusions)."
2. **Find and read the most recent handoff document** (`handoffs/HANDOFF-<section>-<YYYY-MM-DD>.md`, newest by date, or the path the monitor names). Load: voice/style preferences, acronym list, observations selected and their evidence grades, compliance-grade trends and any grade uncertainty, in-session rule additions, and the file paths it lists.
3. **Confirm the resume point in one short summary** — which section/facility was in progress, what was done, what comes next — and ask the monitor to confirm before continuing. Do not silently assume; the handoff is a starting point, not an instruction to act unattended.

If no handoff exists yet, say so and proceed from `kate-rules.md` alone. If `kate-rules.md` is missing, say so plainly — do not draft without the standing rules.

---

## 2. Session-end handoff (when the monitor wraps up a section or signals she is done)

When the monitor finishes a section or says she is wrapping up, generate a **self-contained** handoff document — written so a fresh session that has never seen this conversation can pick up exactly where she left off. Save it to `handoffs/HANDOFF-<section>-<YYYY-MM-DD>.md` (ask for the date if you cannot determine it; never fabricate one) and confirm the save in the `Applied:` format (`kate-rules.md` §6).

The handoff MUST include every one of these — omitting one recreates the context loss this skill exists to prevent:

1. **Voice / style preferences established this session** — anything the monitor corrected or confirmed about tone, ordering, density, or phrasing.
2. **Acronyms** — the pre-defined list (ACEO, DON, LPN, EMR, TAR, DVA, CMS, CFR) plus any added this session, with expansions for any genuinely new term of art.
3. **Observations selected and their evidence grades** — which obs_ids / Record #s were drawn on for which CD paragraphs, with the strength rating used.
4. **Compliance-grade trends and grade uncertainty** — the proposed grade per paragraph, the prior-period anchor, trajectory (improving / holding / declining), and every paragraph flagged uncertain or deferred to the monitors.
5. **Rules the monitor added or modified this session** — verbatim. (Also append these to `kate-rules.md` — see §3.)
6. **File paths touched** — every draft, inventory, source file, and annotation file, with what each is.
7. **A resume prompt** — a ready-to-paste prompt a fresh session can use to continue: which section/facility is next, what state it is in, what to do first.

Keep it factual and specific. The handoff records what happened; it does not draft ahead or guess at grades the monitor has not set.

---

## 3. Maintain the cumulative rulebook (`kate-rules.md`)

When the monitor establishes a new standing rule — anything she says should hold for *all* future sections, not just this one — **append it to `kate-rules.md`** so it loads automatically forever after. This is what stops the 8+ rules she currently repeats by hand from being repeated again.

- Add hard rules under §1, banned phrases under §3, and newly excluded observations under §4 (Exclusions), matching the file's existing format.
- **Never delete or weaken an existing rule.** If a new instruction narrows or supersedes an old one, add the new rule and note the relationship; do not quietly drop the old text.
- After editing, confirm in the `Applied:` format and quote the exact rule text you added, so the monitor can verify it landed correctly.
- A rule that is genuinely one-section-only goes in the handoff (§2.5), not in `kate-rules.md`. When unsure whether a rule is standing or one-off, ask.

---

## 4. Where these files live

- **`kate-rules.md`** — plugin root (bundled with the skills) and/or `00-instructions/` on the mounted Drive. The always-on rulebook.
- **`handoffs/HANDOFF-<section>-<YYYY-MM-DD>.md`** — a `handoffs/` folder beside the drafts on the mounted Drive. Newest by date is the active resume point.

If the monitor keeps these elsewhere, follow her paths and record them in the handoff so the next session finds them.

---

## 5. Hard rules

1. **Load `kate-rules.md` and the latest handoff before drafting** — every session, before the first section task.
2. **The handoff is self-contained** — a fresh session needs nothing but the handoff and `kate-rules.md` to resume. Include all seven §2 fields.
3. **Append new standing rules to `kate-rules.md`; never delete a rule.** One-off rules go in the handoff only.
4. **Record, do not invent.** The handoff captures what this session established — selected observations, proposed grades, stated preferences. It never fabricates a grade, date, or selection the monitor did not make.
5. **Confirm every file write** in the `Applied:` format (`kate-rules.md` §6), quoting any rule text added to the rulebook.
