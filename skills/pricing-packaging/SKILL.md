---
name: pricing-packaging
description: Design or evaluate pricing and packaging strategy. Use when setting prices for a new tier, adjusting existing pricing, or restructuring packages.
---

# Pricing & Packaging

Structure a pricing and packaging analysis in 1-2 days instead of a multi-week pricing project. Claude handles competitive research, tier modeling, and revenue scenario analysis. You handle the strategic positioning, customer conversations, and willingness-to-pay judgment.

## When to Use

- Launching a new product or tier and need to set initial pricing
- Evaluating whether current pricing is leaving money on the table
- Restructuring packages (bundling, unbundling, good-better-best tiering)
- Competitors changed pricing and you need to respond (or not)
- Moving from freemium to paid, or introducing a free tier

## When NOT to Use

- Running a pricing A/B test — use an Experiment Brief template
- Analyzing revenue metrics — use Growth & Retention Diagnostics
- Building an investment case for a pricing change — use Stakeholder Alignment + this skill's output

## The AI-Native Approach

| Step | Time | Claude Does | You Do |
|---|---|---|---|
| Define value metrics | 1-2 hrs | Analyze product usage to identify what users value most | Validate against your customer knowledge |
| Competitive landscape | 2-3 hrs | Survey competitor pricing, features, and positioning | Add context on competitors' strategies |
| Design tiers | 2-3 hrs | Model good-better-best tier structures with feature allocation | Decide strategic positioning per tier |
| Revenue modeling | 1-2 hrs | Run scenario analysis across price points | Validate assumptions, choose target |
| Design the test | 1 hr | Draft experiment brief for pricing change | Define risk tolerance and rollout plan |

## Process

### Step 1: Define Value Metrics (1-2 hours)

A value metric is the unit your customers pay for — the thing that scales with the value they receive.

```
Here's our product context:
- [What the product does]
- [Current pricing model if it exists]
- [Key usage data — what features are used most, by whom, and how much]
- [Customer segments and their primary use cases]

Help me identify the right value metric(s):
- What do users do more of as they get more value?
- Which usage patterns correlate with retention and expansion?
- What metric is easy for customers to understand and predict?
- What metric aligns our revenue growth with customer success?

Evaluate: seats, usage volume, features, outcomes, or hybrid models.
For each option, flag the pros, cons, and which customer segments it favors.
```

### Step 2: Competitive Pricing Landscape (2-3 hours)

```
Analyze the pricing landscape for [our category/competitors]:

For each competitor [list 3-5]:
- Pricing model (per seat, usage-based, flat rate, hybrid)
- Published price points and tier structure
- What's included at each tier
- Free tier or trial availability
- Enterprise/custom pricing signals

Then assess:
- Where is the market converging on pricing model?
- Are there underserved segments (priced out or overpaying)?
- What pricing moves would be expected vs. surprising?
- Where is there room to differentiate on packaging, not just price?
```

### Step 3: Design Tier Structure (2-3 hours)

```
Based on our value metric analysis and competitive landscape, design a
good-better-best tier structure:

For each tier:
- Name and positioning (who is this for?)
- Features included (map to value realization stages)
- Price point range with rationale
- What makes someone upgrade to the next tier?
- What's explicitly excluded and why?

Constraints:
- [Your constraints — e.g., "free tier must exist", "enterprise requires SSO",
  "can't exceed $X for SMB segment"]

Design principles:
- Each tier must deliver complete value for its segment (not crippled versions)
- The upgrade trigger should be natural (usage growth, team growth, feature need)
- Packaging should be easy to explain in one sentence per tier
```

### Step 4: Revenue Modeling (1-2 hours)

```
Model revenue scenarios for the proposed tier structure:

Inputs:
- Current customer distribution: [segments, sizes, current spend]
- Assumed conversion rates between tiers: [estimates]
- Growth assumptions: [new customer acquisition rate, expansion rate]

Model three scenarios:
1. Conservative: [lower conversion, higher churn from price change]
2. Expected: [your best estimates]
3. Optimistic: [higher conversion, lower churn]

For each: project MRR impact at 3, 6, and 12 months.
Flag: which customer segments gain value, which might churn, and the net effect.
```

### Step 5: Design the Pricing Test (1 hour)

```
Draft an experiment brief for rolling out this pricing change:

- Who sees new pricing first (new customers only? specific segment? geography?)
- What's the control vs. variant?
- Success metrics: conversion rate, ARPU, revenue per visitor, churn rate
- Guardrail metrics: support ticket volume, cancellation rate, NPS
- Duration: minimum runtime for statistical significance
- Rollback criteria: what triggers reverting to current pricing
- Communication plan: how do we announce this to existing customers?
```

## Output

- Value metric analysis with recommendation
- Competitive pricing matrix
- Tier structure with feature allocation, price points, and upgrade triggers
- Revenue scenario models (conservative, expected, optimistic)
- Pricing experiment brief with rollout plan

## Common Pitfalls

1. **Cost-plus pricing.** Never set prices based on what it costs you to deliver. Price based on the value customers receive. Cost determines margin, not price.
2. **Competitor-matching.** Matching competitor prices positions you as equivalent. Price to reflect your unique value — higher if you're differentiated, lower only if you're competing on volume.
3. **Too many tiers.** Three tiers (good-better-best) is the sweet spot for most products. More than four creates decision paralysis.
4. **Crippling the free or low tier.** If your free tier is frustrating, it generates negative word-of-mouth. If it's too generous, no one upgrades. The free tier should deliver real value for a specific use case with natural upgrade triggers.
5. **Changing pricing without a communication plan.** Existing customers who discover price changes without context will churn. Always grandfather or communicate.

## Related Skills

- [Growth & Retention Diagnostics](../growth-retention-diagnostics/SKILL.md) — when pricing changes affect retention
- [Stakeholder Alignment](../stakeholder-alignment/SKILL.md) — when pricing decisions need executive buy-in
- Reference: [FRAMEWORKS.md](../../FRAMEWORKS.md) — SaaS Metrics (MRR, ARPU, LTV, CAC)
- Reference: [TEMPLATES.md](../../TEMPLATES.md) — Experiment Brief template
