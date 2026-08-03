# design-interview-prep

A Claude Code skill that runs a live product/UX design interview simulation — any level from Entry IC through Senior Director, in a selectable tone from Brutal to Supportive Coach — with GMAT-style adaptive difficulty and a graded debrief at the end.

Built for design teams practicing in a tight 2026 hiring market: fewer open reqs, no partial credit for vague answers, and generalist range (business, metrics, cross-functional reasoning) expected as the baseline at Senior+.

> Companion skill: [`design-portfolio-builder`](../design-portfolio-builder/) builds or tightens the case studies you'd bring into this interview, if the story doesn't exist yet. Use that first if you don't have a story ready to pressure-test.

## What it does

- **Live simulation, not a quiz.** Claude plays a hiring panelist, asks one question at a time, and pushes back at least once on every answer before moving on.
- **Selectable tone.** Choose **Brutal** (blunt, no cushioning), **Professional** (the default — firm and rigorous, like a genuinely good real-world interviewer), or **Supportive Coach** (same rigor, framed as collaborative practice — lower the barrier for anyone hesitant to try the harder end of this tool). The substance and the honesty of the final debrief never change across tones — only the voice does.
- **Adaptive difficulty.** Answer well and the next question gets harder; answer weakly and it eases off — like the GMAT, the session converges on your real level instead of staying fixed. You choose at setup whether that climb is visible each round or only revealed in the final debrief.
- **Calibrated to a real level ladder**, not a generic "good designer" bar — see [Level ladder](#level-ladder) below.
- **Four rotating interview formats** — portfolio review, whiteboard design challenge + critique, behavioral & leadership, business & metrics acumen — plus a required warm-up every session always runs: your working relationship with PM/Engineering, and a tool-fluency check (Claude Code or similar, Git/GitHub including opening your own PRs, Storybook or equivalent).
- **Session dials**: company size (solo/startup, Series B-D, enterprise), B2B vs. B2C, and how competitive the company's specific market segment is — these recolor the existing question bank live rather than needing a separate set of questions per combination.
- **A real debrief**, not just "good job" — per-question ratings, the calibrated level you actually tested at and your trajectory getting there, scores against four competency dimensions, and a rewritten model version of your weakest answer.

## Install

Copy this folder into your Claude Code skills directory:

```bash
cp -r design-interview-prep ~/.claude/skills/
```

Or, to scope it to one project/repo instead of your whole user account, copy it into that project's `.claude/skills/` folder instead.

## Use it

In Claude Code, either:
- Type `/design-interview-prep`, or
- Just ask in plain language — "let's practice a design interview," "grill me for a design interview," "mock interview me for a UX role."

Claude will ask a short setup intake (tone, level & track, company size, B2B/B2C, market competitiveness, which format(s), and whether to show the difficulty climb live or keep it hidden), then run the session.

## Level ladder

**IC track:** Entry → Senior → Staff → Principal
**Management track:** Associate Manager → Manager → Senior Manager → Director → Senior Director

The IC ladder is condensed from Twilio's internal Product Design Career Development Framework. The Management ladder is condensed from Twilio's generic, cross-role Manager CDF (not design-specific) — both are paraphrased/summarized in [`CONTEXT.md`](CONTEXT.md), not reproduced verbatim.

> **Note on provenance:** because the level bars are derived from Twilio-internal career framework documents, keep this repo internal to Twilio (private repo / internal org) rather than publishing it externally, unless you've re-derived the level bars from a public source.

## File manifest

| File | Purpose |
|---|---|
| `SKILL.md` | Orchestration — session flow, setup intake, wrap-up trigger |
| `PERSONA.md` | Interviewer character, pushback rules, tone guardrails |
| `FORMATS.md` | Required warm-up + the four rotating format question banks |
| `ADAPTIVE.md` | The GMAT-style difficulty ladder and tier adjustment rules |
| `RUBRIC.md` | Scoring dimensions and the debrief template |
| `CONTEXT.md` | Level ladder bars, company size, B2B/B2C, market-competitiveness, and tone calibration |

## Customizing

If your org has its own leveling doc, swap the ladder definitions in `CONTEXT.md` — everything else (the adaptive tier math in `ADAPTIVE.md`, the formats in `FORMATS.md`) is written to work off whatever ladder is defined there, not hardcoded to Twilio's levels.
