# Frameworks for AI-Native Product Management

Traditional PM frameworks were designed for a world where research synthesis took weeks, writing specs took days, and every artifact was crafted by hand. The frameworks themselves are still sound — the problems they solve haven't changed. But the execution model has.

In AI-native product development, Claude handles the mechanical parts of framework execution: structuring the analysis, running the scoring, synthesizing the inputs, and drafting the outputs. You handle the parts that require human judgment: choosing the right framework, providing the context, validating the inputs, and making the call.

The result: frameworks that used to take weeks take days. Discovery that used to require a dedicated sprint happens in focused sessions. The speed gain doesn't come from cutting corners — it comes from compressing the mechanical work so you can spend more time on the decisions that matter.

---

## Table of Contents

- [Choosing the Right Framework](#choosing-the-right-framework)
- [Discovery Process](#discovery-process)
- [Problem & Opportunity Frameworks](#problem--opportunity-frameworks)
- [Prioritization Frameworks](#prioritization-frameworks)
- [Story Splitting](#story-splitting)
- [Financial & SaaS Metrics](#financial--saas-metrics)

---

## Choosing the Right Framework

Don't start with a framework — start with the decision you need to make. The framework serves the decision, not the other way around.

```
Tell Claude: "I need to decide [decision]. Here's what I know: [context].
Which framework would help me structure this decision, and why?"
```

Claude will recommend a framework based on your situation. Use the guide below to validate or override that recommendation.

| You Need To... | Framework | When It Fits |
|---|---|---|
| Understand why users switch or stay | Jobs-to-be-Done | Exploring a new market, redesigning a core flow, or diagnosing retention |
| Map the full user experience to find gaps | Customer Journey Map | Onboarding optimization, cross-functional alignment on user pain |
| Find the highest-leverage opportunity | Opportunity Solution Tree | Multiple possible problems, need to narrow focus with evidence |
| Rank a backlog by impact | RICE / ICE | You have data on reach and impact, need to justify sequencing |
| Understand what delights vs. what's table stakes | Kano Model | Feature decisions where "users want it" isn't enough context |
| Quantify the cost of waiting | Cost of Delay | Sequencing decisions where timing is the key variable |
| Articulate your product's position | Positioning Statement | New product, repositioning, or entering a new market |
| Test a hypothesis before building | Experiment Brief | Any bet where you can validate cheaply before committing |
| Break large work into shippable slices | Story Splitting | Anything estimated above a sprint's capacity |
| Connect product work to business outcomes | SaaS Metrics | Executive conversations, investment cases, portfolio decisions |

---

## Discovery Process

Traditional discovery runs 3-4 weeks as a dedicated sprint. In AI-native development, you compress this to days by using Claude for the synthesis-heavy steps while you focus on the irreplaceable human steps: talking to users and making judgment calls.

### The AI-Native Discovery Cycle

**Day 1: Frame the Problem (2-3 hours)**

You bring the raw signal — support tickets, usage data, user quotes, business context. Claude helps you structure it.

```
Here's what I'm seeing: [raw signals].
Help me frame this as a problem statement. Who's affected, what's the evidence,
and what are we assuming vs. what do we know?
```

Output: Structured problem statement with evidence inventory and assumption list.

**Day 2: Synthesize What You Know (2-3 hours)**

Feed Claude your existing data — analytics exports, survey results, prior research, competitive context. Let it do the synthesis you'd normally spend a week on.

```
Here's our data on this problem: [data sources].
Synthesize the key findings. What patterns emerge? Where do the data sources
agree or conflict? What's the strongest evidence, and where are the gaps?
```

Output: Research synthesis with evidence strength ratings and identified gaps.

**Day 3: Talk to Users (half day)**

This is the step AI cannot replace. Talk to 3-5 users. Use Claude to prepare your discussion guide, but the conversations are yours.

```
Based on our problem statement and research gaps, generate a discussion guide
for 30-minute user interviews. Focus on [specific gaps]. Use past-behavior
questions, not hypotheticals. Flag questions that might lead the witness.
```

After interviews, feed your notes back to Claude for rapid synthesis:

```
Here are my notes from 5 user interviews on [problem]. Identify themes,
contradictions, and surprises. Flag anything that challenges our assumptions.
```

**Day 4: Map Opportunities and Decide (2-3 hours)**

Use an Opportunity Solution Tree to go from synthesized findings to actionable options.

```
Based on our research synthesis and interview findings, build an opportunity
solution tree. Start with the desired outcome, map the opportunities we've
identified, and generate possible solutions for each. Flag which solutions
we can validate cheaply.
```

Output: Structured opportunity tree with recommended next steps and validation approaches.

**Day 5: Validate or Commit**

Based on the evidence, you make the call: build, validate further, or kill.

If you're confident: move directly to spec writing (Claude generates the PRD from your discovery artifacts).

If you need more evidence: design a lightweight validation (experiment brief, prototype test, concierge MVP) using the templates in [TEMPLATES.md](TEMPLATES.md).

### What Changed

The traditional 3-4 week discovery sprint spent most of its time on synthesis, documentation, and alignment. AI compresses the synthesis and documentation to hours. The human work — user conversations, judgment calls, stakeholder alignment — takes the same amount of time it always did. You just spend a higher percentage of your time on it.

---

## Problem & Opportunity Frameworks

### Jobs-to-be-Done (JTBD)

People don't buy products — they hire them to make progress in their lives. JTBD helps you understand the underlying motivation, not just the surface request.

**When to use:** Exploring a new market, redesigning a core flow, understanding why users churn or adopt.

**AI-native approach:**

```
Here are 5 user interview transcripts about [context]. Analyze them through
a Jobs-to-be-Done lens:
- What functional jobs are users trying to accomplish?
- What social jobs matter (how they want to be perceived)?
- What emotional jobs are at play (how they want to feel)?
- What are the current workarounds they're using?
- Where do existing solutions fall short?
```

Claude identifies the job patterns across interviews. You validate whether the patterns ring true based on your direct user knowledge.

**Key insight for AI-native PM:** JTBD is about the *why* behind behavior — something AI can help you analyze at scale but cannot originate. The interviews are yours. The synthesis is Claude's. The interpretation is yours again.

### Customer Journey Mapping

Map the full experience a user has with your product across stages — from awareness through advocacy — to identify gaps, friction, and opportunities.

**When to use:** Onboarding optimization, cross-functional alignment, identifying where users drop off and why.

**AI-native approach:**

```
Based on these data sources [analytics, support tickets, user feedback],
map the customer journey for [persona] doing [task]. For each stage include:
- What the user is doing
- What they're thinking and feeling
- Touchpoints (product, email, support, etc.)
- Pain points and friction
- Opportunities for improvement
Rate confidence for each stage: high (data-backed), medium (inferred), low (assumed).
```

Claude generates the map structure from your data. You fill the gaps from your direct user knowledge and identify which pain points are worth solving.

### Opportunity Solution Tree (Teresa Torres)

A visual framework for connecting desired outcomes to opportunities to solutions — preventing the common trap of jumping from a vague goal to a specific feature.

**When to use:** Multiple possible problems, need to narrow focus based on evidence, want to keep solution options open while converging on the right opportunity.

**AI-native approach:**

```
Desired outcome: [measurable outcome — e.g., "increase activation from 40% to 60%"]

Based on our research [summary], build an opportunity solution tree:
1. What opportunities (user pain points) could we address to achieve this outcome?
2. For each opportunity, what are 2-3 possible solutions?
3. For each solution, what's the simplest experiment that would validate it?

Rank opportunities by evidence strength and potential impact.
```

Claude builds the tree and ranks options. You decide which branch to pursue based on strategic context, team capacity, and your confidence in the evidence.

### Positioning Statement

Articulate who your product is for, what category it competes in, and why it's different — in a single structured statement.

**When to use:** New product launch, repositioning, entering a new segment, onboarding a new team member who needs to understand "what is this and who is it for."

**Format (Geoffrey Moore):**

```
For [target user] who [need/opportunity], [product name] is a [category]
that [key benefit]. Unlike [alternative], our product [primary differentiator].
```

**AI-native approach:**

```
Here's our product context: [what it does, who uses it, competitive landscape].
Draft 3 positioning statement variants using the Geoffrey Moore format.
For each, explain what trade-off it makes (who it excludes, what it de-emphasizes).
```

Claude generates variants. You pick the one that matches your strategy and stress-test it: does this positioning hold up with real users? Would sales and marketing be able to use it?

---

## Prioritization Frameworks

Prioritization frameworks are where AI-native PM gets an immediate speed advantage. Claude runs the mechanical scoring; you provide the inputs and override when strategic context says the math is wrong.

### RICE (Reach, Impact, Confidence, Effort)

**When to use:** You have quantitative data on reach and can estimate impact. Good for backlog ranking when you need to justify decisions with numbers.

```
Here's my backlog with my estimates for each item:
[Items with your Reach, Impact, Confidence, and Effort ratings]

Run RICE scoring. For any item where the score seems counterintuitive, flag it
and explain why. I may override based on strategic context.
```

| Factor | Definition | Your Job | Claude's Job |
|---|---|---|---|
| Reach | Users affected per time period | Provide the data or estimate | Calculate and normalize |
| Impact | How much it moves the target metric (0.25–3x) | Rate based on user knowledge | Apply consistently |
| Confidence | How sure you are (100/80/50%) | Honest self-assessment | Challenge low-confidence items |
| Effort | Person-weeks to ship | Validate with engineering | Structure the calculation |

### ICE (Impact, Confidence, Ease)

**When to use:** Faster, less data-intensive than RICE. Good for early-stage prioritization when reach data isn't available.

Same pattern: you provide ratings, Claude runs the math and flags anomalies.

### Kano Model

**When to use:** Understanding whether a feature is a basic expectation, a performance differentiator, or a delighter — which determines how much to invest in it.

| Category | Description | Investment Implication |
|---|---|---|
| Must-be | Users expect it; absence causes dissatisfaction, presence doesn't delight | Do it, but don't over-invest |
| Performance | More is better; directly correlated with satisfaction | Invest proportionally to impact |
| Attractive | Unexpected delight; absence doesn't cause dissatisfaction | High-leverage bets when confidence is high |
| Indifferent | Users don't care either way | Don't build it |
| Reverse | Some users actively dislike it | Investigate before building |

```
For these features [list], help me classify them using the Kano model.
For each, I'll describe the user reaction to having it and not having it.
Flag any that might be classified differently for different user segments.
```

### Cost of Delay

**When to use:** Sequencing decisions where timing is the key variable — not just "what should we build" but "what should we build *first*."

```
For these initiatives [list], help me estimate cost of delay:
- What revenue, retention, or strategic value is lost per week of delay?
- Are there time-sensitive windows (seasonal, competitive, contractual)?
- What's the CD3 score (Cost of Delay ÷ Duration) for each?

I'll provide the business context; you structure the analysis.
```

**Key insight for AI-native PM:** Prioritization frameworks are not decisions — they're inputs to decisions. Claude can run every framework in minutes. Your job is choosing the right framework for the situation and overriding the score when you know something the formula doesn't.

---

## Story Splitting

Large stories slow teams down. In AI-native development, well-split stories are especially important because AI coding tools produce better results from focused, well-scoped work. A story that takes a sprint is too big for a human *and* too big for an AI coding tool to implement cleanly.

### The Splitting Principle

Every slice must be:
- **Independently shippable** — delivers user value on its own
- **Testable** — has clear acceptance criteria
- **Small enough** — completable in 1-3 days by an engineer (with or without AI tools)

### Splitting Patterns

When a story is too large, apply these patterns in order of preference:

**1. Split by workflow step**
A story that covers a full workflow can be split into individual steps.

*Before:* "As a user, I can complete the onboarding process."
*After:*
- "As a user, I can create an account with email and password."
- "As a user, I can set my preferences during onboarding."
- "As a user, I can import data from an existing account."

**2. Split by business rule**
A story with multiple business rules or validation logic can be split by rule.

*Before:* "As a user, I can submit a valid order."
*After:*
- "As a user, I can submit an order with required fields validated."
- "As a user, I see an error when my payment method is declined."
- "As a user, I see inventory warnings when items are low stock."

**3. Split by data variation**
A story that handles multiple data types or input formats.

*Before:* "As a user, I can import my data."
*After:*
- "As a user, I can import data from a CSV file."
- "As a user, I can import data from the API."
- "As a user, I can import data via manual entry."

**4. Split by user segment**
A story that serves different user types with different needs.

*Before:* "As a user, I can view my dashboard."
*After:*
- "As a free user, I see basic usage metrics on my dashboard."
- "As a paid user, I see detailed analytics on my dashboard."
- "As an admin, I see team-wide metrics on my dashboard."

**5. Split by happy path vs. edge cases**
Ship the happy path first, handle edge cases in follow-up stories.

*Before:* "As a user, I can update my profile."
*After:*
- "As a user, I can update my display name and bio."
- "As a user, I see validation errors for invalid inputs."
- "As a user, I can revert my profile to previous values."

**6. Split by operation (CRUD)**
A story covering create, read, update, and delete can be split by operation.

**7. Split by platform**
A story spanning multiple platforms (web, mobile, API) can be split by platform.

**8. Split by performance constraint**
Ship the functional version first, optimize performance separately.

*Before:* "As a user, I can search across all my data instantly."
*After:*
- "As a user, I can search my data (basic implementation)."
- "As a user, search results return within 200ms for datasets up to 100k records."

### AI-Native Story Splitting

```
Here's a large user story: [story].
Split it using the most appropriate pattern. For each slice:
- Write the story in standard format
- Include testable acceptance criteria
- Estimate relative size (S/M/L)
- Flag dependencies between slices
- Identify which slice should ship first to deliver value earliest

Keep each slice small enough for an engineer to complete in 1-3 days.
```

Claude generates the split. You validate that each slice is independently valuable (not just a technical layer) and that the sequencing makes sense for your users.

---

## Financial & SaaS Metrics

Product decisions ultimately tie to business outcomes. You don't need to be a finance expert, but you need to speak the language well enough to connect product work to business impact — especially in executive conversations and investment cases.

### Revenue Metrics

| Metric | What It Measures | Why You Care |
|---|---|---|
| **MRR** (Monthly Recurring Revenue) | Predictable monthly revenue | Baseline for all growth math |
| **ARR** (Annual Recurring Revenue) | MRR × 12 | How investors and executives think about scale |
| **Net New MRR** | New + Expansion - Contraction - Churn MRR | Whether you're actually growing |
| **Expansion MRR** | Revenue growth from existing customers | Product-led growth signal — your features drive upsells |
| **ARPU** (Avg Revenue Per User) | Revenue ÷ Users | Segment health; trending up means higher-value usage |

### Retention & Churn Metrics

| Metric | What It Measures | Why You Care |
|---|---|---|
| **Logo Churn** | % of customers lost per period | Are users leaving? |
| **Revenue Churn** | % of MRR lost per period | Are you losing high-value or low-value customers? |
| **Net Revenue Retention (NRR)** | (Starting MRR + Expansion - Contraction - Churn) ÷ Starting MRR | >100% means you grow even without new customers. Best single metric for product health. |
| **DAU/MAU Ratio** | Daily actives ÷ Monthly actives | Engagement depth — are users coming back? |

**NRR benchmarks:**
- Below 90%: Serious retention problem
- 90-100%: Stable but not growing from existing base
- 100-120%: Healthy expansion — product is sticky and users upgrade
- Above 120%: Exceptional — common in best-in-class B2B SaaS

### Growth Efficiency Metrics

| Metric | What It Measures | Why You Care |
|---|---|---|
| **CAC** (Customer Acquisition Cost) | Total sales/marketing spend ÷ new customers | How expensive is growth? |
| **LTV** (Lifetime Value) | ARPU × Gross Margin × (1 ÷ Churn Rate) | How much a customer is worth over their lifetime |
| **LTV:CAC Ratio** | LTV ÷ CAC | Unit economics viability. Below 3:1 is a warning. |
| **CAC Payback** | CAC ÷ (ARPU × Gross Margin) | Months to recoup acquisition cost. Under 12 is healthy. |
| **Rule of 40** | Revenue Growth % + Profit Margin % ≥ 40 | Executive benchmark for balancing growth and profitability |

### Connecting Product Work to Business Metrics

This is where PMs earn their seat at the table. Every feature, initiative, or experiment should connect to one of these metrics:

```
For this initiative [description], help me build the business case:
- Which revenue or retention metric does this primarily affect?
- What's the estimated impact (quantified)?
- What's the confidence level on that estimate?
- What's the cost to build (effort × team cost)?
- What's the expected payback period?

Frame it as an executive-ready investment case.
```

### AI-Native Application

Don't manually calculate these metrics or build spreadsheets from scratch. Feed Claude your data:

```
Here's our monthly revenue data for the last 12 months: [data].
Calculate MRR, MRR growth rate, net new MRR breakdown (new, expansion,
contraction, churn), NRR, and logo churn. Flag any concerning trends
and compare against SaaS benchmarks for our stage ([stage/ARR range]).
```

Claude runs the math and benchmarking. You interpret the results in the context of your product strategy, competitive position, and what you know about upcoming changes.

**Key insight for AI-native PM:** Financial fluency is how you justify continued investment in product development — including investment in AI-native workflows. If you can't connect your team's AI-accelerated velocity to business outcomes, the investment case weakens. Every framework in this document ultimately serves one purpose: making better product decisions faster, and proving it with numbers.
