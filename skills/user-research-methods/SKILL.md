---
name: user-research-methods
description: Plan and execute user research — interviews, surveys, usability tests. Use when you need primary evidence to inform a product decision.
---

# User Research Methods

Plan, execute, and synthesize user research in 1-3 days. Claude handles protocol design, guide generation, survey drafting, and findings synthesis. You handle the user conversations, observation, and interpretation.

## When to Use

- You need primary evidence before committing to a direction
- Existing data (analytics, support tickets) doesn't explain the "why"
- You're designing for a user segment you don't deeply understand
- A feature launched and adoption is lower than expected — you need to understand why
- You're validating a prototype or concept before engineering investment

## When NOT to Use

- You have enough evidence to decide — don't research to delay a decision
- You need to analyze quantitative data you already have — use Growth & Retention Diagnostics
- You're running a statistical experiment — use the Experiment Brief template

## The AI-Native Approach

**Traditional research:** 2-4 weeks for research planning, recruitment, execution, synthesis, and presentation.

**AI-native research:** 1-3 days. Claude compresses planning and synthesis to hours. The user conversations — the actual research — take the same time they always did.

| Step | Time | Claude Does | You Do |
|---|---|---|---|
| Choose method | 15 min | Recommend method based on your question | Validate fit for your context |
| Design protocol | 1-2 hrs | Generate guides, scripts, or surveys | Customize with your domain knowledge |
| Execute | Half day - 1 day | (Not present for conversations) | Conduct interviews, run tests, deploy survey |
| Synthesize | 1-2 hrs | Identify themes, patterns, contradictions | Validate interpretation, add context |
| Present findings | 30 min | Structure findings for stakeholder consumption | Add implications and recommendations |

## Process

### Step 1: Choose the Right Method (15 minutes)

```
I need to answer this question: [your research question].

Context:
- Decision this informs: [what you'll do with the findings]
- Timeline: [when you need the answer]
- Access to users: [how you can reach them — existing users, prospects, internal]
- What you already know: [existing data or hypotheses]

Recommend the right research method and explain why.
```

**Method selection guide:**

| Method | Best For | Sample Size | Time |
|---|---|---|---|
| User interviews | Understanding motivations, pain points, workflows | 5-8 users | 1-2 days |
| Usability testing | Evaluating whether users can complete tasks in your product or prototype | 5 users | 1 day |
| Surveys | Quantifying preferences, satisfaction, or behavior across a population | 50-200+ responses | 1-2 days |
| Concept testing | Validating an idea before building it | 5-8 users | 1 day |
| Card sorting | Informing information architecture or navigation | 10-20 users | 1 day |
| Diary studies | Understanding behavior over time | 5-10 users | 1-2 weeks (exception to our speed principle — some things need time) |

### Step 2: Design the Research Protocol (1-2 hours)

**For interviews:**

```
Generate a discussion guide for [N] 30-minute interviews about [topic].

Requirements:
- Start with warm-up questions to build rapport (2 minutes)
- Focus on past behavior, not hypotheticals ("tell me about the last time..." not "would you...")
- Include one open-ended question that might surface something unexpected
- Probe for specific examples, not generalizations
- End with "what should I have asked that I didn't?"
- Flag questions that might lead the participant
- Keep it to 10-12 questions max

Apply Mom Test principles: no pitching, no hypotheticals, focus on their life, not your idea.
```

**For usability tests:**

```
Generate a usability test script for [feature/prototype].

Include:
- Pre-test briefing (remind them: we're testing the product, not them)
- 4-6 task scenarios written as goals, not instructions
  (e.g., "You want to change your notification settings" not "Click Settings, then Notifications")
- Follow-up probes for each task (what did they expect? what was confusing?)
- Post-test questions about overall impression
- Note: think-aloud protocol instructions
```

**For surveys:**

```
Design a survey to [research objective].

Requirements:
- 10-15 questions max (completion rate drops after 15)
- Mix of: Likert scale, multiple choice, and 1-2 open-ended
- No double-barreled questions (asking two things at once)
- No leading questions
- Logical flow: broad → specific → demographic
- Include a screening question if needed for targeting
- Estimated completion time: under 5 minutes
```

### Step 3: Execute the Research

This is the human step. Some guidance:

**For interviews:** Take notes on what they said, not what you think they meant. Record (with permission) so Claude can help with synthesis. Ask "why?" at least three times. The first answer is surface-level.

**For usability tests:** Watch, don't help. Note where they hesitate, where they backtrack, where they express frustration or surprise. The struggle IS the data.

**For surveys:** Deploy to your target audience. Monitor early responses for confusion or drop-off patterns.

### Step 4: Synthesize Findings (1-2 hours)

```
Here are my research notes/transcripts from [N] [interviews/tests/survey results]:

[Paste notes, transcripts, or data]

Synthesize:
1. Key themes (what came up repeatedly)
2. Frequency (how many participants raised each theme)
3. Contradictions (where participants disagreed)
4. Surprises (findings that challenge our assumptions)
5. Strongest quotes (verbatims worth preserving)
6. Confidence rating for each finding: strong (consistent across participants),
   moderate (present but not universal), weak (one-off or ambiguous)
```

Review Claude's synthesis against your memory of the conversations. Did the synthesis miss the energy behind a comment? Did it over-weight an articulate participant? Add your interpretive layer.

### Step 5: Present Findings (30 minutes)

```
Structure our research findings for [audience — team, leadership, design]:

Format:
1. Research question and method (one paragraph)
2. Key findings (3-5 findings with evidence strength ratings)
3. Implications for [the decision this was meant to inform]
4. Recommended next steps
5. Appendix: participant details, methodology notes, raw quotes

Keep findings factual. Separate what participants said from what we interpret.
```

## Output

- Research protocol (discussion guide, test script, or survey)
- Raw notes or transcripts (your input)
- Synthesized findings with themes, frequency, and confidence ratings
- Stakeholder-ready findings presentation
- Recommended next steps

## Common Pitfalls

1. **Asking hypothetical questions.** "Would you use this?" always gets yes. Ask about past behavior instead: "Tell me about the last time you tried to solve this problem."
2. **Small sample ≠ statistical significance.** 5-8 interviews reveal themes, not percentages. Don't say "80% of users want X" from 5 interviews. Say "a consistent theme across interviews was X."
3. **Confirmation bias in synthesis.** You'll naturally notice findings that confirm your hypothesis. Force yourself to document contradictory evidence first.
4. **Research without a decision.** If you can't articulate what you'll do differently based on the findings, you don't need the research yet.
5. **Over-polishing the protocol.** A good-enough discussion guide used tomorrow beats a perfect one used next week. Iterate after the first session.

## Related Skills

- [Discovery Process](../discovery-process/SKILL.md) — research as part of a structured discovery cycle
- [Growth & Retention Diagnostics](../growth-retention-diagnostics/SKILL.md) — when you need qualitative context for quantitative trends
- Reference: [FRAMEWORKS.md](../../FRAMEWORKS.md) — Jobs-to-be-Done, Customer Journey Mapping
