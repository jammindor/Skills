# Skills
Claude Skills by me. There are a few categories 


# Design Interview Skills

Claude Code skills for product/UX design interview prep, built for a tight 2026 hiring market: fewer open reqs, no partial credit for vague answers, and generalist range (business, metrics, cross-functional reasoning) expected as the baseline at Senior+.

Two companion skills, each documented in its own folder:

- **[`design-interview-prep/`](design-interview-prep/)** — a live product/UX design interview simulation. Use once you have a story to pressure-test.
- **[`design-portfolio-builder/`](design-portfolio-builder/)** — a two-phase coaching session that builds or tightens the portfolio case studies you'd bring into that interview. Use when the story doesn't exist yet, or exists as rough/partial material.

Both share the same level ladder and company-context dials, and both offer a selectable tone (**Brutal** / **Professional** / **Supportive Coach**) so the bar of entry to trying either one is low, without softening the substance of either skill's feedback.

> **Note on provenance:** because the level bars in both skills are derived from Twilio-internal career framework documents, keep this repo internal to Twilio (private repo / internal org) rather than publishing it externally, unless you've re-derived the level bars from a public source.

## Install

Copy either (or both) skill folders into your Claude Code skills directory:

```bash
cp -r design-interview-prep ~/.claude/skills/
cp -r design-portfolio-builder ~/.claude/skills/
```

Or, to scope a skill to one project/repo instead of your whole user account, copy it into that project's `.claude/skills/` folder instead.

See each skill's own README for what it does, how to use it, and its file manifest: [`design-interview-prep/README.md`](design-interview-prep/README.md), [`design-portfolio-builder/README.md`](design-portfolio-builder/README.md).

## Customizing

If your org has its own leveling doc, swap the ladder definitions in each skill's `CONTEXT.md` — everything else is written to work off whatever ladder is defined there, not hardcoded to Twilio's levels.
