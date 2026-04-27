---
name: metrics-review
description: Run a regular metrics review — pull data, spot patterns, translate numbers into narrative. Use for weekly or biweekly product health checks.
---

# Metrics Review & Data Storytelling

Turn your weekly metrics review from a 3-hour dashboard-clicking session into a 30-minute focused analysis. Claude pulls the patterns, flags anomalies, and drafts the narrative. You interpret the results, decide what matters, and communicate it.

## When to Use

- Weekly or biweekly product health check
- Preparing a metrics update for team standup or leadership review
- You noticed something in a dashboard and need to investigate quickly
- Pulling together a data story for a specific audience
- Quarterly business review prep

## When NOT to Use

- Churn is increasing and you need root cause analysis — use Growth & Retention Diagnostics
- You're setting up metrics for the first time — use KPI definition in CLAUDE.md
- You're analyzing a specific experiment — use the Experiment Brief template

## The AI-Native Approach

| Step | Time | Claude Does | You Do |
|---|---|---|---|
| Pull and structure data | 10 min | Organize metrics, calculate trends, flag anomalies | Feed the data, confirm accuracy |
| Identify patterns | 10 min | Surface what's moving, what's flat, what's surprising | Apply context Claude doesn't have |
| Build the narrative | 10 min | Draft the data story for your audience | Add judgment, implications, and next steps |

## Process

### Step 1: Pull and Structure (10 minutes)

```
Here's this [week's/month's] metrics data:
[Paste from your analytics tool, spreadsheet, or dashboard export]

Structure a metrics review:
- For each key metric: current value, previous period, trend (improving/flat/declining), vs. target
- Flag anything that moved more than [10%/your threshold] in either direction
- Flag anything that's been flat for 3+ periods when you'd expect movement
- Calculate rates of change — is the trend accelerating or decelerating?
```

### Step 2: Identify Patterns (10 minutes)

```
Based on the structured metrics:
- What's the headline? (The single most important thing in this data)
- What's improving and why might that be?
- What's declining and what hypotheses explain it?
- What's surprisingly flat — should we be concerned?
- Are there correlations between metrics? (e.g., activation up but retention flat)
- What happened this period that might explain changes? (releases, marketing, seasonal, external)
```

Add your context: What shipped this period? What's happening in the market? What do you know from user conversations that explains a number?

### Step 3: Build the Narrative (10 minutes)

Different audiences need different data stories.

**For your team:**
```
Draft a team metrics update:
- Headline metric and trend
- What's working (keep doing)
- What needs attention (investigate or act)
- Specific actions for this sprint based on the data
Keep it to 5-7 bullet points max.
```

**For leadership:**
```
Draft an executive metrics summary:
- Lead with the business metric they care about (revenue, growth, retention)
- Show trajectory vs. target — are we on pace?
- One risk to flag with a mitigation plan
- One bright spot worth highlighting
Keep it to one paragraph or 3-5 bullets.
```

**For a quarterly review:**
```
Structure a quarterly business review section:
- Quarter-over-quarter trends for key metrics
- Progress against OKRs (actual vs. target)
- Cohort comparison: are newer cohorts healthier?
- Top 3 wins and top 3 concerns with evidence
- Outlook: what the data predicts for next quarter
```

## Output

- Structured metrics dashboard with trends and anomaly flags
- Pattern analysis with hypotheses
- Audience-appropriate data narrative (team, leadership, or quarterly review)

## Common Pitfalls

1. **Reporting numbers without interpretation.** "MRR grew 3%" is data. "MRR grew 3%, driven by expansion in the enterprise segment, which validates our upsell investment" is a story.
2. **Cherry-picking good metrics.** Include the bad numbers. Credibility comes from honesty. If churn is up, say so and say what you're doing about it.
3. **Too many metrics.** A weekly review should cover 5-8 key metrics, not 30. If everything is a priority, nothing is.
4. **No action items.** A metrics review that doesn't lead to "so what do we do?" is a waste of time. Every review should end with at least one action.
5. **Trusting AI-generated insights without validation.** Claude spots patterns in the data you provide. It doesn't know about the pricing change you announced, the competitor that launched, or the bug that affected 5% of users. Add your context.

## Related Skills

- [Growth & Retention Diagnostics](../growth-retention-diagnostics/SKILL.md) — when a metric needs deep investigation
- [OKR & Goal Setting](../okr-goal-setting/SKILL.md) — metrics review feeds OKR progress tracking
- Reference: [FRAMEWORKS.md](../../FRAMEWORKS.md) — SaaS Metrics definitions and benchmarks
- Reference: [AGENTIC-WORKFLOWS.md](../../AGENTIC-WORKFLOWS.md) — User Analytics Agent for automated monitoring
