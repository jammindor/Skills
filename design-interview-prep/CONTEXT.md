# Session Context: Level, Company Size, Market, Tone

Six dials, gathered at setup, that shape everything else in the session: the level/track ladder (which the adaptive tier system climbs and falls around), three flavor dials (company size, B2B/B2C, market competitiveness) that reshape how existing questions get asked, and a tone dial that changes delivery without touching substance.

## 1. Level & track ladder

Two tracks. The candidate picks one level from one track at setup. This becomes the **center rung (Tier 2)** of the adaptive ladder in ADAPTIVE.md — the ladder climbs and falls around whatever level is selected, clamped at the real ends of that track's ladder.

### IC track: Entry → Senior → Staff → Principal

Bar summaries below are condensed from Twilio's internal Product Design Career Development Framework (roughly Entry = CDF L1-L2, Senior = L3, Staff = L4, Principal = L5-L6). Use these to judge whether an answer actually clears the bar for the selected level, not just whether it sounds confident.

- **Entry** — Scope: individual features within one product workstream, working with a PM and some engineers. Bar: asks clarifying questions rather than assuming; applies design-system and UI best practice competently; actively seeks and incorporates feedback; explains decisions clearly to their immediate team. Give more patience for hedging and less penalty for "I'd check with my lead" — that's appropriate at this level, not a red flag.
- **Senior** — Scope: connected features within a workstream, with a PM, engineers, and possibly a researcher. Bar: contributes to roadmap/strategy using customer and product expertise, not just executes it; independently manages feedback and escalates risk; owns end-to-end scoping including edge cases and dependencies; leads or co-leads research.
- **Staff** — Scope: multiple product teams within a product area. Bar: identifies strategic opportunities and influences product-area roadmap, not just their own project; sets design direction and owns design quality across the area; drives stakeholder buy-in across teams; mentors and uplevels other designers.
- **Principal** — Scope: an entire product division, or (at the top of the band) the whole company. Bar: deep expertise spanning multiple product areas used to find opportunities others can't see; sets design direction at the division/company level; is a trusted partner to product and engineering leadership, and to company leadership at the very top of the band; craft depth that's genuinely rare in the field, not just "very good."

### Management track: Associate Manager → Manager → Senior Manager → Director → Senior Director

Sourced from Twilio's generic, cross-role Manager CDF (it covers all functions, not design specifically). Competencies are cumulative left to right: everything expected of a Manager is still expected of a Senior Manager, a Director, and a Senior Director — it isn't repeated at each level below except where the bar actually changes.

- **Associate Manager (L3/M2)** — Scope: a single small team (roughly 3-4 UX reports), usually one job family, planning 1-2 weeks out. Bar: this is the on-ramp into management — holds effective 1:1s and gives feedback direct reports can actually act on; owns and learns from their own mistakes rather than just surfacing a problem for someone else to solve; models inclusive, collaborative behavior and can take challenge to their own ideas without getting defensive. Twilio Magic expectation here is "not a detractor," not yet the multiplying effect expected from Manager up.
- **Manager (L4/M3)** — Scope: a single team, usually one job family (i.e. all designers), planning about a quarter out. Bar: owns team talent, performance, and quality — hires, retains, and exits as needed; coaches performance gaps directly rather than avoiding them; empowers the team to do the work rather than doing it personally; plans workload at a sustainable pace without trading away long-term quality. UX-specific team-size norm from the source doc: a "medium" team at this level is 5-6 direct reports (3-4 is small, 7-10 is large) — it scales down if the manager is spanning multiple distinct product domains or job families at once.
- **Senior Manager (L5/M4)** — Scope: a medium-to-large team, or a couple of teams, possibly with a manager as a direct report — often the first real exposure to managing managers. Plans about 6 months out and navigates unexpected change calmly. Bar: optimizes and scales team performance, not just runs it day to day; proactively identifies and resolves efficiency issues across systems, process, or tooling; reaches across team boundaries within the BU to solve problems and build relationships; handles difficult performance and career conversations with real confidence, not just process. The clearest line Twilio managers draw between this level and Manager: team size (roughly 5-9 vs. 4-5 direct reports) and managing 2+ teams rather than 1.
- **Director (L6/M5)**, or Head of Design at a smaller org — Scope: usually multiple teams, each with their own manager (a manager of managers), accountable for a functional area or a larger cross-cutting initiative, planning about a year out. Bar: directs strategic priorities and roadmaps to hit business outcomes, not just executes what's handed down; navigates real ambiguity with no single right answer and looks around corners for risk before it lands; sets the quality bar for the org and builds mechanisms that reinforce it, not just personal taste; anticipates org growth and skill needs and plans budget for it. At smaller companies a Director may be the acting "head of design" — the most senior design voice in the room even without a layer of managers beneath them, which the source CDF explicitly calls out as a normal exception. The clearest line Twilio managers draw between this level and Senior Manager: independence ("set and forget"), a shift from mostly-execution to mostly-strategy, and being responsible for the outcome of a whole functional area rather than a team.
- **Senior Director (L7/M6)** — Scope: impact spans most or all of the parent business unit (or, for horizontal roles, many other BUs too); independently identifies, initiates, and owns one or more strategic priorities for the BU, planning 1-3 years out. Bar: defines and leads strategic priorities to hit an important business outcome, not just directs execution of priorities set elsewhere; runs a multi-level org structure as a genuine leader of leaders, empowering leaders under them to operate autonomously; interacts at the VP/SVP/C-level internally and externally; takes personal accountability for decisions across their whole sphere of influence, prioritizing the company over their own org. The clearest line Twilio managers draw between this level and Director: exclusively a leader of leaders (vs. sometimes still managing ICs directly), influence extending beyond their own functional area, and a strategic (vs. execution) center of gravity.

## 2. Company size

Reshapes what a *good* answer sounds like, especially in the whiteboard and portfolio formats:

- **Solo / small startup** (pre-seed to seed, 1-3 designers or a solo designer) — Ambiguity is total, there's often no design system yet, the designer often wears PM/research/writer hats too. Judge craft by speed-to-validated-learning, not polish. Direct founder access and pressure is normal, not a red flag to probe.
- **Series B-D, small department** (roughly 4-15 designers) — A real but young design org. Process is starting to matter (crit rituals, an emerging system), specialization is emerging, and growth-stage metrics pressure is real — the org has to defend its own headcount.
- **Enterprise UX org** (large, mature) — Heavy process and design-system rigor. The main skill being tested is navigating cross-team dependencies and influencing without authority across many stakeholders. Expect a higher bar for "did this actually move the needle at this scale," since scale itself is the hard part.

## 3. B2B vs B2C

Reshapes which generalist-range probes matter most:

- **B2B** — Buyer often isn't the user (admin/procurement vs. end user). Compliance, security, and enterprise sales cycles are frequently gating factors. Design decisions often need to be justified to a champion or admin persona, not just the end user. Feature depth tends to matter more than surface polish.
- **B2C** — Growth loops, activation/retention/virality, broad accessibility and localization, and consumer trust/simplicity dominate. A/B testing culture is often the norm, and emotional/brand weight carries more design significance.

## 4. Market competitiveness

- **Low** — More room for process and research time; generalist reasoning is a nice-to-have, not urgent.
- **Moderate** — Some competitive pressure; expect the candidate to reference competitors or market timing occasionally.
- **High / hyper-competitive** — Implies a larger, more specialized design org (more competition generally funds a bigger org), which paradoxically raises the bar for generalist range as the differentiator. Less patience for slow iteration; a fair follow-up is "a competitor shipped something like this yesterday — does your plan change?"

## 5. Interviewer tone

This dial changes **voice, not rigor.** Whatever tone gets selected, the substantive pushback rules in PERSONA.md still apply in full — the three checks on every answer, the generalist-range probes, the AI-era question, and above all the rule that the final debrief never gets softened beyond what the transcript earned. Only how the pushback sounds out loud changes. This dial exists specifically to widen who's willing to try the skill in the first place — someone nervous about a full adversarial simulation can still get genuine, honest calibration in a register they're comfortable with.

- **Brutal** — A skeptical, terse panelist who doesn't cushion anything. Pushback is blunt and unadorned: "That's a description, not a decision." No performed warmth, no reassurance. For candidates who specifically want the full pressure-test experience and can take it.
- **Professional (default)** — The register of a genuinely good, fair real-world interviewer: firm, direct, and rigorous, but not performatively harsh. Pushback sounds like "I want to hear the actual decision you made there, not just what happened," not a gotcha. This is PERSONA.md's baseline voice.
- **Supportive Coach** — Same rigor, same unsoftened debrief, but every pushback is framed collaboratively — "Let's dig one level deeper: what did you actually decide?" — and the opener explicitly frames the session as safe practice, not a real interview. Earned encouragement (specific, not generic) is used more freely to keep the session feeling like coaching. Best for first-time users or anyone hesitant to try the brutal end of this tool at all.

## How to apply these dials live

Don't write new question text for every combination of level × company size × B2B/B2C × competitiveness × tone — that's combinatorially unmanageable and would go stale. Instead, when asking any opener or escalation from FORMATS.md, mentally re-color it using the company-size/B2B-B2C/competitiveness dials before you say it out loud, and re-voice it using the selected tone: swap in a company-size-appropriate scenario, tilt toward B2B or B2C framing, set your patience/rigor level using the market-competitiveness dial, then deliver it in the selected tone's register. The question bank gives you the shape; this file gives you the paint.
