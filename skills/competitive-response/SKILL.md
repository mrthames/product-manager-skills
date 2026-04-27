---
name: competitive-response
description: Assess and respond to a competitor move within 24-48 hours. Use when a competitor launches, changes pricing, or makes a strategic shift.
---

# Competitive Response

A competitor just did something. You have 24-48 hours before sales starts losing deals, leadership starts asking questions, and your team starts wondering if the roadmap needs to change. Claude compresses the analysis; you make the strategic call.

## When to Use

- A competitor launched a major feature or product
- A competitor changed pricing or packaging
- A competitor was acquired, raised funding, or pivoted
- Sales is getting objections referencing a competitor move
- Leadership is asking "what are we doing about [competitor]?"

## When NOT to Use

- Routine competitive monitoring — set up a Competitive Intelligence Agent (see AGENTIC-WORKFLOWS.md)
- You're doing a deep competitive analysis as part of discovery — use Discovery Process
- You're setting strategy, not responding to a move — use Product Strategy & Vision

## The AI-Native Approach

**Traditional response:** Days to weeks of analysis, slide decks, meetings, and eventually a position paper no one reads.

**AI-native response:** 2-4 hours to assess, decide, and arm the team.

| Step | Time | Claude Does | You Do |
|---|---|---|---|
| Assess the move | 30 min | Gather public info, analyze what changed | Validate accuracy, add inside knowledge |
| Evaluate impact | 30 min | Map impact to your users, deals, and roadmap | Apply strategic judgment |
| Decide response | 30 min | Generate response options with trade-offs | Make the call: respond, monitor, or ignore |
| Arm the team | 1 hr | Draft talking points, objection handlers, FAQs | Review and distribute |

## Process

### Step 1: Assess the Move (30 minutes)

```
[Competitor] just [describe what happened — launch, pricing change, acquisition, etc.].

Assess:
- What exactly changed? (features, pricing, positioning, availability)
- Who does this target? (which user segment or market)
- What's the likely strategic intent? (growth play, retention, competitive blocking, new market)
- How does this compare to what we offer?
- What are they NOT doing that our users still need us for?

Sources to check: [their website, changelog, press release, app store, social media]
```

### Step 2: Evaluate Impact on Us (30 minutes)

```
Given this competitive move, evaluate the impact:

On our users:
- Which of our user segments overlap with their target?
- Are any of our users likely to evaluate or switch?
- Does this change what our users expect from us?

On our pipeline/sales:
- Will this come up in competitive deals?
- Does it change our win/loss dynamics?
- Do we need updated competitive positioning?

On our roadmap:
- Does this validate or invalidate anything we're building?
- Does this change the urgency of any planned initiative?
- Is there something we should accelerate, and what would we defer?

Rate overall impact: high (threatens core business), medium (affects some
segments or deals), low (noise, no action needed).
```

### Step 3: Decide the Response (30 minutes)

```
Generate response options:

Option A — Respond directly:
- What we'd build or change and timeline
- What we'd defer to make room
- Risk: are we chasing their strategy instead of executing ours?

Option B — Monitor and prepare:
- Watch for user/market reaction before committing resources
- Prepare talking points for sales and CS now
- Set a review point in [2-4 weeks] to reassess
- Risk: we might lose deals in the interim

Option C — Ignore:
- This doesn't affect our core users or strategy
- Our differentiation is intact
- Risk: we're wrong about the impact

For each option: what it costs, what it gets us, and when we'd know if it worked.
```

Make the call. Most competitor moves deserve Option B. Resist the urge to react to every launch.

### Step 4: Arm the Team (1 hour)

Regardless of strategic response, your customer-facing teams need talking points now.

```
Draft competitive response materials:

For Sales — Objection handling:
- "But [competitor] just launched [feature]" → [response with our differentiation]
- Positioning: why we're still the better choice for [our target segment]
- What to say about our roadmap without over-promising

For Customer Success — Proactive talking points:
- For at-risk customers who might be evaluating: [what to say]
- For customers who ask about it: [factual comparison without FUD]

For Leadership — Assessment brief:
- What happened (2 sentences)
- Impact assessment (high/medium/low with reasoning)
- Recommended response
- What we're doing right now
```

## Output

- Competitive move assessment (what changed, who it targets, strategic intent)
- Impact evaluation (users, pipeline, roadmap)
- Response recommendation with options and trade-offs
- Sales objection handlers and CS talking points
- Leadership brief

## Common Pitfalls

1. **Reacting to every move.** Not every competitor launch warrants a response. If your strategy is sound, most moves are noise. Respond to threats to your core, not distractions.
2. **Copying instead of differentiating.** "They have it so we need it" is the weakest product rationale. Ask: does our user need this? Not: does our competitor have this?
3. **Slow response on talking points.** Even if the strategic response takes weeks, sales and CS need talking points within 24 hours. Arm the team immediately.
4. **FUD in competitive materials.** Never trash the competitor. State facts, highlight your strengths, and let the customer decide. FUD backfires.
5. **Forgetting to follow up.** Set a review date. Was the impact what you predicted? Did the response work? Update your assessment.

## Related Skills

- [Product Strategy & Vision](../product-strategy-vision/SKILL.md) — when a competitive shift requires strategic repositioning
- [Stakeholder Alignment](../stakeholder-alignment/SKILL.md) — when the response requires executive decision-making
- [Go-to-Market Planning](../go-to-market-planning/SKILL.md) — when the response involves a counter-launch
- Reference: [AGENTIC-WORKFLOWS.md](../../AGENTIC-WORKFLOWS.md) — Competitive Intelligence Agent for ongoing monitoring
