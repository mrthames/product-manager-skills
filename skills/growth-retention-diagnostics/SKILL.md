---
name: growth-retention-diagnostics
description: Diagnose churn, retention, or growth problems with data. Use when metrics are declining and you need to find the root cause, not just report the numbers.
---

# Growth & Retention Diagnostics

Move from "churn is up" to "here's why and here's what to do about it" in half a day. Claude runs the cohort math, generates diagnostic hypotheses, and structures the intervention design. You validate against your user knowledge and decide what to pursue.

## When to Use

- Churn or revenue retention is trending the wrong direction
- Activation or onboarding metrics have dropped
- A specific cohort or segment is underperforming
- You need to build a retention case for leadership
- Growth has stalled and you need to find the lever

## When NOT to Use

- You're setting up initial metrics and instrumentation — use KPI definition in CLAUDE.md
- You're running a specific experiment — use the Experiment Brief template
- The problem is clearly a bug or outage — that's incident response, not diagnostics

## The AI-Native Approach

| Step | Time | Claude Does | You Do |
|---|---|---|---|
| Define the problem | 30 min | Structure the data picture, flag anomalies | Confirm what's real vs. noise |
| Run cohort analysis | 1-2 hrs | Run cohort math, generate retention curves, segment breakdowns | Validate data quality, add context |
| Diagnose root cause | 1-2 hrs | Generate hypotheses ranked by evidence, map to user journey | Apply user knowledge, eliminate false leads |
| Design interventions | 1 hr | Structure intervention options with expected impact | Choose what to pursue, validate with eng/design |
| Build the case | 30 min | Draft retention plan for stakeholders | Add strategic context and commitment |

## Process

### Step 1: Define the Problem with Data (30 minutes)

```
Here's what we're seeing: [paste your metrics — churn rate, NRR, retention
curves, activation rates, whatever you have].

Help me structure the problem:
- What exactly is declining, by how much, and since when?
- Is this across all users or specific segments?
- Is this a sudden change or a gradual trend?
- What changed around the time the metric shifted? (releases, pricing, competitors, seasonality)
- What's the revenue impact of this trend continuing?
```

### Step 2: Run Cohort Analysis (1-2 hours)

```
Here's our user/revenue data: [export from analytics tool].

Run cohort analysis:
- Monthly cohorts for the last 12 months
- Retention at Day 1, Day 7, Day 30, Day 60, Day 90
- Segment by: [plan type, acquisition channel, use case, geography — whatever matters]
- Identify which cohorts are underperforming vs. your baseline
- Flag the biggest drop-off point in the user journey

For revenue retention (NRR), break down:
- Expansion MRR by cohort
- Contraction MRR by cohort
- Churn MRR by cohort
- Net: are newer cohorts healthier or sicker than older ones?
```

### Step 3: Diagnose Root Cause (1-2 hours)

```
Based on the cohort analysis, generate diagnostic hypotheses.

For each hypothesis:
- What the data suggests
- Where in the user journey the problem occurs
- Which user segment is most affected
- What additional data would confirm or reject this hypothesis
- Confidence level: high (data clearly points here), medium (pattern exists),
  low (possible but thin evidence)

Map hypotheses to these common root cause categories:
1. Onboarding failure (users never reach value)
2. Value gap (product doesn't solve the job well enough)
3. Competitive loss (users found a better alternative)
4. Pricing mismatch (value delivered doesn't justify cost)
5. Engagement decay (users engaged initially, then stopped)
6. Segment mismatch (acquiring users who aren't a good fit)
```

Validate against what you know: Which hypotheses match what users are telling you? Which are surprising? What context does Claude not have?

### Step 4: Design Interventions (1 hour)

```
For the top 2-3 hypotheses, design interventions:

For each:
- What changes (product, onboarding, messaging, pricing, support)
- Expected impact on the target metric
- Effort to implement (days/weeks, who's involved)
- How to test it (experiment design, success criteria)
- Time to measurable result

Rank by: impact × confidence ÷ effort.
```

### Step 5: Build the Retention Case (30 minutes)

```
Draft a retention plan for [audience — leadership, board, team]:

Structure:
- The problem: what's happening and the revenue impact
- Root cause: what our analysis found (lead with the strongest evidence)
- Plan: 2-3 interventions with expected impact and timeline
- Investment needed: effort, resources, trade-offs
- What happens if we don't act: projected impact at current trend
- How we'll measure: success metrics and review cadence
```

## Output

- Structured problem definition with revenue impact
- Cohort analysis with segment breakdowns
- Ranked diagnostic hypotheses with evidence ratings
- Intervention designs with experiment briefs
- Retention plan for stakeholder presentation

## Common Pitfalls

1. **Treating symptoms, not causes.** "Add a re-engagement email" is a tactic, not a diagnosis. Find the root cause first.
2. **Averaging across segments.** Overall churn can look stable while one segment hemorrhages and another grows. Always segment.
3. **Confusing correlation with causation.** "Users who use Feature X retain better" might mean Feature X drives retention, or it might mean engaged users discover Feature X. Dig deeper.
4. **Analysis paralysis.** The point of this skill is a half-day diagnostic, not a 6-month research project. Get to hypotheses fast, design experiments, and test.
5. **Ignoring qualitative data.** Cohort math tells you where the problem is. Exit surveys, support tickets, and cancellation reasons tell you why. You need both.

## Related Skills

- [Discovery Process](../discovery-process/SKILL.md) — when the diagnostic reveals a problem worth a deeper investigation
- [Pricing & Packaging](../pricing-packaging/SKILL.md) — when pricing mismatch is the root cause
- [User Research Methods](../user-research-methods/SKILL.md) — when you need qualitative data to complement the quantitative diagnosis
- Reference: [FRAMEWORKS.md](../../FRAMEWORKS.md) — SaaS Metrics, NRR benchmarks
