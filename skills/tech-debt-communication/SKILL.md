---
name: tech-debt-communication
description: Quantify and communicate tech debt as a business decision. Use when engineering needs investment in infrastructure and you need to make the case to leadership.
---

# Tech Debt Communication

Translate technical debt into business language in 2-4 hours. Claude helps quantify impact, structure the investment case, and generate scenario models. You provide the engineering partnership, stakeholder context, and the judgment to frame it as a business decision, not a technical one.

## When to Use

- Engineering is flagging tech debt that's slowing velocity or increasing risk
- You need to justify infrastructure investment to non-technical stakeholders
- Technical debt is creating user-facing quality issues
- You're negotiating capacity allocation between features and platform work
- A major incident was caused by deferred maintenance and you need to prevent the next one

## When NOT to Use

- Engineering can handle it within their normal capacity — not everything needs a PM business case
- The debt is purely internal with no velocity, risk, or user impact — defer to engineering's judgment
- You need to align stakeholders on a non-technical decision — use Stakeholder Alignment

## The AI-Native Approach

| Step | Time | Claude Does | You Do |
|---|---|---|---|
| Understand the debt | 30 min | Structure the information from engineering | Partner with engineering to understand scope |
| Quantify business impact | 1 hr | Model velocity cost, incident risk, opportunity cost | Validate with engineering, add user context |
| Frame the decision | 1 hr | Draft the investment case as a business trade-off | Add stakeholder context, political awareness |
| Build scenarios | 30 min | Model invest-now vs. defer scenarios | Choose the framing that fits your audience |
| Present | 30 min | Format for target audience | Deliver with conviction and handle questions |

## Process

### Step 1: Understand the Debt (30 minutes)

Partner with your engineering lead. This step is a conversation, not a document.

```
I need to understand and communicate tech debt to non-technical stakeholders.
Help me structure what I've learned from engineering:

The debt: [what engineering described — outdated systems, scaling limits,
testing gaps, dependency risks, architecture constraints]

Help me categorize:
1. What type of debt is this?
   - Deliberate (we chose speed over quality knowingly)
   - Accidental (we didn't know better at the time)
   - Environmental (the world changed — new scale, new requirements)
2. What's the blast radius?
   - Which systems, features, or teams are affected?
3. What's the trajectory?
   - Is this stable (bad but not getting worse)?
   - Compounding (getting worse over time)?
   - Time-bombed (will fail at a known threshold)?
```

### Step 2: Quantify Business Impact (1 hour)

Non-technical stakeholders don't care about code quality. They care about velocity, risk, and cost.

```
Help me quantify the business impact of this tech debt:

Velocity impact:
- How much slower is development in the affected area? [engineering's estimate]
- What features are delayed or blocked by this debt?
- What's the cost of that delay? (Use Cost of Delay: revenue, competitive position, user impact per week of delay)

Risk impact:
- What's the probability of an incident caused by this debt? [engineering's assessment]
- What's the cost of that incident? (Downtime × revenue impact, customer trust, support load)
- Have we already had incidents? [history]

Opportunity cost:
- What could the team build if they weren't working around this debt?
- What new capabilities does addressing the debt unlock?
- What becomes possible that's currently impossible?

Model the total cost of inaction over 6 and 12 months.
```

### Step 3: Frame as a Business Decision (1 hour)

The goal is to present this as a resource allocation decision with clear trade-offs — not as "engineering wants to refactor."

```
Draft an investment case for addressing this tech debt.

Structure as a business decision, not a technical request:
1. The business problem: [velocity/risk/opportunity framed in business terms]
2. Options:
   a. Invest now: [scope, timeline, team cost, what we defer]
   b. Invest later: [what we accept in the meantime, how cost grows]
   c. Don't invest: [projected impact over 6-12 months]
3. Recommendation: [which option and why]
4. What we get: [concrete outcomes — faster delivery, reduced incidents, new capabilities]
5. What it costs: [engineering weeks, features we delay, timeline]
6. What happens if we don't: [quantified cost of inaction]

Audience: [executive team / product leadership / board — adjust tone accordingly]
```

### Step 4: Build Scenario Models (30 minutes)

```
Model two scenarios for this tech debt decision:

Scenario A — Invest Now:
- Investment: [X engineering weeks]
- Features deferred: [list with estimated delay]
- Expected outcome: [velocity improvement, risk reduction, capabilities unlocked]
- Break-even: [when the velocity gain pays back the investment]

Scenario B — Defer 6 Months:
- Continued velocity drag: [X% slower in affected area]
- Incident probability: [estimated, with cost per incident]
- Growing scope: [how much more work it becomes to address later]
- Features at risk: [what becomes harder or impossible]

Present as a table comparing both scenarios across: cost, velocity, risk, and timeline.
```

### Step 5: Present to Stakeholders (30 minutes)

```
Format the investment case for [audience]:

For executive leadership:
- Lead with the business metric at risk
- Show the cost of inaction in dollars or velocity percentage
- Present options as a trade-off, not a request
- End with a clear ask and timeline

For product leadership:
- Lead with the roadmap impact
- Show which features are affected and by how much
- Present the opportunity cost — what we could build if this was resolved
- End with a proposed allocation (e.g., "20% of next quarter's capacity")
```

## Output

- Categorized tech debt assessment (type, blast radius, trajectory)
- Quantified business impact (velocity, risk, opportunity cost)
- Investment case with options and recommendation
- Scenario comparison (invest now vs. defer)
- Stakeholder-ready presentation

## Common Pitfalls

1. **Presenting it as a technical problem.** "We need to refactor the billing service" means nothing to an executive. "We're losing $X/month in developer velocity and our incident risk is growing" is a business problem.
2. **Framing it as all-or-nothing.** Executives fear open-ended infrastructure projects. Scope it tightly: specific debt, specific investment, specific outcome, specific timeline.
3. **No engineering partnership.** You cannot quantify tech debt alone. This skill requires genuine collaboration with engineering to understand scope and estimate impact.
4. **Crying wolf.** If every sprint includes a tech debt pitch, stakeholders tune out. Prioritize the debt that has the highest business impact and make that case well.
5. **Ignoring the trade-off.** Every week spent on tech debt is a week not spent on features. Acknowledge this explicitly and show why the trade-off is worth it.

## Related Skills

- [Stakeholder Alignment](../stakeholder-alignment/SKILL.md) — when the tech debt case needs cross-functional buy-in
- [Growth & Retention Diagnostics](../growth-retention-diagnostics/SKILL.md) — when tech debt is causing user-facing quality issues
- Reference: [FRAMEWORKS.md](../../FRAMEWORKS.md) — Cost of Delay framework
- Reference: [TEMPLATES.md](../../TEMPLATES.md) — Stakeholder Update (Executive Level) template
