---
name: okr-goal-setting
description: Set OKRs or quarterly goals — define objectives, decompose key results, align with strategy. Use at the start of a planning cycle.
---

# OKR & Goal Setting

Structure your quarterly or annual OKRs in a focused 2-3 hour session. Claude handles the framework mechanics — decomposition, measurement criteria, alignment checks. You provide the strategic judgment about what matters most.

## When to Use

- Start of a quarter or fiscal year when goals need to be set
- Mid-cycle when OKRs need revision based on new information
- When leadership asks for your team's goals and you need to connect them to company objectives
- When you're inheriting a team and need to set direction quickly

## When NOT to Use

- You need to decide what to build — use Prioritization frameworks in FRAMEWORKS.md
- You need to track progress against existing OKRs — use Metrics Review
- You need to communicate goals to stakeholders — use Stakeholder Alignment

## The AI-Native Approach

| Step | Time | Claude Does | You Do |
|---|---|---|---|
| Audit context | 30 min | Structure company goals, last quarter's results, strategic priorities | Provide context, flag what changed |
| Draft objectives | 30 min | Generate objective candidates tied to strategy | Choose the 2-4 that matter most |
| Decompose key results | 45 min | Propose measurable KRs with baselines and targets | Validate that KRs are achievable and measurable |
| Stress-test | 30 min | Check alignment, flag conflicts, identify gaps | Confirm with leadership and team |

## Process

### Step 1: Audit Context (30 minutes)

```
Here's our context for [quarter/year] goal setting:

Company-level goals: [what leadership has set as priorities]
Last quarter's results: [what we achieved vs. planned, what we learned]
Product strategy: [current vision and strategic bets]
Team capacity: [team size, any changes, known constraints]
What changed: [new data, market shifts, strategy pivots since last cycle]

Summarize:
- What should carry forward from last quarter (unfinished but still important)
- What should be dropped (no longer relevant or strategic)
- What's new this quarter (emerging priorities)
```

### Step 2: Draft Objectives (30 minutes)

```
Based on our context, draft 4-6 objective candidates.

Good objectives are:
- Qualitative and inspirational (what we want to achieve, not a metric)
- Aligned to company goals (clear line of sight to what leadership cares about)
- Achievable within the time horizon (ambitious but not delusional)
- Within our team's influence (we can move this, not just observe it)

For each objective:
- The objective statement (one sentence)
- Which company goal it supports
- Why this quarter (what makes it timely)
- What we'd sacrifice to pursue this (every yes is a no to something else)
```

Select 2-4 objectives. More than 4 means nothing is a priority.

### Step 3: Decompose Key Results (45 minutes)

```
For each selected objective, draft 2-4 key results.

Good key results are:
- Quantitative and measurable (a number with a target)
- Outcome-based, not output-based ("increase activation to 60%" not "ship onboarding redesign")
- Time-bound (measurable by end of quarter)
- Stretch but achievable (60-70% confidence of hitting)

For each key result:
- The metric and target
- Current baseline
- Data source (where we measure this)
- Leading indicators (early signals we're on track or off)
- Risk: what could prevent us from hitting this?
```

### Step 4: Stress-Test (30 minutes)

```
Review our OKRs for:

Alignment:
- Does each objective clearly connect to a company goal?
- Do the key results actually measure the objective? (not a proxy)
- Are there company goals we're not covering? Should we be?

Conflicts:
- Do any key results conflict with each other? (optimizing one hurts another)
- Do any require resources we don't control?
- Are any dependent on other teams' OKRs being met?

Gaps:
- Is anything important missing?
- Are we measuring what's easy instead of what matters?
- Do we have leading indicators for each KR so we don't find out we missed at quarter-end?

Achievability:
- At our current trajectory, which KRs are we likely to hit/miss?
- What needs to change for us to hit the stretch targets?
```

## Output

- Context audit with carry-forward, drop, and new priorities
- 2-4 objectives with strategic alignment
- 2-4 key results per objective with baselines, targets, and data sources
- Alignment and conflict analysis
- Leading indicators for early tracking

## Common Pitfalls

1. **Too many objectives.** 2-4 per team. Period. If you can't say no, your OKRs are a to-do list, not a strategy.
2. **Output key results.** "Ship feature X" is not a key result — it's a task. "Increase metric Y from A to B" is a key result. The feature is one possible way to get there.
3. **Sandbagging targets.** OKRs should be stretch goals (60-70% confidence). If you hit 100% of your KRs, they weren't ambitious enough.
4. **Set and forget.** Review OKR progress weekly in metrics review. Adjust tactics, not goals — unless fundamentally wrong assumptions surface.
5. **No connection to daily work.** If the team can't explain how their sprint work connects to a KR, the OKRs are decorative.

## Related Skills

- [Product Strategy & Vision](../product-strategy-vision/SKILL.md) — OKRs should flow from strategy
- [Metrics Review](../metrics-review/SKILL.md) — tracking OKR progress week over week
- [Sprint & Release Planning](../sprint-release-planning/SKILL.md) — translating OKRs into sprint work
- Reference: [FRAMEWORKS.md](../../FRAMEWORKS.md) — SaaS Metrics for choosing the right KR metrics
