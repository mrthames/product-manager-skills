---
name: roadmap-planning
description: Translate strategy and OKRs into a sequenced product roadmap. Use when you need to communicate what's next, why, and in what order.
---

# Roadmap Planning

Turn your strategy, OKRs, and backlog into a roadmap that stakeholders can understand and the team can execute against — in 2-4 hours instead of a multi-week planning offsite. Claude handles the synthesis and formatting. You handle the sequencing judgment and stakeholder reality.

## When to Use

- Start of a quarter when you need to communicate the plan
- After OKR setting, when objectives need to be mapped to deliverables
- When leadership asks "what are we building and when?"
- When multiple teams need to coordinate sequencing and dependencies
- After a strategy pivot when the previous roadmap is obsolete

## When NOT to Use

- You need to set the goals first — use OKR & Goal Setting
- You need to align on strategy before roadmapping — use Product Strategy & Vision
- You're planning a single sprint — use Sprint & Release Planning
- You need to prioritize the backlog before sequencing — use RICE/ICE in FRAMEWORKS.md

## The AI-Native Approach

| Step | Time | Claude Does | You Do |
|---|---|---|---|
| Gather inputs | 30 min | Structure OKRs, backlog, and constraints into a planning view | Provide context on dependencies and political realities |
| Sequence work | 45 min | Propose sequencing based on dependencies, risk, and value | Apply judgment on what ships when and why |
| Format the roadmap | 30 min | Generate roadmap views for different audiences | Validate accuracy and add narrative context |
| Stress-test | 30 min | Flag capacity conflicts, dependency risks, and coverage gaps | Confirm with engineering leads and stakeholders |

## Process

### Step 1: Gather Inputs (30 minutes)

A roadmap is only as good as its inputs. Start by bringing together everything that informs sequencing.

```
Help me build a roadmap for [time horizon: quarter / half / year].

Inputs:
- OKRs / goals: [paste or summarize your objectives and key results]
- Current backlog: [top initiatives, epics, or themes with rough sizing]
- Commitments: [anything already promised — customer commitments, partner deadlines, compliance dates]
- Team capacity: [number of teams/squads, any planned absences or ramp-ups]
- Dependencies: [cross-team dependencies, platform work, external integrations]
- Carry-over: [unfinished work from last cycle that still matters]

Structure this into a planning view:
- Group initiatives by which OKR/goal they serve
- Flag initiatives with no clear goal alignment
- Identify dependencies between initiatives
- Note rough sizing (S/M/L or sprint count) for each
```

### Step 2: Sequence Work (45 minutes)

This is the judgment-heavy step. AI proposes; you decide.

```
Propose a sequencing for this roadmap:

Sequencing criteria (in priority order):
1. Dependencies: what must ship before something else can start?
2. Commitments: what has a hard external deadline?
3. Value: what moves the highest-priority OKR the most?
4. Risk: what has the most uncertainty and should start earlier?
5. Quick wins: what can ship fast and build momentum?

For each time bucket [month / sprint / now-next-later]:
- What ships in this period
- Why it's sequenced here (which criteria drove the decision)
- What's at risk if it slips
- Dependencies on other teams or initiatives

Flag:
- Capacity conflicts (more work than team can absorb)
- Sequencing trade-offs (two things that should go first — which one wins?)
- Items that don't fit (lower priority, should be cut or deferred)
```

### Step 3: Format the Roadmap (30 minutes)

Different audiences need different views of the same plan.

```
Generate three roadmap views from the sequenced plan:

1. Now / Next / Later view (for the team):
   - Now: actively in progress or starting this sprint
   - Next: planned for the next 1-2 cycles
   - Later: on the radar but not yet committed
   For each item: name, goal it serves, owner, rough timeline

2. Timeline view (for leadership):
   - Monthly or quarterly columns
   - Initiatives mapped to time periods
   - Key milestones and decision points marked
   - Dependencies shown as connections
   Include: what we're betting on and what we're explicitly NOT doing

3. Theme-based view (for stakeholders and customers):
   - Grouped by strategic theme or user outcome
   - No internal implementation details
   - Focused on "what changes for you and when"
   - Appropriate level of commitment language (exploring / planned / committed)
```

### Step 4: Stress-Test (30 minutes)

```
Review this roadmap for:

Capacity:
- Does the work fit the team's capacity in each period?
- Are there periods that are overloaded?
- Is there buffer for unplanned work (bugs, incidents, support)?

Dependencies:
- Are any items sequenced before their dependencies are resolved?
- Are we depending on other teams? Have they committed?
- What happens to downstream work if an upstream item slips?

Coverage:
- Does every OKR have at least one initiative mapped to it?
- Are any OKRs under-invested (one small initiative for a stretch goal)?
- Are we spreading too thin across too many goals?

Reality check:
- What are we NOT doing? Is the team clear on what's been cut?
- Where are we most likely to be wrong about estimates?
- What's our contingency if the top-priority item takes 2x longer?
```

## Output

- Structured planning view with initiatives mapped to goals
- Sequenced roadmap with rationale for ordering
- Three audience-specific roadmap views (team, leadership, stakeholder)
- Stress-test analysis with capacity, dependency, and coverage flags

## Common Pitfalls

1. **Roadmap as commitment.** A roadmap is a plan, not a promise. Use commitment language carefully — "exploring," "planned," and "committed" mean different things. Over-committing destroys trust when plans change.
2. **No room for the unexpected.** If your roadmap fills 100% of capacity, the first production incident or urgent request derails everything. Budget 15-20% for unplanned work.
3. **Sequencing by loudest voice.** Sequence by value, dependencies, and risk — not by who asked most recently. The roadmap should be defensible against "why isn't my thing first?"
4. **Too much detail too far out.** High confidence for this month. Moderate confidence for next quarter. Themes only for 6+ months. Detailed roadmaps for H2 are fiction.
5. **No explicit "not doing" list.** A roadmap without a "not doing" section isn't making hard choices. What you cut is as important as what you keep — make it visible.

## Related Skills

- [OKR & Goal Setting](../okr-goal-setting/SKILL.md) — set goals before mapping them to a roadmap
- [Product Strategy & Vision](../product-strategy-vision/SKILL.md) — roadmap should flow from strategy
- [Sprint & Release Planning](../sprint-release-planning/SKILL.md) — translate roadmap items into sprint-level work
- [Stakeholder Alignment](../stakeholder-alignment/SKILL.md) — when roadmap trade-offs need stakeholder buy-in
