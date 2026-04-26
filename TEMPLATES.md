# Artifact Templates

Starter templates for product management artifacts. Each template is structured for AI-native workflows — designed to be generated with Claude Code, reviewed by you, and consumed by engineers and designers using AI tools.

Copy the relevant template into your Claude Code session and fill in the bracketed sections to get started.

---

## Table of Contents

- [Product Requirements Document (PRD)](#product-requirements-document-prd)
- [Epic](#epic)
- [Feature](#feature)
- [User Story with Acceptance Criteria](#user-story-with-acceptance-criteria)
- [Experiment Brief](#experiment-brief)
- [Competitive Analysis](#competitive-analysis)
- [Prioritization Scorecard](#prioritization-scorecard)
- [Stakeholder Update — Team Level](#stakeholder-update--team-level)
- [Stakeholder Update — Executive Level](#stakeholder-update--executive-level)
- [Release Communication — Customer Facing](#release-communication--customer-facing)
- [Product Readiness Checklist](#product-readiness-checklist)
- [FAQ — Internal](#faq--internal)
- [FAQ — External](#faq--external)
- [Training Outline](#training-outline)
- [How-To Guide](#how-to-guide)

---

## Product Requirements Document (PRD)

```markdown
# [Feature Name]

**Status:** Draft | In Review | Approved
**Author:** [PM name]
**Last updated:** [Date]
**Engineering lead:** [Name]
**Design lead:** [Name]

---

## Problem Statement

**Who** is affected: [specific user segment]
**What** they experience: [the problem in their words]
**Evidence:**
- [Data point 1 — source, date, sample size]
- [Data point 2]
- [Data point 3]
**Impact if unaddressed:** [business/user consequence]

## Success Metrics

| Metric | Type | Target | Baseline | Measurement Method |
|---|---|---|---|---|
| [Primary metric] | Outcome | [target] | [current] | [how measured] |
| [Secondary metric] | Outcome | [target] | [current] | [how measured] |
| [Guardrail metric] | Guardrail | [threshold] | [current] | [how measured] |

**Evaluation timeline:** [when we assess success — e.g., 30 days post-launch]

## Solution

**Approach:** [1-2 sentence summary of the chosen approach]
**Why this approach:** [what alternatives were considered and why this one was selected]

## Scope

### v1 — Ship This
- [Capability 1]
- [Capability 2]
- [Capability 3]

### Deferred — Validated by v1 Results
- [Deferred item 1 — trigger for inclusion]
- [Deferred item 2 — trigger for inclusion]

### Out of Scope
- [Excluded item 1 — why]
- [Excluded item 2 — why]

## User Stories

[Link to or inline the user stories — see User Story template below]

## Technical Constraints
- [Platform/infrastructure constraints]
- [API contracts or integration requirements]
- [Performance requirements — latency, throughput, availability]
- [Data/privacy requirements]

## Dependencies
- [Team/system 1 — what's needed and by when]
- [Team/system 2 — what's needed and by when]

## Risks
| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| [Risk 1] | [H/M/L] | [H/M/L] | [Plan] |
| [Risk 2] | [H/M/L] | [H/M/L] | [Plan] |

## Readiness Requirements
- [ ] Internal FAQ drafted and reviewed by support
- [ ] External help article drafted
- [ ] Release notes written
- [ ] Training completed for [affected teams]
- [ ] Monitoring and alerts configured
- [ ] Rollback plan documented
```

---

## Epic

```markdown
# Epic: [Epic Name]

**Status:** Draft | In Review | Approved | In Progress | Complete
**Owner:** [PM name]
**Target quarter:** [Q# YYYY]
**Last updated:** [Date]

---

## Strategic Context

**Objective:** [What this epic achieves — tied to a company or product goal]
**Key result:** [Measurable outcome this epic drives — e.g., "Reduce onboarding drop-off from 40% to 25%"]
**Theme:** [Product theme or pillar this falls under — e.g., Growth, Retention, Platform]

## Problem Statement

[The user or business problem this epic addresses. Same rigor as a PRD — ground it in evidence, not assumption.]

**Evidence:**
- [Data point 1 — source, date]
- [Data point 2]

## Scope

### Features Included

| Feature | Description | Status | Owner |
|---|---|---|---|
| [Feature 1] | [One-line summary] | Not Started | [Name] |
| [Feature 2] | [One-line summary] | Not Started | [Name] |
| [Feature 3] | [One-line summary] | Not Started | [Name] |

### Out of Scope
- [What this epic explicitly does not include — and why]

## Success Metrics

| Metric | Target | Baseline | Measurement Method |
|---|---|---|---|
| [Primary outcome metric] | [target] | [current] | [how measured] |
| [Secondary metric] | [target] | [current] | [how measured] |
| [Guardrail] | [threshold] | [current] | [how measured] |

## Dependencies

| Dependency | Team/System | Status | Needed By |
|---|---|---|---|
| [Dependency 1] | [team] | [resolved/pending] | [date] |
| [Dependency 2] | [team] | [resolved/pending] | [date] |

## Risks

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| [Risk 1] | [H/M/L] | [H/M/L] | [Plan] |
| [Risk 2] | [H/M/L] | [H/M/L] | [Plan] |

## Timeline

| Milestone | Target Date | Features Included |
|---|---|---|
| [Milestone 1 — e.g., "Design complete"] | [Date] | [Feature 1, Feature 2] |
| [Milestone 2 — e.g., "Beta launch"] | [Date] | [Feature 1] |
| [Milestone 3 — e.g., "GA launch"] | [Date] | [All features] |

## Stakeholders

| Stakeholder | Role | Interest |
|---|---|---|
| [Name/Team] | [Approver / Informed / Consulted] | [What they care about] |
```

---

## Feature

```markdown
# Feature: [Feature Name]

**Epic:** [Parent epic name and link]
**Status:** Draft | In Review | Approved | In Progress | Complete
**Owner:** [PM name]
**Engineering lead:** [Name]
**Design lead:** [Name]
**Last updated:** [Date]

---

## Overview

[2-3 sentence summary of what this feature does and why it exists. Should be understandable by anyone on the team without additional context.]

## User Problem

**Who:** [Specific user segment]
**Problem:** [What they experience today]
**Impact:** [Why this matters — frequency, severity, business consequence]

## Solution Summary

**Approach:** [What we're building — one paragraph]
**Why this approach:** [Alternatives considered and why this was chosen]

## User Stories

| Story | Priority | Points | Status |
|---|---|---|---|
| [Story 1 — as a user, I want to...] | Must-have | [est.] | Not Started |
| [Story 2] | Must-have | [est.] | Not Started |
| [Story 3] | Nice-to-have | [est.] | Not Started |

[Link to detailed user stories with acceptance criteria]

## Design

**Design status:** Not Started | In Progress | Complete
**Design link:** [Figma/design file URL]

**Key design decisions:**
- [Decision 1 — what was decided and why]
- [Decision 2]

## Technical Considerations

- [API contracts or integration points]
- [Performance requirements]
- [Data model changes]
- [Migration needs]
- [Infrastructure or scaling considerations]

## Scope Boundaries

**In scope:**
- [Specific capability 1]
- [Specific capability 2]

**Deferred to next iteration:**
- [Deferred item 1 — trigger for inclusion]
- [Deferred item 2]

**Out of scope:**
- [Excluded item — why]

## Success Metrics

| Metric | Target | Baseline | When to Measure |
|---|---|---|---|
| [Adoption metric] | [target] | [current] | [timeframe post-launch] |
| [Engagement metric] | [target] | [current] | [timeframe] |
| [Guardrail] | [threshold] | [current] | [ongoing] |

## Dependencies

- [Dependency 1 — team, what's needed, by when]
- [Dependency 2]

## Rollout Plan

| Stage | Audience | Duration | Success Criteria to Advance |
|---|---|---|---|
| Internal dogfood | Team | [duration] | [criteria] |
| Beta / 10% | [segment] | [duration] | [criteria] |
| 50% | [segment] | [duration] | [criteria] |
| GA / 100% | All users | — | — |

## Readiness

- [ ] Acceptance criteria reviewed with engineering
- [ ] Design approved
- [ ] Internal FAQ drafted
- [ ] External help article drafted
- [ ] Monitoring configured
- [ ] Rollback plan documented
```

---

## User Story with Acceptance Criteria

```markdown
## [Story Title]

**As a** [user type],
**I want to** [action],
**so that** [outcome/benefit].

### Acceptance Criteria

- [ ] [Specific, testable criterion 1]
- [ ] [Specific, testable criterion 2]
- [ ] [Specific, testable criterion 3]

### Edge Cases

- [Edge case 1]: [expected behavior]
- [Edge case 2]: [expected behavior]

### Error States

- [Error condition 1]: [expected behavior and user messaging]
- [Error condition 2]: [expected behavior and user messaging]

### Technical Notes

- [API endpoint, data model, or integration detail relevant to implementation]
- [Performance expectation — e.g., response within 200ms]

### Design References

- [Link to Figma/design file if available]
- [Key interaction patterns or existing components to reuse]
```

---

## Experiment Brief

```markdown
# Experiment: [Name]

**Hypothesis:** If we [change], then [user segment] will [measurable behavior change],
because [reasoning based on evidence].

## Background
- [What we know — data, research, prior experiments]
- [What we don't know — the gap this experiment fills]

## Design

**Type:** A/B test | Multivariate | Feature flag rollout | Other
**Control:** [current experience]
**Variant(s):** [what changes]
**Audience:** [segment, percentage, geography]
**Duration:** [minimum runtime based on sample size]
**Sample size needed:** [calculated MDE and statistical power]

## Success Criteria

| Metric | Threshold | Direction |
|---|---|---|
| [Primary metric] | [minimum detectable effect] | [increase/decrease] |
| [Guardrail metric] | [do not cross] | [must stay above/below] |

## Decision Framework

- If primary metric hits threshold: [action — ship, iterate, expand]
- If primary metric is inconclusive: [action — extend, redesign, kill]
- If guardrail metric is breached: [action — kill immediately, investigate]

## Rollback Plan
- [How to revert if something goes wrong]
- [Who has the authority to kill the experiment]
```

---

## Competitive Analysis

```markdown
# Competitive Analysis: [Domain/Feature Area]

**Date:** [Date]
**Analyst:** [Name]

## Landscape Overview

| Competitor | Market Position | Relevant Feature | Key Differentiator |
|---|---|---|---|
| [Competitor 1] | [position] | [their version of this feature] | [what makes theirs different] |
| [Competitor 2] | [position] | [their version] | [differentiator] |
| [Competitor 3] | [position] | [their version] | [differentiator] |

## Detailed Comparison

### [Competitor 1]
- **What they do well:** [specific strengths]
- **What they miss:** [gaps or weaknesses]
- **User sentiment:** [app store reviews, social media, forums — with sources]
- **Relevance to us:** [why this matters for our users specifically]

### [Competitor 2]
[Same structure]

## Our Positioning

- **Our strengths relative to market:** [what we do better]
- **Our gaps relative to market:** [where we're behind]
- **Opportunities:** [unmet needs no competitor addresses well]

## Recommendation

[What this analysis means for our roadmap — grounded in user needs, not competitor parity]

**Evidence strength:** [Strong/Moderate/Weak — how confident are we in this data]
```

---

## Prioritization Scorecard

```markdown
# Prioritization: [Quarter/Cycle]

**Framework:** RICE | ICE | Weighted Scoring | MoSCoW
**Date:** [Date]
**Decision-maker:** [PM name]

## Scoring Criteria

| Factor | Definition | Scale |
|---|---|---|
| [Factor 1 — e.g., Reach] | [How many users affected per quarter] | [1-10 or absolute number] |
| [Factor 2 — e.g., Impact] | [How much it moves the target metric] | [1-10] |
| [Factor 3 — e.g., Confidence] | [How sure we are about reach and impact] | [percentage] |
| [Factor 4 — e.g., Effort] | [Engineering weeks to ship v1] | [person-weeks] |

## Scored Backlog

| Initiative | [F1] | [F2] | [F3] | [F4] | Score | Notes |
|---|---|---|---|---|---|---|
| [Item 1] | | | | | | |
| [Item 2] | | | | | | |
| [Item 3] | | | | | | |

## Prioritized Ranking

1. [Item] — [one-line rationale]
2. [Item] — [one-line rationale]
3. [Item] — [one-line rationale]

## Overrides and Context

[Any items where you're overriding the framework score and why — strategic importance,
dependencies, stakeholder commitments, technical debt thresholds, etc.]
```

---

## Stakeholder Update — Team Level

```markdown
# [Project Name] — Sprint [N] Update

**Date:** [Date]
**PM:** [Name]

## Status: 🟢 On Track | 🟡 At Risk | 🔴 Blocked

## Shipped This Sprint
- [What was completed — be specific]

## In Progress
- [What's underway — include owner and expected completion]

## Blocked
- [What's stuck, why, and what's needed to unblock]
- **Action needed from:** [specific person or team] **by:** [date]

## Upcoming
- [What's planned for next sprint]

## Metrics
- [Key metric]: [current value] vs. [target] — [trend: improving/flat/declining]

## Risks
- [Risk]: [mitigation plan]
```

---

## Stakeholder Update — Executive Level

```markdown
# [Initiative Name] — Executive Update

**Date:** [Date]
**PM:** [Name]

## Headline

[One sentence: the most important thing leadership needs to know]

## Status: 🟢 On Track | 🟡 At Risk | 🔴 Needs Decision

## Progress Against Milestones

| Milestone | Target Date | Status | Notes |
|---|---|---|---|
| [Milestone 1] | [Date] | ✅ Complete | |
| [Milestone 2] | [Date] | 🔄 In Progress | [brief note] |
| [Milestone 3] | [Date] | ⏳ Upcoming | |

## Business Impact

- [Primary metric]: [current] → [projected] ([% change])
- [Revenue/cost/efficiency impact in dollars or percentages]

## Ask

[What you need from leadership — decision, resources, air cover, nothing]

## What Happens If We Do Nothing

[The cost of inaction — quantified if possible]
```

---

## Release Communication — Customer Facing

```markdown
# [Feature Name] — Now Available

**Date:** [Release date]

## What's New

[2-3 sentences describing what changed, written from the user's perspective. Focus on
the benefit, not the implementation.]

## How It Works

1. [Step 1 — what the user does]
2. [Step 2]
3. [Step 3]

## What You Need to Do

[Any action required from users — migration steps, settings to update, or "nothing, it's
automatic"]

## FAQ

**Q: [Most likely user question]**
A: [Direct answer]

**Q: [Second most likely question]**
A: [Direct answer]

## Feedback

[How to reach you — support channel, feedback form, email]
```

---

## Product Readiness Checklist

```markdown
# Readiness Checklist: [Feature Name]

**Target launch:** [Date]
**PM:** [Name]
**Readiness owner:** [Name — may be PM or program manager]

## Documentation Readiness
- [ ] Internal FAQ reviewed by support team
- [ ] External FAQ reviewed by support team
- [ ] Help center article drafted and reviewed
- [ ] How-to guide drafted and reviewed
- [ ] Release notes written
- [ ] Changelog updated

## Training Readiness
- [ ] Support team training completed
- [ ] Sales team briefed (if applicable)
- [ ] Customer success team briefed (if applicable)
- [ ] Training materials published to [system]

## Communication Readiness
- [ ] Internal announcement drafted
- [ ] Customer-facing release communication drafted
- [ ] Executive summary prepared
- [ ] Partner/vendor notifications sent (if applicable)

## Operational Readiness
- [ ] Monitoring and alerts configured
- [ ] Rollback plan documented and tested
- [ ] Staged rollout plan defined (percentages and criteria)
- [ ] On-call team briefed on the feature
- [ ] Escalation path documented

## Data Readiness
- [ ] Analytics events implemented and verified
- [ ] Dashboard or reporting updated
- [ ] Baseline metrics captured pre-launch
- [ ] Success criteria measurement plan confirmed

## Sign-Off
| Role | Name | Approved | Date |
|---|---|---|---|
| Product | | ☐ | |
| Engineering | | ☐ | |
| Design | | ☐ | |
| Support | | ☐ | |
| Legal/Compliance (if needed) | | ☐ | |
```

---

## FAQ — Internal

```markdown
# Internal FAQ: [Feature Name]

**For:** Support, Sales, Customer Success teams
**Last updated:** [Date]
**Contact for questions:** [PM name and channel]

---

**Q: What is [feature name]?**
A: [Plain-language explanation of what it does and why it exists]

**Q: Who gets access to this feature?**
A: [Plans, tiers, geographies, rollout stages]

**Q: When does it launch?**
A: [Date and rollout plan — staged percentages if applicable]

**Q: What problem does this solve for customers?**
A: [The user problem — same framing as the PRD]

**Q: How does it work?**
A: [Step-by-step from the user's perspective]

**Q: What are the known limitations?**
A: [What it doesn't do yet — be honest, support teams need this]

**Q: What if a customer reports a bug?**
A: [Triage path — who to escalate to, what information to collect]

**Q: What if a customer asks for [deferred feature]?**
A: [Talking points — acknowledge the need, share the timeline if known]

**Q: Are there any billing or pricing changes?**
A: [Yes/no — details if yes]

**Q: Where can I learn more?**
A: [Links to help articles, training recordings, PRD, design files]
```

---

## FAQ — External

```markdown
# FAQ: [Feature Name]

---

**What is [feature name]?**
[One-sentence answer in plain language]

**How do I use it?**
[Brief steps or link to how-to guide]

**Is it available on my plan?**
[Which plans/tiers include this feature]

**Do I need to do anything to get started?**
[Any setup required, or "it's available automatically"]

**What if something isn't working?**
[How to get help — support link, email, chat]

**Will this change how [existing feature] works?**
[Address the most common concern about disruption to current workflows]
```

---

## Training Outline

```markdown
# Training: [Feature Name]

**Audience:** [Support / Sales / Customer Success / All]
**Duration:** [30 min / 60 min]
**Trainer:** [Name]
**Date:** [Date]

## Agenda

| Time | Topic | Format |
|---|---|---|
| 5 min | Why we built this — the user problem | Presentation |
| 10 min | Demo — how it works | Live walkthrough |
| 10 min | Common scenarios and edge cases | Q&A with examples |
| 5 min | What to do when something goes wrong | Escalation paths |
| [Remaining] | Open Q&A | Discussion |

## Key Points to Cover
- [Point 1 — what the team needs to know to do their job]
- [Point 2]
- [Point 3]

## Resources
- [Link to help article]
- [Link to internal FAQ]
- [Link to recording (post-session)]
```

---

## How-To Guide

```markdown
# How to [Accomplish Specific Task]

## Before You Start

**You'll need:**
- [Prerequisite 1 — account type, permissions, etc.]
- [Prerequisite 2]

## Steps

### Step 1: [Action]
[What to do, where to find it, what it looks like]

### Step 2: [Action]
[Instructions — be specific about button names, menu locations, field labels]

### Step 3: [Action]
[Instructions]

## Result
[What the user should see when they're done — confirmation message, changed state, etc.]

## Troubleshooting

**[Problem 1]:** [Solution]
**[Problem 2]:** [Solution]

## Related
- [Link to related guide]
- [Link to FAQ]
```
