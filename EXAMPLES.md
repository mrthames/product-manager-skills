# Examples

Practical demonstrations of the Product Manager Guidelines applied to real scenarios.

---

## Principle 1: Start With the Problem, Not the Solution

### Before (Anti-Pattern)

> "Write a PRD for adding a notification preferences page."

Claude generates a full spec for a notification preferences UI — settings toggles, frequency controls, channel selection — without knowing why it's needed.

### After (Guideline Applied)

> "Users are churning because they feel spammed by notifications (exit survey data: 34% cite 'too many emails'). We need to reduce notification-driven churn. A preferences page is one option — what else should we consider? Start with the problem framing."

Claude frames the problem, explores multiple solutions (preferences page, smarter defaults, digest mode, quiet hours), and recommends which to investigate first based on the evidence provided.

---

## Principle 2: Write for Builders

### Before (Anti-Pattern)

```markdown
## Requirements
- Users should be able to manage their notification preferences
- The experience should be intuitive and user-friendly
- It should work across all platforms
```

Vague, untestable, requires multiple follow-up conversations before any engineer or designer can start work.

### After (Guideline Applied)

```markdown
## User Stories

**As a** registered user receiving email notifications,
**I want to** choose which notification types I receive,
**so that** I only get emails relevant to my usage.

### Acceptance Criteria
- [ ] User can toggle on/off each notification category independently
- [ ] Categories: account security, product updates, activity alerts, marketing
- [ ] Changes persist immediately (no separate save action)
- [ ] Default state for new users: security ON, all others OFF
- [ ] Unsubscribe link in emails deep-links to this page with the relevant category highlighted

### Edge Cases
- User disables all categories: show confirmation warning that security notifications are recommended
- User has no verified email: show prompt to verify before enabling non-security notifications
- API failure on save: show inline error, retain the previous state, do not silently revert

### Technical Constraints
- Must integrate with existing email service provider (SendGrid)
- Preference state stored in user profile service, not email provider
- Changes must propagate to email provider within 5 minutes
```

An engineer — or their AI coding tool — can begin implementation from this spec without a follow-up meeting.

---

## Principle 3: Define Done Before Starting

### Before (Anti-Pattern)

> "Success: users adopt the notification preferences page."

### After (Guideline Applied)

> **Success Metrics:**
> - Primary: Notification-related churn decreases by 15% within 60 days of launch (baseline: 34% of churning users cite notifications)
> - Secondary: 40% of active users customize at least one preference within 30 days
> - Guardrail: Overall email open rate does not drop below 22% (current: 28%) — if users over-suppress, we may hurt engagement
>
> **Measurement plan:** Track via Mixpanel events on preference changes, cross-referenced with churn cohort analysis in our data warehouse. Run as a staged rollout (10% → 50% → 100%) with a 2-week hold at each stage.

---

## Principle 4: Scope Ruthlessly

### Before (Anti-Pattern)

A PRD that includes notification preferences, a notification center inbox, push notification support, scheduled digest emails, notification templates for admins, and an analytics dashboard — all in v1.

### After (Guideline Applied)

```markdown
## Scope

### v1 (Ship This)
- Email notification preferences page (toggle by category)
- Four categories: security, product updates, activity alerts, marketing
- Deep-link from unsubscribe in emails

### Deferred (Validated by v1 Results)
- Push notification preferences — defer until we validate email preferences reduce churn
- Digest mode — requires new email infrastructure; pursue only if preference toggles alone don't hit the 15% churn reduction target
- Notification center inbox — separate initiative; not required for the churn hypothesis
- Admin notification templates — internal tooling; schedule separately

### Cut (Not Doing)
- Per-notification granularity (too complex for v1; category-level is sufficient)
- AI-recommended preferences (speculative; no evidence users want this)
```

---

## Principle 5: Stay Evidence-Based

### Before (Anti-Pattern)

> "Our competitors all have notification preferences, so we need one too."

### After (Guideline Applied)

> **Evidence supporting this initiative:**
> - **Strong (data):** 34% of churning users cite notification volume in exit surveys (n=847, last 90 days)
> - **Moderate (inferred):** Support tickets about notifications increased 22% QoQ, suggesting growing dissatisfaction
> - **Weak (assumption):** Competitors offering preferences may be contributing to higher retention — but we have no data on their retention rates or whether preferences are the cause
>
> **Recommendation:** The exit survey data alone justifies the initiative. Competitor parity is a supporting argument, not the driver. If we can't articulate the user problem, competitor features should not move prioritization.

---

## Stakeholder Communication Examples

### Team-Level Update

> **Sprint 14 Status — Notification Preferences**
>
> **Shipped:** Preference page UI (all 4 categories), deep-link from unsubscribe.
> **In progress:** SendGrid integration — propagation delay is 12min, target is 5min. Engineering investigating.
> **Blocked:** QA environment doesn't have SendGrid sandbox configured. Need DevOps support by Wednesday or we slip the staged rollout by a week.
> **Next sprint:** 10% rollout if SendGrid propagation is resolved.

### Executive-Level Update

> **Notification Preferences — Executive Summary**
>
> **Headline:** On track to begin staged rollout next week. Targeting 15% reduction in notification-driven churn (currently 34% of churn exits).
>
> **Status:** Feature complete. One technical issue (email propagation delay) being resolved this week.
>
> **Ask:** None at this time. Will escalate if rollout results at 10% don't trend toward the 15% target within 2 weeks.
>
> **Risk:** If preference adoption is lower than 40%, we may need to explore smarter defaults rather than user-driven preferences — would require a design pivot and ~3 additional weeks.

---

## Human-in-the-Loop in Practice

### What Claude Does

- Generates the first draft of the PRD from your problem statement
- Enumerates edge cases you might miss
- Applies RICE scoring to your backlog data
- Structures the stakeholder update in the right format and tone
- Synthesizes 200 support tickets into 5 themes with frequency counts

### What You Do

- Decide whether the problem is worth solving
- Validate that the acceptance criteria match what you actually mean
- Override the RICE score when strategic context says otherwise
- Add the political context and relationship nuance to the stakeholder update
- Read the raw tickets that sit behind the most surprising theme to verify Claude's interpretation

The pattern: Claude does the first 80% (structure, thoroughness, formatting). You do the last 20% (judgment, context, decisions). That last 20% is the part that matters most.
