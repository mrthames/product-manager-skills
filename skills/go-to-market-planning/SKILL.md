---
name: go-to-market-planning
description: Build a go-to-market plan for a launch — messaging, channels, enablement, timeline. Use when you're shipping something that needs coordinated market entry.
---

# Go-to-Market Planning

Build a complete go-to-market plan in 1-2 days. Claude drafts messaging frameworks, enablement materials, and launch timelines. You provide the strategic channel decisions, audience judgment, and cross-functional coordination.

## When to Use

- Launching a new product, major feature, or tier
- Entering a new market segment or geography
- Repositioning an existing product
- A launch is 4-8 weeks out and you need to coordinate cross-functionally
- Marketing, sales, or CS is asking "how do we talk about this?"

## When NOT to Use

- You need product readiness (FAQs, help docs, training) — those templates exist in TEMPLATES.md and overlap with this skill but are distinct
- You're writing release notes for an incremental update — use the Release Communication template
- The product isn't ready to launch — use Discovery Process or finish building first

## The AI-Native Approach

| Step | Time | Claude Does | You Do |
|---|---|---|---|
| Define audience & positioning | 1-2 hrs | Draft positioning variants, audience profiles | Choose positioning, validate against customer knowledge |
| Build messaging framework | 2-3 hrs | Generate messaging hierarchy with proof points | Stress-test with sales/CS for accuracy |
| Select channels | 1 hr | Analyze channel options with pros/cons | Decide channel mix based on budget and capacity |
| Create enablement | 2-3 hrs | Draft sales one-pagers, CS talking points, demo scripts | Review with the teams who'll use them |
| Build launch timeline | 1 hr | Structure timeline with dependencies and owners | Confirm commitments with cross-functional leads |

## Process

### Step 1: Define Audience & Positioning (1-2 hours)

```
We're launching [product/feature/tier]:
- What it does: [description]
- Who it's for: [target users/buyers]
- The problem it solves: [evidence-backed problem statement]
- Current alternatives: [what users do today without this]
- Competitive context: [how competitors address this]

Draft 3 positioning variants using this structure:
For [target audience] who [need], [product] is a [category] that [key benefit].
Unlike [alternative], we [primary differentiator].

For each variant:
- Who it resonates with most
- What it de-emphasizes
- What proof points support it
```

### Step 2: Build Messaging Framework (2-3 hours)

```
Based on our chosen positioning, build a messaging hierarchy:

1. Headline message (one sentence — the thing that goes on the landing page)
2. Supporting messages (3 pillars — the key reasons to believe)
3. For each pillar:
   - Claim (what we're saying)
   - Proof point (evidence — data, customer quote, demo)
   - Objection (what skeptics will say)
   - Response (how we address the objection)
4. Audience-specific angles:
   - For [buyer persona]: emphasize [what matters to them]
   - For [user persona]: emphasize [what matters to them]
   - For [technical evaluator]: emphasize [what matters to them]

Write in the customer's language, not product jargon.
```

### Step 3: Select Channels (1 hour)

```
For this launch, evaluate these channel options:

For each channel [product-led, sales-led, content/SEO, paid acquisition,
email to existing base, partner channel, community/social, events]:
- Fit for our audience (how do they discover and evaluate products?)
- Expected reach and conversion
- Cost and effort to execute
- Timeline to impact
- What we'd need to create for this channel

Recommend a channel mix based on:
- Our budget: [range]
- Our team capacity: [what teams are available]
- Our timeline: [launch date]
```

### Step 4: Create Enablement Materials (2-3 hours)

```
Generate enablement materials for launch:

For Sales:
- One-page overview (problem, solution, differentiation, pricing, competitive comparison)
- Objection handling guide (top 5 objections with responses)
- Discovery questions to identify fit

For Customer Success:
- Talking points for customer conversations
- FAQ for existing customer questions about the new offering
- Upgrade/migration guidance if applicable

For Marketing:
- Landing page copy (headline, subhead, 3 benefit sections, CTA)
- Email announcement (subject line, body, CTA)
- Social media posts (3-5 variants for different platforms)

All materials should use the messaging framework from Step 2.
```

### Step 5: Build Launch Timeline (1 hour)

```
Create a launch timeline for [launch date]:

Work backward from launch day:
- T-4 weeks: [what needs to happen]
- T-2 weeks: [what needs to happen]
- T-1 week: [final preparations]
- Launch day: [sequence of events]
- T+1 week: [post-launch activities]
- T+2 weeks: [first review point]

For each milestone:
- Owner (which team/person)
- Deliverable
- Dependencies
- Readiness gate (what must be true before proceeding)

Include cross-functional coordination points: engineering freeze date,
design asset deadlines, marketing copy approvals, sales training dates.
```

## Output

- Positioning statement (chosen from variants)
- Messaging framework with hierarchy, proof points, and audience angles
- Channel strategy with recommended mix
- Enablement package (sales, CS, marketing materials)
- Launch timeline with owners, dependencies, and readiness gates

## Common Pitfalls

1. **Building messaging without talking to customers.** Your positioning should be informed by how customers describe the problem, not how your team describes the solution.
2. **Launching without enablement.** If sales can't articulate the value or CS can't answer questions, the launch creates problems, not growth.
3. **Too many channels, too thin.** Better to go deep on 2-3 channels than shallow on 7. Choose channels where your audience actually is.
4. **Marketing-only GTM.** Go-to-market is cross-functional. Product, sales, CS, support, and marketing all need coordinated execution.
5. **No post-launch plan.** Launch day is the beginning, not the end. Plan for the first 2 weeks of monitoring, feedback collection, and iteration.

## Related Skills

- [Product Strategy & Vision](../product-strategy-vision/SKILL.md) — when GTM needs to align with broader strategy
- [Pricing & Packaging](../pricing-packaging/SKILL.md) — when the launch includes pricing decisions
- [Stakeholder Alignment](../stakeholder-alignment/SKILL.md) — when cross-functional leads need to align on the plan
- Reference: [TEMPLATES.md](../../TEMPLATES.md) — Release Communication, Product Readiness Checklist, FAQ templates
- Reference: [AI-NATIVE-WORKFLOW.md](../../AI-NATIVE-WORKFLOW.md) — Product Readiness section
