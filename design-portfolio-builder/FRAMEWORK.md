# Case Study Framework

The section skeleton every case study gets built or fitted into, variants for different project shapes, and how to scale depth to the target level from `CONTEXT.md`.

## Standard section skeleton

1. **Context & problem** — the business/user problem, stated before any UI. Who has this problem, why it matters now, and to whom (the reader should know the stakes before seeing a single screen).
2. **Constraints** — timeline, headcount, technical debt, org politics, ambiguity. This is what makes the later decisions legible as decisions rather than obvious choices.
3. **Process & key decisions** — not a chronological activity log. The 2-3 decisions that actually mattered, each stated as a choice made under the constraints above.
4. **Tradeoffs & rejected alternatives** — what else was on the table and why it lost. This is the single most commonly missing section — flag it hard in `DISCOVERY.md` triage if absent.
5. **Outcome & metrics** — the actual number. If it was never measured, say that plainly (see "Handling unmeasured outcomes" below) rather than writing around it vaguely.
6. **Retrospective** — what they'd do differently. A "nothing" answer is a red flag per `AUDIT.md` — push for a real one in discovery.
7. **What only they brought to this** — the AI-era differentiator: judgment, taste, a call made under ambiguity that a generated flow couldn't have made. Not required in every case study, but strongly recommended for Senior+.

## Variants by project shape

- **Single feature** (typical for Entry/Senior) — Keep the skeleton tight; the "constraints" and "rejected alternatives" sections can be short. Depth should live in the decision and retrospective sections.
- **0-to-1** — Context & problem expands to cover the ambiguity itself (there was no existing pattern to follow); process should show how validation happened without a base to test against.
- **Redesign / growth-driven** — Context should include the metric pressure that triggered the redesign; outcome section should show before/after, not just after.
- **Leadership & strategy** (Staff+/Management track) — Replace "process & key decisions" with a story about setting direction, driving buy-in across teams, or a talent/team decision. The "artifact" being showcased may be a roadmap, a design principle that got adopted org-wide, or a team outcome rather than a shipped screen — that's expected at this level, not a gap. Don't assume this variant just because the target level is Staff+ — let what actually came out in `DISCOVERY.md`'s intake decide it: if the material describes a single feature scope even at Staff+, use the single-feature skeleton and let level-fit scoring in `AUDIT.md` surface that as a scope gap, rather than forcing a strategy framing onto material that doesn't support it.

## Scaling depth to level (see CONTEXT.md)

- **Entry** — Scope stays small; strength comes from clarity of reasoning and evidence of incorporating feedback, not scale.
- **Senior** — Scope should show independent ownership across a connected set of features; the "why" should draw on customer/product context, not just internal logic.
- **Staff** — Scope should span teams; the narrative center of gravity shifts from "I designed X" to "I identified/directed X across an area."
- **Principal** — Scope should span a division or company; craft depth and strategic rarity should be evident without needing to be asserted.
- **Management track** — Center the story on the team/org outcome, not personal craft — see the leadership variant above.

## Working from existing material

When a section is "needs modification" (per `DISCOVERY.md` triage), decide out loud with the user whether this is:
- **A tightening pass** — the content and framing are right, it just needs to be shorter/clearer/better ordered. Edit their words; keep their voice.
- **A reframe** — the underlying facts are right but the shape is wrong (e.g. it's currently a chronological activity log; it needs to become a decision-and-tradeoff narrative). Substantial rewrite, but built entirely from what they told you — don't introduce new claims.
- **A rebuild** — so little of the original is usable that starting over from the discovery answers is faster and cleaner than editing. Say so plainly rather than quietly discarding their draft.

## Handling unmeasured outcomes

If a real number genuinely doesn't exist, don't invent one and don't write around it with vague language ("well received," "positive feedback"). Two honest options: (a) state the leading/qualitative signal that does exist and name the gap directly ("we didn't instrument this — anecdotally, support tickets on this flow dropped, but I can't give you a number"), or (b) if truly nothing was tracked, say that as the retrospective lesson itself ("the biggest thing I'd do differently is instrument this before shipping"). Calibrate how damaging this is using `AUDIT.md` and the target level from `CONTEXT.md` — a missing number is a bigger gap the more senior the target level.

## Handling a genuinely-missing rejected alternative

Push in discovery first — most people did weigh another option and just never framed it as one ("did anything else get discussed and dropped, even informally?"). If there truly wasn't a considered alternative, don't invent one. Instead, either: (a) reframe the section around the constraint that made the choice feel obvious at the time, and name in the retrospective that no alternative was seriously explored ("in hindsight, I don't think I considered another approach here — that's worth flagging"), or (b) if the level is Staff+ where this gap is most damaging (see `AUDIT.md` and `CONTEXT.md`), treat this itself as the retrospective lesson and be direct with the user that this weakens the case study's fit for that level — don't smooth it over.

## Portfolio-level architecture (when building more than one case study)

- 3-4 case studies is typical; more dilutes rather than strengthens.
- Order matters — lead with the strongest, most level-appropriate story, not chronologically.
- Don't repeat the same "shape" of story twice (e.g. two 0-to-1 stories back to back) — pick the set that shows the widest range relevant to the target level and company dials.
- For Staff+/Management, at least one case study should center on influence/strategy/team rather than shipped craft alone.
