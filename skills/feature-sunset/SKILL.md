---
name: feature-sunset
description: Plan and communicate a feature or product end-of-life. Use when deprecating features, sunsetting products, or managing migration off legacy systems.
---

# Feature Sunset & EOL

Shutting things down is harder than launching them. This skill walks you through the full lifecycle: impact analysis, migration planning, communication strategy, and stakeholder management. Claude handles the artifact generation; you handle the relationship sensitivity and timing judgment.

## When to Use

- Deprecating a feature that has active users
- Sunsetting a product or product tier
- Migrating users off a legacy system
- Removing an integration or API that external partners depend on
- Consolidating overlapping features after an acquisition

## When NOT to Use

- You're deciding whether to build something — use Discovery Process
- You're evaluating tech debt (not removing features) — use Tech Debt Communication
- You're communicating a scope reduction in an upcoming release — that's release planning, not EOL

## The AI-Native Approach

| Step | Time | Claude Does | You Do |
|---|---|---|---|
| Impact analysis | 1 hr | Quantify usage, identify affected users, model revenue risk | Validate data, add relationship context |
| Migration planning | 1-2 hrs | Design migration path, generate guides and timelines | Confirm with engineering, set deadlines |
| Communication strategy | 1-2 hrs | Draft multi-audience communications at each stage | Add empathy, timing, and relationship awareness |
| Stakeholder alignment | 1 hr | Prepare decision document and FAQ | Navigate the politics and get sign-off |

## Process

### Step 1: Impact Analysis (1 hour)

```
We're considering sunsetting [feature/product]. Here's what we know:

Usage data:
- [Active users/accounts using this feature]
- [Usage frequency and trend — growing, stable, declining]
- [Revenue attributed to or dependent on this feature]

Help me assess the full impact:
- How many users are affected and in which segments?
- What's the revenue at risk (direct and indirect)?
- Are any contractual obligations tied to this feature?
- What do these users do with this feature — what job does it serve?
- What alternatives exist (in our product or elsewhere)?
- What's the cost of maintaining it vs. the cost of removing it?
```

### Step 2: Design Migration Path (1-2 hours)

```
For users affected by this sunset, design a migration plan:

For each user segment:
- Where do they go? (alternative feature, competitor, workaround)
- What do they need to do? (export data, change workflow, update integrations)
- What do we provide to help? (migration tool, guide, support, credits)
- Timeline: how much notice and what's the grace period?

Migration timeline:
1. Announcement: [date] — feature continues working, users notified
2. Deprecation warning: [date] — in-app warnings, feature flagged
3. Migration support window: [date range] — active help for transitioning users
4. Read-only / reduced functionality: [date] — can access data but not create new
5. Full removal: [date] — feature removed, data archived or exported

For each phase: what changes for the user, what we communicate, what support we offer.
```

### Step 3: Communication Strategy (1-2 hours)

EOL communication happens in waves, not a single announcement.

```
Draft communications for each phase of the sunset:

Phase 1 — Early notice (8-12 weeks before removal):
- Email to affected users: what's happening, why, what they should do, timeline
- In-app notification: brief, links to details
- Internal announcement: what the team needs to know
- Tone: transparent, empathetic, solution-oriented

Phase 2 — Migration support (4-8 weeks before):
- Follow-up email to users who haven't migrated
- Help center article: step-by-step migration guide
- FAQ: anticipated questions with honest answers
- For high-value accounts: personal outreach talking points

Phase 3 — Final warning (1-2 weeks before):
- Last-chance email with clear deadline
- In-app banner: urgent but not alarmist
- Support team briefing: expected ticket volume and escalation path

Phase 4 — Post-removal:
- Confirmation email: what happened, where to find their data, who to contact
- Updated help docs: remove references to sunset feature

For each communication: draft the copy, specify the audience, and note the delivery channel.
```

### Step 4: Stakeholder Alignment (1 hour)

```
Draft a decision document for the sunset:

1. What we're sunsetting and why (business rationale)
2. Impact: users affected, revenue at risk, migration cost
3. Migration plan summary
4. Communication timeline
5. Risk: what could go wrong and how we mitigate
6. Ask: approval to proceed with [date] for announcement

Also draft a FAQ for internal stakeholders:
- "Why are we doing this?" — [business rationale]
- "What about customer X who depends on this?" — [migration plan for key accounts]
- "What if churn spikes?" — [monitoring plan and rollback criteria]
- "Can we just leave it?" — [cost of maintenance vs. benefit of removal]
```

## Output

- Impact analysis with user segments, revenue risk, and maintenance cost
- Migration plan with timeline, user guides, and support resources
- Multi-phase communication package (emails, in-app, help docs, FAQs)
- Stakeholder decision document
- Internal FAQ for customer-facing teams

## Common Pitfalls

1. **Not enough notice.** Minimum 8 weeks for a minor feature, 6+ months for a product or API that external systems depend on. Rushed sunsets destroy trust.
2. **No migration path.** "We're removing this" without "here's what to do instead" is abandonment. Always provide an alternative, even if it's an export.
3. **Burying the news.** Don't hide a sunset in a changelog. Proactive, direct communication shows respect for the users who relied on this feature.
4. **Ignoring high-value accounts.** If enterprise customers depend on this, they need personal outreach, not a mass email. Coordinate with their account team.
5. **No monitoring after removal.** Track churn, support tickets, and sentiment for 30 days post-removal. If the impact is worse than projected, have a response plan ready.

## Related Skills

- [Stakeholder Alignment](../stakeholder-alignment/SKILL.md) — when the sunset decision is contentious
- [Go-to-Market Planning](../go-to-market-planning/SKILL.md) — if the sunset coincides with a replacement launch
- Reference: [TEMPLATES.md](../../TEMPLATES.md) — Release Communication, FAQ, and Readiness Checklist templates
