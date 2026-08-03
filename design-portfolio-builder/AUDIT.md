# Audit Rubric

The same rubric, used three times in a session: triaging incoming material (Phase A), naming the biggest gap before drafting, and scoring the finished draft (wrap-up).

## Dimensions

Rate each Strong / Adequate / Weak / Red Flag, calibrated to the target level's bar from `CONTEXT.md`:

- **Narrative structure** — does it follow (or intentionally adapt) the `FRAMEWORK.md` skeleton, with the problem framed before the UI and the decisions foregrounded over the activity log?
- **Evidence of impact** — is there a real, specific outcome? A missing number handled honestly (see `FRAMEWORK.md`'s "Handling unmeasured outcomes") is Adequate at worst; a missing number papered over with vague language ("well received") is Weak; a fabricated-sounding number with no source is a Red Flag.
- **Decision-making clarity** — are the 2-3 real decisions visible, along with what was rejected and why? A case study that reads as "here's what shipped" with no visible alternative is Weak regardless of how polished the writing is.
- **Retrospective honesty** — is there a genuine "what I'd change," not a humble-brag disguised as one ("I'd do it exactly the same, we just needed more time" is a Red Flag dodge)?
- **Craft & presentation notes** — visual clarity of whatever artifacts exist (this skill can't see images, so ask the user to describe them and flag presentation concerns: is the visual polished enough for the target company's bar per `CONTEXT.md`, is there enough visual evidence at all, is text-to-image balance reasonable).
- **Level-fit** — does the scope and center of gravity of the story actually match the target level's bar (`CONTEXT.md`), not a level below or above it? A Staff-level story that reads as "I designed a great feature" with no cross-team influence is under-scoped; an Entry-level story straining to sound strategic is over-reaching.

## Rating definitions

- **Strong** — clears the target level's bar outright; would read well to a hiring committee.
- **Adequate** — the bones are right but thin in one dimension; fixable with the material already gathered.
- **Weak** — descriptive rather than decisive, missing real evidence, or under/over-scoped for the level.
- **Red Flag** — a fabricated-sounding claim, a dodged retrospective, or a narrative that doesn't hold together on inspection (e.g. claimed impact contradicts the stated constraints).

## Using the rubric mid-session (Phase A triage)

Map the three-bucket triage from `DISCOVERY.md` onto these dimensions: a section landing "usable as-is" should already be Strong/Adequate on its relevant dimension; "needs modification" is Adequate/Weak; "missing entirely" starts as a Red Flag/Weak until discovery fills it. Don't let a Red Flag survive into Phase B unaddressed — resolve it in discovery or flag it explicitly to the user as an open risk they're choosing to carry.

## Wrap-up scorecard

Produce this at the end of Phase B:

```
## Case Study Audit — [project name] · [level/track] · [company size] · [B2B/B2C] · [competitiveness]

**Dimension scores:**
- Narrative structure: [rating]
- Evidence of impact: [rating]
- Decision-making clarity: [rating]
- Retrospective honesty: [rating]
- Craft & presentation notes: [rating] — [specific note]
- Level-fit: [rating]

**Strongest section:** [which, and why]

**Weakest section (if any remain):** [which, why, and what it would take to fix]

**Open risks carried into the final draft:** [e.g. "no real outcome number — framed honestly per FRAMEWORK.md" — or "none"]

**Next step:** Run `/design-interview-prep` in portfolio-review format to pressure-test this case study live against real interviewer follow-ups.
```

## Rules

- Never inflate a rating to be encouraging — the debrief's value is the same honest calibration `design-interview-prep` uses.
- Calibrate to the *selected* level, not a generic "good portfolio" bar — an Entry-scoped story that clears the Entry bar is Strong, full stop.
- If a Red Flag is knowingly carried into the final draft (user chooses not to fix it), say so plainly in "open risks" rather than silently omitting it.
- **Invariant across all three coaching tones (CONTEXT.md):** a Supportive Coach session can deliver this scorecard more gently, and a Brutal session more bluntly — but every dimension score, the open-risks list, and the overall read must be identical to what a different-toned run of the same material would produce. Tone changes how a gap is said; it never changes whether it's scored as one.
