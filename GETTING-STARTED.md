# Getting Started

A practical guide for product managers using Claude Code for the first time. By the end of this walkthrough, you'll have produced your first real artifact and understand the working pattern you'll use daily.

## Prerequisites

- Claude Code installed ([installation guide](https://docs.anthropic.com/en/docs/claude-code/overview))
- The `CLAUDE.md` file from this repo copied into your project directory
- A real product problem you're currently working on (not a hypothetical — you'll get more value from a real artifact)

## First Session: From Problem to PRD (15 Minutes)

### Step 1: Set Your Profile (1 minute)

Start a Claude Code session and introduce yourself:

```
I'm a [junior/mid/senior/executive] product manager working on [product type].
I'm a [solo PM / PM on a squad / PM leading multiple squads].
Right now I'm focused on [discovery/definition/delivery/launch/growth/maintenance].
```

Claude calibrates its depth and approach based on this. Be honest about your experience level — junior PMs get more framework context, senior PMs get faster output.

### Step 2: State the Problem (2 minutes)

Don't start with a feature. Start with the problem:

```
Here's a problem I'm working on:

[Who] is experiencing [what problem].
We know this because [evidence — support tickets, survey data, metrics, user interviews].
If we don't address this, [business impact].
```

If you don't have evidence yet, say so. Claude will help you figure out what to gather before committing to a solution.

### Step 3: Explore Before Committing (3 minutes)

Ask Claude to help you think before jumping to solutions:

```
Before we define a solution, help me think through this:
- What are the possible approaches?
- What assumptions are we making?
- What do we need to validate before investing engineering time?
```

Review Claude's output. This is where you apply judgment — Claude generates options, you evaluate them based on your knowledge of users, strategy, and constraints.

### Step 4: Generate the Artifact (5 minutes)

Once you've aligned on an approach:

```
Write a PRD for [the approach you chose]. Include:
- Problem statement and evidence
- Success metrics with specific targets
- Scope (what's in v1, what's deferred)
- User stories with testable acceptance criteria
- Edge cases and error states
- Technical constraints and dependencies
```

### Step 5: Review and Refine (4 minutes)

Read the output critically. Ask yourself:

- **Problem:** Is the problem statement accurate to what I know? Would a new team member understand the "why"?
- **Metrics:** Can we actually measure these? Do we have the instrumentation?
- **Scope:** Is this the smallest thing that tests the hypothesis, or has Claude over-scoped?
- **Acceptance criteria:** Could an engineer start work from these today?
- **Edge cases:** Did Claude catch anything I missed? Did it add any that don't apply?

Tell Claude what to fix. Be specific:

```
The success metric for adoption is too aggressive — change from 40% to 25% based on our
historical adoption rates for settings pages. Also, remove the admin notification template
from v1 scope — that's a separate initiative.
```

### What You Just Did

You followed the core pattern:

1. **You** provided the problem, context, and judgment
2. **Claude** generated the structure, detail, and thoroughness
3. **You** reviewed and refined with your domain knowledge

This is the working pattern for everything — research synthesis, roadmap planning, stakeholder updates, experiment design. Claude handles the first 80% (structure, boilerplate, edge cases). You handle the last 20% (judgment, context, decisions).

---

## Adapting to Your Organization's Tools

Every organization has required systems — Confluence, SharePoint, Notion, Workvivo, Google Docs, Jira, or others. Claude Code generates artifacts in markdown, which means you'll need a workflow for getting content into your org's systems.

### The Generation-to-Deployment Pattern

```
1. Generate  →  Claude produces the artifact in markdown
2. Review    →  You apply judgment, context, and corrections
3. Adapt     →  Format for your target system (Confluence page, Jira tickets, Slides deck)
4. Validate  →  Confirm accuracy, check links, verify data points
5. Deploy    →  Publish to the organizational system
```

### Practical Approaches

**For documentation platforms (Confluence, SharePoint, Notion):**

```
Format this PRD for Confluence. Use Confluence-compatible markdown with:
- A table of contents at the top
- Status macro placeholder (Draft/In Review/Approved)
- Jira ticket links formatted as [PROJ-123] placeholders
- Section structure that matches our team's standard template
```

**For project management tools (Jira, Linear, Asana):**

```
Break this PRD into Jira-ready tickets. For each ticket include:
- Summary (under 80 characters)
- Description with acceptance criteria
- Story points estimate (use fibonacci)
- Labels: [feature area]
- Dependencies on other tickets
```

**For presentations (Google Slides, PowerPoint):**

```
Convert this stakeholder update into a 5-slide executive summary:
- Slide 1: Headline and key metric
- Slide 2: Progress against milestones
- Slide 3: Risks and mitigations
- Slide 4: What we need from leadership
- Slide 5: Next 30-day plan
Structure as speaker notes and bullet points I can drop into slides.
```

### Guardrails for Organizational Deployment

Before publishing any AI-generated artifact to an organizational system:

1. **Verify all data points.** Claude may generate plausible-sounding numbers. Every metric, date, percentage, and claim needs to trace back to a real source.
2. **Check for confidential information.** Ensure you haven't inadvertently included sensitive data in prompts or outputs that will be stored in organizational systems.
3. **Confirm naming conventions.** Project names, team names, product names, and terminology should match your org's standards, not Claude's best guess.
4. **Review for tone and audience.** An artifact written for engineers reads differently than one for executives. Make sure the format matches the destination.
5. **Add attribution where appropriate.** Your organization may have policies on AI-generated content disclosure. Follow them.

---

## Next Steps

Once you're comfortable with the basic pattern:

- **[TEMPLATES.md](TEMPLATES.md)** — Starter templates for every major PM artifact
- **[AI-NATIVE-WORKFLOW.md](AI-NATIVE-WORKFLOW.md)** — How PM changes when your whole team uses AI tools
- **[EXAMPLES.md](EXAMPLES.md)** — Before/after demonstrations of each core principle
- **[CLAUDE.md](CLAUDE.md)** — The full behavioral guidelines reference
