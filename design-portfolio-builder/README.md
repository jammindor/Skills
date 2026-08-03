# design-portfolio-builder

A Claude Code skill that coaches a product/UX designer through building or tightening a portfolio case study — in a selectable tone from Brutal to Supportive Coach.

Built for the same tight 2026 hiring market as its companion skill: no invented metrics, no papered-over gaps, and a case study honest enough to survive real pressure-testing.

> Companion skill: [`design-interview-prep`](../design-interview-prep/) runs a live, adversarial mock-interview simulation. Use this skill first if the story doesn't exist yet or exists only as rough/partial material, then pressure-test the finished case study over there.

## What it does

- **Works from whatever you actually have.** A rough draft, an old case study, resume bullets, a half-written deck, or nothing at all — the skill absorbs existing material first rather than assuming a blank page.
- **Selectable tone.** Same three options as `design-interview-prep` — **Brutal**, **Professional** (default), **Supportive Coach** — changing voice, never rigor: a flagged gap gets flagged in every tone, just said differently.
- **Two-phase session.** Phase A (Discovery) triages every case-study section as usable-as-is / needs-modification / missing, then asks targeted questions to fill the gaps. Phase B (Build) drafts the case study section by section, showing each one for feedback before moving on — never a full unreviewed dump.
- **Honest about what's missing.** No invented metrics or papered-over gaps — missing outcomes and missing rejected-alternatives get named and handled honestly (see [`FRAMEWORK.md`](FRAMEWORK.md)), calibrated to how damaging that gap is at the target level.
- **Calibrated to the same level ladder** as `design-interview-prep`, so a case study built here holds up when pressure-tested there.
- **A real audit**, not just polish — per-section ratings, a wrap-up scorecard across six dimensions, and any open risks the user chose to carry into the final draft, stated plainly rather than hidden.

## Install

Copy this folder into your Claude Code skills directory:

```bash
cp -r design-portfolio-builder ~/.claude/skills/
```

Or, to scope it to one project/repo instead of your whole user account, copy it into that project's `.claude/skills/` folder instead.

## Use it

In Claude Code, either:
- Type `/design-portfolio-builder`, or
- Just ask in plain language — "help me build my portfolio," "I need to write a case study," "can you tighten up this case study draft."

Claude will ask a short setup intake (tone, level & track, target company size/B2B-C/competitiveness, scope, and what raw material already exists), then run Phase A and Phase B. At the end, it'll suggest running `/design-interview-prep` in portfolio-review format to pressure-test the finished case study live.

## Level ladder

**IC track:** Entry → Senior → Staff → Principal
**Management track:** Associate Manager → Manager → Senior Manager → Director → Senior Director

The IC ladder is condensed from Twilio's internal Product Design Career Development Framework. The Management ladder is condensed from Twilio's generic, cross-role Manager CDF (not design-specific) — both are paraphrased/summarized in [`CONTEXT.md`](CONTEXT.md), not reproduced verbatim.

> **Note on provenance:** because the level bars are derived from Twilio-internal career framework documents, keep this repo internal to Twilio (private repo / internal org) rather than publishing it externally, unless you've re-derived the level bars from a public source.

## File manifest

| File | Purpose |
|---|---|
| `SKILL.md` | Orchestration — two-phase session flow, setup intake, wrap-up |
| `DISCOVERY.md` | Intake/triage technique and the gap-filling question bank |
| `FRAMEWORK.md` | Case-study section skeleton, project-shape variants, and portfolio architecture |
| `AUDIT.md` | Scoring rubric, used for triage, gap-calling, and the final scorecard |
| `CONTEXT.md` | Level ladder bars, company size, B2B/B2C, market-competitiveness, and tone calibration |

## Customizing

If your org has its own leveling doc, swap the ladder definitions in `CONTEXT.md` — everything else is written to work off whatever ladder is defined there, not hardcoded to Twilio's levels.
