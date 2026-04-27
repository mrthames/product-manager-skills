---
name: sprint-release-planning
description: Plan sprints and releases — break epics into stories, model capacity, flag risks. Use for weekly sprint planning or release scoping.
---

# Sprint & Release Planning

Turn sprint and release planning from a half-day meeting prep exercise into an hour of focused work. Claude breaks down epics, models capacity, sequences work, and flags dependency risks. You validate with engineering and make the scope calls.

## When to Use

- Sprint planning is coming up and you need to break work into shippable stories
- You're scoping a release and need to map what fits in the timeline
- Scope changed mid-sprint and you need to re-plan quickly
- You're negotiating capacity allocation across initiatives
- A new dependency surfaced and you need to assess the impact on the plan

## When NOT to Use

- You need to prioritize what to build — use Prioritization frameworks in FRAMEWORKS.md
- You need to set quarterly goals — use OKR & Goal Setting
- You need to communicate the plan to stakeholders — use the Stakeholder Update templates

## The AI-Native Approach

| Step | Time | Claude Does | You Do |
|---|---|---|---|
| Break down work | 20 min | Split epics into stories with acceptance criteria | Validate scope and completeness with eng |
| Model capacity | 15 min | Calculate available capacity, map stories to capacity | Confirm team availability and velocity |
| Sequence and dependencies | 15 min | Identify dependencies, flag risks, suggest sequence | Validate with dependent teams |
| Handle scope trade-offs | 10 min | Model what fits vs. what gets deferred | Make the scope call |

## Process

### Step 1: Break Down Work (20 minutes)

```
Here are the epics/features planned for [sprint/release]:
[List with brief descriptions]

For each, break into shippable user stories:
- Standard format (As a... I want to... so that...)
- Testable acceptance criteria for each
- Relative size estimate (S/M/L)
- Flag any story that's larger than "M" — it needs further splitting

Apply story splitting patterns: workflow steps, business rules, data
variations, happy path vs. edge cases.
```

### Step 2: Model Capacity (15 minutes)

```
Sprint/release parameters:
- Duration: [2 weeks / 4 weeks / specific dates]
- Team: [N engineers, N designers]
- Known absences or commitments: [PTO, on-call rotations, meetings]
- Historical velocity: [points or stories per sprint]

Map the stories from Step 1 against available capacity:
- Total capacity in story points or estimated days
- Stories that fit within capacity
- Stories that overflow — ranked by priority for deferral
- Buffer: leave [10-20%] for unplanned work and bugs
```

### Step 3: Sequence and Flag Dependencies (15 minutes)

```
For the stories that fit in this sprint/release:
- Identify dependencies between stories (which must complete before others start)
- Identify external dependencies (other teams, APIs, design assets, data)
- Flag any dependency that could block progress
- Suggest a sequencing that minimizes blocking risk
- Identify what can be parallelized

For each risk:
- What's the risk
- Probability (high/medium/low)
- Impact if it materializes
- Mitigation: what we can do now to reduce the risk
```

### Step 4: Handle Scope Trade-offs (10 minutes)

When more work exists than capacity allows:

```
We have [X points] of work and [Y points] of capacity. Help me make the
scope trade-off:

For each story that might be deferred:
- What user value is delayed
- Is anything else blocked if this is deferred
- Can it be descoped (smaller version that still delivers value)
- Impact on the release goal if removed

Recommend a cut line with rationale.
```

Review the recommendation. Override based on stakeholder commitments, strategic context, and what you know about team momentum.

## Output

- Sprint/release backlog with sized, sequenced stories
- Capacity model with buffer allocation
- Dependency map with risk flags
- Scope trade-off analysis with recommended cut line
- Sprint goal statement (one sentence: what's the most important thing this sprint delivers)

## Common Pitfalls

1. **No buffer for unplanned work.** Every sprint has surprises. Plan to 80-90% capacity, not 100%.
2. **Stories too large.** If a story takes more than 3 days, it should be split. Large stories hide risk and reduce the team's ability to course-correct.
3. **Ignoring dependencies until they block.** Surface dependencies at planning time, not when someone is stuck.
4. **Planning without engineering input.** Claude estimates are starting points. Engineers validate sizing, flag technical risks, and confirm sequencing.
5. **Treating the plan as fixed.** The plan is a starting point. When reality changes mid-sprint, re-plan — don't pretend the original plan still holds.

## Related Skills

- [OKR & Goal Setting](../okr-goal-setting/SKILL.md) — setting the goals that sprints execute against
- [Stakeholder Alignment](../stakeholder-alignment/SKILL.md) — when scope trade-offs need stakeholder buy-in
- Reference: [FRAMEWORKS.md](../../FRAMEWORKS.md) — Story Splitting patterns
- Reference: [TEMPLATES.md](../../TEMPLATES.md) — Epic, Feature, and User Story templates
