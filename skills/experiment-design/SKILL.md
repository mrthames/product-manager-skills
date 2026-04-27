---
name: experiment-design
description: Design and run lean experiments — hypothesis, cheapest test, success criteria, decision. Use when you need to validate before you build.
---

# Experiment Design & Monitoring

The core lean loop: build-measure-learn. This skill structures the full cycle — from shaky assumption to validated learning — so you test cheaply and decide fast. Claude designs the experiment framework and monitors the results. You define what you're betting on and make the call when the data comes in.

## When to Use

- You have a hypothesis but aren't sure it's worth a full build
- Leadership wants evidence before committing engineering resources
- You're choosing between multiple solutions and need data, not opinions
- A feature launched but you need to validate it's actually changing behavior
- You want to run an A/B test and need a rigorous setup

## When NOT to Use

- You're exploring a problem space — use Discovery Process first
- You need to align stakeholders on whether to experiment — use Stakeholder Alignment
- You're reviewing existing metrics, not testing a hypothesis — use Metrics Review

## The AI-Native Approach

| Step | Time | Claude Does | You Do |
|---|---|---|---|
| Map assumptions | 20 min | Structure assumptions from your context, rank by risk | Validate which assumptions are truly unproven |
| Design the experiment | 30 min | Propose cheapest valid test, define metrics and criteria | Confirm feasibility with engineering, set guardrails |
| Build the brief | 20 min | Draft experiment brief with hypothesis, method, success criteria | Review and share with the team |
| Monitor results | Ongoing | Track metrics, flag significance and guardrails | Interpret results with product context |
| Make the call | 15 min | Summarize findings, frame the decision | Decide: ship, iterate, or kill |

## Process

### Step 1: Map Assumptions (20 minutes)

Every product bet is a stack of assumptions. Most teams skip straight to building. Lean teams identify which assumptions are riskiest and test those first.

```
We're considering [initiative/feature]. Here are the assumptions behind it:

List every assumption we're making:
- About the user problem (is it real? how painful?)
- About the solution (will this approach work?)
- About the market (will people pay? switch? adopt?)
- About feasibility (can we build it in time? at this cost?)

For each assumption:
- How confident are we? (high / medium / low)
- What's the consequence if we're wrong? (high / medium / low)
- Is there existing evidence? (data, research, analogues)

Rank by risk: low confidence + high consequence = test this first.
```

### Step 2: Design the Experiment (30 minutes)

The goal is the cheapest, fastest test that gives you a decision-quality signal. Not a perfect study — a lean experiment.

```
For our riskiest assumption: [assumption]

Design the cheapest valid experiment:

Hypothesis: "We believe [this] will cause [that] for [whom]."
Null hypothesis: "There is no meaningful difference when [this] changes."

Method options (from cheapest to most expensive):
1. Fake door / painted door test
2. Concierge / manual-behind-the-scenes
3. Wizard of Oz prototype
4. A/B test on existing feature
5. Limited beta / feature flag rollout
6. Full A/B test on new feature

For the recommended method:
- What do we build/change? (minimum implementation)
- Who do we expose it to? (segment, sample size)
- How long do we run it? (minimum duration for significance)
- What do we measure? (primary metric, secondary, guardrails)

Success criteria:
- Ship if: [primary metric] improves by [X%] with [confidence level]
- Iterate if: [signal is positive but below threshold]
- Kill if: [no signal or guardrail metric degrades by Y%]

Guardrail metrics (must not degrade):
- [Metric 1]: [threshold]
- [Metric 2]: [threshold]
```

### Step 3: Build the Experiment Brief (20 minutes)

```
Draft an experiment brief:

1. Background: Why we're running this experiment (1-2 sentences)
2. Hypothesis: Stated as testable prediction
3. Method: What changes, for whom, for how long
4. Primary metric: What we measure, target, baseline
5. Secondary metrics: Supporting signals
6. Guardrail metrics: What must not degrade
7. Sample size and duration: Minimum for statistical significance
8. Success criteria: Ship / iterate / kill thresholds
9. Decision date: When we read the results and decide
10. Owner: Who makes the call

Keep it to one page. If the brief is longer than the experiment, you're over-engineering it.
```

### Step 4: Monitor Results (Ongoing)

```
Here are the current experiment results: [paste data or describe]

Analyze:
- Are we reaching statistical significance? How many more days at current rate?
- Is the primary metric trending toward the success threshold?
- Are any guardrail metrics showing degradation?
- Are there segment-level differences worth investigating?
- Any external factors that could be confounding results?

Flag:
- 🟢 On track — continue running
- 🟡 Mixed signals — may need more time or investigation
- 🔴 Guardrail breach — consider stopping early
- ✅ Reached significance — ready for decision
```

### Step 5: Make the Call (15 minutes)

```
The experiment has concluded. Here are the final results: [data]

Summarize:
1. Did the primary metric hit the success threshold?
2. Did any guardrail metrics degrade?
3. Were there surprising segment-level differences?
4. What did we learn that we didn't expect?

Frame the decision:
- Ship: results met criteria, here's the rollout plan
- Iterate: signal is there but we need to adjust [what] and retest
- Kill: no meaningful signal, here's what we learned and what to try next

Either way: what's the validated learning? What do we now know that we didn't before?
```

## Output

- Ranked assumption map with risk scores
- Experiment brief (hypothesis, method, metrics, success criteria)
- Monitoring summary with significance tracking
- Decision recommendation with validated learning

## Common Pitfalls

1. **Testing too many things at once.** One hypothesis per experiment. If you're testing three things simultaneously, you won't know which one caused the result.
2. **Calling it too early.** Wait for statistical significance. Early reads are noise. Set the duration upfront and stick to it unless a guardrail breaches.
3. **No kill criteria.** If you only define "success," you'll always find a way to declare victory. Define the kill threshold before you start.
4. **Over-engineering the test.** The cheapest valid test wins. A fake door that takes a day beats an A/B test that takes a sprint. Match the test cost to the decision stakes.
5. **Learning nothing from failures.** A killed experiment isn't a failure — it's a validated learning that saved you from building the wrong thing. Document what you learned and feed it back into discovery.

## Related Skills

- [Discovery Process](../discovery-process/SKILL.md) — when you need to explore the problem space before you can form a hypothesis
- [Metrics Review](../metrics-review/SKILL.md) — for ongoing monitoring of experiment results alongside product health
- [Growth & Retention Diagnostics](../growth-retention-diagnostics/SKILL.md) — when experiment results reveal a deeper retention or growth issue
