---
name: build-vs-buy
description: Evaluate whether to build in-house, buy a vendor solution, or partner. Use when facing a make-or-buy decision for a capability.
---

# Build vs. Buy Evaluation

Structure a build-vs-buy decision in half a day. Claude runs the comparison framework, models total cost of ownership, and maps the risk profile. You provide the strategic judgment about what's core to your product and what's commodity.

## When to Use

- Evaluating a vendor solution vs. building in-house
- Deciding whether to integrate a third-party service or build your own
- Assessing whether to partner with another company for a capability
- Reviewing an existing vendor relationship (should we bring this in-house?)
- Engineering is proposing to build something that might already exist

## When NOT to Use

- The decision is about pricing an existing product — use Pricing & Packaging
- You're evaluating competitive products for market analysis — use Discovery Process
- The decision is purely technical (language, framework) — defer to engineering

## The AI-Native Approach

| Step | Time | Claude Does | You Do |
|---|---|---|---|
| Define the capability | 30 min | Structure requirements, must-haves vs. nice-to-haves | Validate requirements with stakeholders |
| Evaluate options | 1-2 hrs | Research vendors, model build effort, map partner options | Add context from vendor conversations |
| Model total cost | 1 hr | Calculate TCO for each option over 1-3 years | Validate engineering estimates |
| Assess strategic fit | 30 min | Map options against strategic criteria | Make the core vs. commodity judgment |
| Recommend | 30 min | Draft decision document with recommendation | Present and get sign-off |

## Process

### Step 1: Define the Capability (30 minutes)

```
We need [capability] for [reason]. Help me structure the requirements:

Functional requirements:
- What must it do? (non-negotiable features)
- What should it do? (important but flexible)
- What could it do? (nice-to-haves, future needs)

Non-functional requirements:
- Performance: [latency, throughput, availability]
- Scale: [current and projected usage]
- Security/compliance: [requirements]
- Integration: [what it needs to connect to]
- Customization: [how much do we need to adapt it]

Constraints:
- Timeline: [when do we need this]
- Budget: [available investment]
- Team capacity: [who could build and maintain this]
```

### Step 2: Evaluate Options (1-2 hours)

```
Evaluate three paths for this capability:

BUILD:
- Estimated effort to build (engineering weeks/months)
- What we'd build first (MVP) vs. full version
- Maintenance burden (ongoing engineering time)
- Time to first value
- What we control and can customize

BUY (evaluate 2-3 vendors if applicable):
For each vendor [names]:
- Feature coverage vs. our requirements
- Pricing model and estimated annual cost
- Integration complexity
- Vendor reliability (size, funding, customer base, track record)
- Lock-in risk (data portability, contract terms, switching cost)
- Customization limits

PARTNER:
- Are there companies that offer this as a white-label or co-build?
- What's the partnership structure (revenue share, co-development, licensing)?
- What do we give up (control, margin, data)?
```

### Step 3: Model Total Cost of Ownership (1 hour)

```
Calculate TCO for each option over [1/2/3] years:

BUILD:
- Development cost: [engineering hours × loaded cost]
- Ongoing maintenance: [% of dev time per year]
- Infrastructure cost: [hosting, monitoring, tools]
- Opportunity cost: [what the team can't build while building this]
- Risk cost: [probability of failure × impact]

BUY:
- License/subscription cost: [annual]
- Integration cost: [engineering time to integrate]
- Ongoing integration maintenance: [annual]
- Training and change management: [one-time]
- Switching cost if we leave: [data migration, re-integration]
- Price escalation risk: [vendor raises prices]

PARTNER:
- Revenue share or licensing: [ongoing]
- Integration and co-development: [one-time + ongoing]
- Dependency risk: [partner changes terms, gets acquired, shuts down]

Present as a comparison table with 1-year and 3-year views.
```

### Step 4: Assess Strategic Fit (30 minutes)

This is the judgment call that matters most.

```
Evaluate each option against strategic criteria:

Core vs. commodity:
- Is this capability a competitive differentiator for us?
- Do we need to innovate on this, or do we just need it to work?
- Would our users notice if we built this vs. bought it?

Speed vs. control:
- How urgently do we need this? (Buy is usually faster)
- How much customization do we need? (Build gives more control)
- How likely are requirements to change? (Build adapts faster to our needs)

Risk profile:
- Build risk: can we actually build this well with our team?
- Buy risk: vendor dependency, lock-in, price changes
- Partner risk: alignment of incentives, longevity

Team and culture:
- Does our team have the expertise to build and maintain this?
- Is building this a valuable skill-building opportunity?
- Or would it distract from our core mission?
```

### Step 5: Recommend (30 minutes)

```
Draft a decision document:

1. Capability needed and why
2. Options evaluated (build, buy [vendors], partner)
3. TCO comparison (table)
4. Strategic fit assessment
5. Recommendation and rationale
6. Implementation plan for recommended option
7. Risks and mitigations
8. Decision deadline and review point

If recommending BUY: include vendor selection criteria and next steps (POC, trial, contract negotiation).
If recommending BUILD: include phased build plan and resource request.
If recommending PARTNER: include partnership structure and terms to negotiate.
```

## Output

- Structured requirements (functional, non-functional, constraints)
- Option evaluation (build, buy, partner with specifics)
- TCO comparison table (1-year and 3-year)
- Strategic fit assessment
- Decision document with recommendation

## Common Pitfalls

1. **"We can build it better."** Maybe. But should you? Building commodity infrastructure instead of product differentiation is the most common misallocation of engineering time.
2. **Ignoring maintenance cost.** Building is a one-time cost. Maintaining is forever. Factor in 15-20% of original build cost annually for maintenance.
3. **Vendor lock-in fear.** Some lock-in is acceptable for speed and focus. Evaluate the actual switching cost, not the theoretical risk. If switching cost is manageable, the lock-in concern may be overblown.
4. **Not involving engineering.** Build estimates from PMs are fiction. Engineering needs to evaluate feasibility, estimate effort, and assess maintenance burden.
5. **Decision avoidance via POC.** Proof of concepts are valuable, but "let's do a POC" can be a way to avoid deciding. Set clear POC success criteria and a decision deadline before starting.

## Related Skills

- [Tech Debt Communication](../tech-debt-communication/SKILL.md) — when "buy" replaces a homegrown system with debt
- [Stakeholder Alignment](../stakeholder-alignment/SKILL.md) — when the build-vs-buy decision involves cross-functional trade-offs
- [Pricing & Packaging](../pricing-packaging/SKILL.md) — when the vendor cost affects your product's unit economics
