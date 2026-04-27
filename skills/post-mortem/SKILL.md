---
name: post-mortem
description: Run a structured post-mortem after a failure, missed target, or incident. Use when you need to learn from what went wrong without blame.
---

# Post-Mortem & Retrospective

Turn a failure into actionable learning in 2-3 hours instead of a week of finger-pointing. Claude structures the timeline, surfaces contributing factors objectively, and drafts action items. You facilitate the conversation and ensure the team learns without blame.

## When to Use

- A launch went poorly (missed targets, quality issues, user backlash)
- A major incident or outage occurred
- A quarter's OKRs were significantly missed
- A key initiative was killed after significant investment
- A process breakdown caused preventable problems

## When NOT to Use

- Things went well and you want to celebrate — do that, but not with this skill
- You're doing routine sprint retrospectives — those are lighter weight than this
- The problem is ongoing — fix it first, post-mortem after

## The AI-Native Approach

| Step | Time | Claude Does | You Do |
|---|---|---|---|
| Build the timeline | 30 min | Structure events chronologically from your input | Validate accuracy, fill gaps |
| Identify contributing factors | 45 min | Categorize factors objectively without blame | Facilitate team input, add context |
| Extract lessons | 30 min | Distill what was learned and what should change | Decide which lessons lead to action |
| Draft action items | 30 min | Structure specific, assigned, time-bound actions | Confirm ownership and commitment |
| Write the post-mortem doc | 15 min | Format the complete document | Review and distribute |

## Process

### Step 1: Build the Timeline (30 minutes)

```
We're running a post-mortem on [what happened].

Here's what I know about the sequence of events:
[Paste your notes — dates, decisions, milestones, when things went wrong]

Build a chronological timeline:
- Key decisions made and by whom (no blame — just facts)
- When warning signs appeared
- When the problem became visible
- Actions taken in response
- Final outcome

Flag: at which points could a different decision have changed the outcome?
```

### Step 2: Identify Contributing Factors (45 minutes)

```
Based on the timeline, identify contributing factors. Categorize each:

1. Process factors: Were there process gaps that allowed this?
2. Communication factors: Was information available but not shared?
3. Technical factors: Were there system limitations or failures?
4. Scope/planning factors: Was the plan realistic given constraints?
5. External factors: Did something outside our control contribute?

For each factor:
- What happened (factual, blameless description)
- Why it mattered (how it contributed to the outcome)
- Whether it was visible at the time (could we have caught it?)
- Whether it's systemic (likely to recur) or one-off

Do NOT assign individual blame. Focus on systems and processes, not people.
```

This step benefits from team input. Share Claude's draft with the team and ask what's missing or mischaracterized.

### Step 3: Extract Lessons (30 minutes)

```
From the contributing factors, extract lessons learned:

For each lesson:
- What we learned (one sentence)
- Evidence (which factor(s) taught us this)
- Is this new or something we already knew but didn't act on?
- How generalizable is this? (applies to this project only, or to how we work broadly)

Prioritize: which lessons, if acted on, would have the biggest impact on
preventing similar failures?
```

### Step 4: Draft Action Items (30 minutes)

```
Convert the top lessons into action items:

For each action:
- What specifically changes (process, tooling, communication, planning)
- Owner (who is responsible for making this change)
- Deadline (when will this be implemented)
- How we verify (how do we know the change stuck)
- Scope: is this a one-time fix or an ongoing process change?

Keep it to 3-5 actions max. More than 5 means nothing gets done.
Distinguish between:
- Quick wins (can implement this week)
- Structural changes (need a project or process redesign)
- Monitoring (watch for recurrence, no action yet)
```

### Step 5: Write the Post-Mortem Document (15 minutes)

```
Format the complete post-mortem:

1. Summary: What happened, in 2-3 sentences
2. Impact: Users affected, revenue impact, reputation impact
3. Timeline: Key events in chronological order
4. Contributing factors: Categorized, blameless
5. Lessons learned: Prioritized
6. Action items: Specific, owned, time-bound
7. Follow-up date: When we review whether actions were implemented

Tone: factual, blameless, forward-looking. This document exists to prevent
recurrence, not to assign fault.
```

## Output

- Chronological event timeline
- Contributing factors categorized by type
- Prioritized lessons learned
- 3-5 specific, owned, time-bound action items
- Complete post-mortem document

## Common Pitfalls

1. **Blame culture.** The fastest way to kill learning is to punish honesty. Post-mortems must be blameless. If people fear consequences, they won't share what went wrong.
2. **Too many action items.** 3-5 max. A post-mortem with 15 action items means none of them get done. Prioritize ruthlessly.
3. **No follow-up.** Schedule a review 30 days after the post-mortem to check: did we implement the actions? Did they work? This is where most post-mortems fail.
4. **Recency bias.** The most recent failure gets the most attention. But is it representative? Check whether this is a pattern or a one-off before over-investing in prevention.
5. **Only doing post-mortems for failures.** The best learning comes from near-misses too. If something almost went wrong but didn't, that's worth analyzing — you might not get lucky next time.

## Related Skills

- [Stakeholder Alignment](../stakeholder-alignment/SKILL.md) — when post-mortem findings need executive action
- [Metrics Review](../metrics-review/SKILL.md) — monitoring for recurrence after implementing changes
- [Sprint & Release Planning](../sprint-release-planning/SKILL.md) — incorporating post-mortem actions into sprint work
