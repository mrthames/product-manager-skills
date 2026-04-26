---
name: discovery-process
description: Run a compressed 5-day product discovery cycle. Use when validating whether a problem is worth solving before committing engineering resources.
---

# Discovery Process

A structured discovery cycle compressed from the traditional 3-4 weeks to 5 focused days. AI handles synthesis and framework execution; you handle user conversations and judgment calls.

## When to Use

- You've identified a potential problem or opportunity but haven't validated it
- Leadership is asking "should we build this?" and you need evidence
- You're entering a new market or user segment and need to understand needs
- Churn data, support tickets, or feedback suggest a problem but you don't know the root cause
- You need to choose between multiple possible initiatives

## When NOT to Use

- The problem is already validated and you need to write a spec — go to your PRD template
- You're optimizing an existing feature with clear metrics — use Growth & Retention Diagnostics
- You need stakeholder buy-in for something already validated — use Stakeholder Alignment

## The AI-Native Approach

**Traditional discovery:** 3-4 week dedicated sprint. Most time spent on synthesis, documentation, and alignment meetings.

**AI-native discovery:** 5 focused days. Claude compresses synthesis and documentation to hours. Your time goes to the irreplaceable human work — talking to users, applying judgment, and making the call.

| Day | Focus | Time | Claude Does | You Do |
|---|---|---|---|---|
| 1 | Frame the problem | 2-3 hrs | Structure raw signals, identify assumptions | Provide context, validate framing |
| 2 | Synthesize existing data | 2-3 hrs | Synthesize analytics, feedback, competitive data | Review against your knowledge |
| 3 | Talk to users | Half day | Prepare discussion guide, synthesize notes after | Conduct 3-5 interviews |
| 4 | Map opportunities | 2-3 hrs | Build opportunity solution tree, rank by evidence | Decide which branch to pursue |
| 5 | Decide | 1-2 hrs | Draft spec or experiment brief | Make the build/validate/kill call |

## Process

### Day 1: Frame the Problem (2-3 hours)

Bring your raw signals — support tickets, usage data, user quotes, business context.

```
Here's what I'm seeing: [raw signals — paste data, quotes, metrics].

Help me frame this as a problem statement:
- Who is affected and how many?
- What's the evidence (data vs. inference vs. assumption)?
- What are we assuming that we haven't validated?
- What's the business impact if we don't address this?
```

Review Claude's output. Challenge the framing: does this match what you're hearing from users, or is Claude over-fitting to the loudest signals?

### Day 2: Synthesize What You Know (2-3 hours)

Feed Claude your existing data sources. Don't generate new research — synthesize what already exists.

```
Here are our data sources on this problem:
- [Analytics data / dashboard exports]
- [Support ticket themes from the last 90 days]
- [Survey responses or NPS verbatims]
- [Competitive context]

Synthesize the key findings:
- What patterns emerge across sources?
- Where do sources agree or conflict?
- Rate evidence strength: strong (data-backed), moderate (inferred), weak (assumed)
- What are the critical gaps we need to fill with primary research?
```

### Day 3: Talk to Users (half day)

This step cannot be compressed or delegated. Talk to 3-5 users.

```
Based on our problem statement and the gaps identified yesterday, generate a
discussion guide for 30-minute user interviews.

Requirements:
- Focus questions on [specific gaps identified]
- Use past-behavior questions, not hypotheticals
- Include one "surprise me" open-ended question
- Flag any questions that might lead the witness
- Keep it to 8-10 questions max
```

After interviews, feed your notes back:

```
Here are my notes from [N] user interviews. Identify:
- Themes that appeared across multiple interviews
- Contradictions between users
- Surprises — anything that challenges our assumptions
- Quotes worth preserving for stakeholder communication
```

### Day 4: Map Opportunities and Rank (2-3 hours)

```
Based on our research synthesis and interview findings, build an opportunity
solution tree:

Desired outcome: [measurable outcome — e.g., "reduce onboarding drop-off from 40% to 25%"]

For each opportunity:
- 2-3 possible solutions
- Evidence strength supporting this opportunity
- Simplest experiment that would validate each solution
- Estimated effort and impact

Rank opportunities by evidence strength × potential impact.
```

Review the tree. Override the ranking when your strategic context says otherwise.

### Day 5: Decide (1-2 hours)

Three possible outcomes:

**Build:** Evidence is strong. Ask Claude to draft the PRD from your discovery artifacts.

**Validate further:** Evidence is promising but thin. Ask Claude to draft an experiment brief.

**Kill:** Evidence doesn't support the hypothesis. Document why and move on.

```
Based on our 5-day discovery, draft a [PRD / experiment brief / decision memo]
that captures:
- The problem and evidence
- What we learned from users
- The recommended path forward
- What we're explicitly choosing NOT to do and why
```

## Output

- Structured problem statement with evidence ratings
- Research synthesis with gap analysis
- User interview themes and key quotes
- Opportunity solution tree with ranked options
- PRD, experiment brief, or kill decision memo

## Common Pitfalls

1. **Skipping user interviews to save time.** Days 1-2 and 4-5 can be compressed further. Day 3 cannot. Talking to users is the entire point.
2. **Treating Claude's synthesis as ground truth.** Claude identifies patterns in the data you provide. It can't tell you about the user who churned silently or the competitor move that hasn't been announced.
3. **Falling in love with the first opportunity.** The tree exists to keep options open. Don't collapse to a solution before you've evaluated alternatives.
4. **Discovery as delay tactic.** 5 days is the limit. If you need more time, you're probably avoiding a decision, not gathering evidence.

## Related Skills

- [Product Strategy & Vision](../product-strategy-vision/SKILL.md) — when discovery feeds into strategic planning
- [User Research Methods](../user-research-methods/SKILL.md) — for deeper research beyond the 5-day cycle
- [Stakeholder Alignment](../stakeholder-alignment/SKILL.md) — when discovery findings need stakeholder buy-in
- Reference: [FRAMEWORKS.md](../../FRAMEWORKS.md) — JTBD, Opportunity Solution Trees, Customer Journey Mapping
- Reference: [TEMPLATES.md](../../TEMPLATES.md) — PRD and Experiment Brief templates
