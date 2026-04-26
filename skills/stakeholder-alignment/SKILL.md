---
name: stakeholder-alignment
description: Align stakeholders on priorities, scope, or direction when there's disagreement. Use when you need buy-in fast, not just a status update.
---

# Stakeholder Alignment

Get stakeholders aligned on a decision in hours, not weeks of back-channel meetings. This skill covers stakeholder mapping, decision-forcing documents, objection pre-emption, and structured alignment sessions — not just drafting updates.

## When to Use

- Stakeholders disagree on priorities and you need a decision
- You're proposing a significant scope change or trade-off
- A new initiative needs executive sponsorship
- Engineering and business stakeholders have conflicting goals
- You need to kill a pet project with evidence, not politics

## When NOT to Use

- You need to write a routine status update — use the stakeholder update templates in TEMPLATES.md
- You're reporting results, not seeking alignment — use the executive update template
- The decision has already been made and you're communicating it — that's communication, not alignment

## The AI-Native Approach

**Traditional alignment:** Weeks of 1:1 meetings, hallway conversations, slide decks revised six times, alignment meetings that don't align.

**AI-native alignment:** 2-4 hours of preparation with Claude, then one structured session or async review that forces a decision.

| Step | Time | Claude Does | You Do |
|---|---|---|---|
| Map stakeholders | 20 min | Generate stakeholder map from context | Validate concerns, add political context |
| Build decision document | 1-2 hrs | Draft options with trade-offs, evidence, and recommendations | Add strategic framing and relationship context |
| Pre-empt objections | 30 min | Anticipate objections from each stakeholder's perspective | Validate and add objections Claude would miss |
| Run the alignment | 30-60 min | (Not present) | Facilitate the meeting or async review |
| Capture decisions | 15 min | Structure the decision memo | Confirm with stakeholders |

## Process

### Step 1: Map Stakeholders (20 minutes)

```
I need to align stakeholders on [decision/initiative]. Here's the context:
- [What needs to be decided]
- [Why it's contentious or complex]
- [Who's involved and what you know about their positions]

Generate a stakeholder map:
- For each stakeholder: their role, what they care about, likely position, and what would change their mind
- Identify who's a decision-maker vs. influencer vs. informed
- Flag potential alliances and conflicts between stakeholders
```

Add what Claude can't know: the relationship dynamics, political history, and unspoken concerns.

### Step 2: Build a Decision-Forcing Document (1-2 hours)

A decision-forcing document is not a recommendation deck — it's a structured presentation of options that makes it impossible to leave the room without a decision.

```
Draft a decision document for [decision]. Structure it as:

1. Context: What happened that requires a decision (2-3 sentences)
2. Decision needed: Exactly what we're deciding, in one sentence
3. Options (3 max):
   - For each: what it is, what it costs, what it gets us, what we give up
   - Evidence supporting each option
   - Who benefits and who bears the cost
4. Recommendation: Which option and why
5. What happens if we don't decide: The cost of inaction
6. Decision deadline: When this needs to be resolved and why

Tailor the framing for these stakeholders: [stakeholder list with concerns].
```

### Step 3: Pre-empt Objections (30 minutes)

```
For each stakeholder in our map, anticipate their top 2-3 objections to the
recommended option. For each objection:
- State it in their words (how they'd actually phrase it)
- Provide the evidence-based response
- Identify where they're right (concessions you can make)
- Flag any objections that would change the recommendation if valid
```

Review Claude's output. Add the objections that come from political context, history, or personality that Claude wouldn't know.

### Step 4: Run the Alignment (30-60 minutes)

This is the human step. Two approaches:

**Synchronous (meeting):**
- Share the decision document 24 hours before the meeting
- Open with "here's what we need to decide and why it can't wait"
- Walk through options — let stakeholders react
- When objections come up, address them (you've pre-empted them)
- Close with a decision or a clear next step with a deadline

**Asynchronous (for distributed teams):**
- Share the decision document with a deadline for comments
- Ask each stakeholder to state their preferred option and why
- Synthesize responses and flag disagreements
- Escalate only genuine disagreements to a synchronous decision

### Step 5: Capture the Decision (15 minutes)

```
Based on the alignment session, draft a decision memo:
- Decision made: [what was decided]
- Options considered: [brief summary]
- Rationale: [why this option]
- Dissent: [who disagreed and what was their concern]
- Next steps: [who does what by when]
- Review date: [when we revisit if needed]

Format for [audience — team Slack, email to leadership, Confluence page].
```

## Output

- Stakeholder map with concerns and likely positions
- Decision-forcing document with options, trade-offs, and recommendation
- Objection-response matrix
- Decision memo with captured dissent and next steps

## Common Pitfalls

1. **Seeking consensus instead of a decision.** Consensus is everyone agreeing. Alignment is everyone understanding the decision and committing to it, even if they'd choose differently. Aim for alignment.
2. **Presenting one option as a recommendation.** If there's only one option, you're informing, not aligning. Decision-forcing documents need real alternatives.
3. **Skipping the "cost of inaction."** Stakeholders who are comfortable with the status quo need to understand what doing nothing costs. Quantify it.
4. **Letting the meeting end without a decision.** If the deadline passes without resolution, escalate. Indecision has a cost — that's why you calculated it.
5. **Ignoring dissent.** Capturing dissent is not just good practice — it protects the decision. When things go wrong (they will), the dissent record shows what was considered.

## Related Skills

- [Product Strategy & Vision](../product-strategy-vision/SKILL.md) — when alignment is needed on strategic direction
- [Tech Debt Communication](../tech-debt-communication/SKILL.md) — when the alignment topic is engineering investment
- [Pricing & Packaging](../pricing-packaging/SKILL.md) — when the alignment topic is pricing decisions
- Reference: [TEMPLATES.md](../../TEMPLATES.md) — Stakeholder Update templates for post-decision communication
