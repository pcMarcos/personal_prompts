# Software Engineer Prompts

## Code Implementation
```
Act as a principal engineer. Implement [feature]. Before coding:
1. Identify the core challenge/trade-off
2. Show 2-3 approaches with pros/cons
3. Explain why you chose your approach
4. Flag potential pitfalls
```

```
Implement [feature]. For each decision, explain:
- What could go wrong with alternatives
- How this scales (or doesn't)
- What you'd revisit if constraints changed
```

```
Write [function/module] with inline comments on NON-OBVIOUS decisions only. Mark each with "LEARN: [brief explanation]"
```

## Architecture & Design
```
Design the architecture for [system]. Include:
- Key decisions and the trade-offs that forced them
- What you're deliberately NOT solving and why
- How this breaks at scale and what that would look like
- Alternatives you rejected
```

```
Review this API/data model design. For each decision:
- What assumptions does it make?
- What changes would break it?
- How does it evolve over time?
```

```
Generate 3 architecture options for [problem]. For each:
- Happy path, failure modes, scaling behavior
- Operational complexity
- Team/organization implications
```

## Code Review
```
Review this PR as a senior engineer. For each concern:
- Severity and likelihood
- How it would manifest in production
- Suggested fix with reasoning
- "Ship it" or "Block it" with justification
```

```
Review this code. Focus on:
- What questions does this raise about the broader system?
- What implicit contracts is this assuming?
- What would debugging this look like?
```

## Spikes & POCs
```
Run a spike on [technology/approach]. Deliver:
- 3 concrete findings with evidence
- Clear go/no-go recommendation
- What the production implementation looks like
- Remaining unknowns
```

```
Evaluate [library/framework]. Cover:
- Real-world limitations (not docs)
- Maintenance/author signals
- Migration path out
- Production readiness signals
```

## Documentation
```
Document [system]. Structure as:
- Decisions made (and why alternatives lost)
- Known failure modes
- "It's broken when..." diagnosis guide
- Onboarding path for new engineers
```

```
Write architecture decision record (ADR) for [change]. Format:
- Status, Context, Decision, Consequences
- Rejected alternatives with reasoning
- What would make us revisit this
```

## Refactoring
```
Analyze [codebase section]. Identify:
- The core abstraction (if any)
- What's preventing clean extraction
- Minimum viable refactor vs. ideal state
- Riskiest change
```

```
Refactor [X] to [Y]. Explain:
- What principle motivated this change
- What tests prove correctness
- What could regress
```

## Debugging & Incidents
```
Help debug [issue]. Think like:
- What assumptions are likely wrong?
- What's the simplest explanation?
- What would you instrument to confirm?
```

```
Run a mock postmortem for [incident type]. Include:
- Timeline of likely failure cascade
- What detection missed
- What prevention failed
- Actionable improvements (not generic)
```

## Technical Planning
```
Estimate [feature]. Break down:
- Where complexity lives
- What you don't know yet
- Best/worst case variance
- What enables speed
```

```
Break down [epic/feature] into tasks. For each:
- Primary risk
- Unblock path
- Definition of done (technical, not just checkboxes)
```

## Performance
```
Analyze performance of [code/query/endpoint]. For each bottleneck:
- Why it matters (or doesn't)
- Fix cost vs. gain
- What you're trading off
```

```
Profile this [system]. Identify:
- Where time/memory actually goes
- What scales O(n) vs O(1)
- Whether optimization is worth it
```

## Security
```
Review [feature/endpoint] for security. Cover:
- Attack surface
- Which assumptions are dangerous
- What you'd test
- Defense in depth gaps
```

## Personal Growth
```
I'm stuck on [concept]. Explain it as:
- A real analogy from systems I know
- A common misconception
- What to build to prove understanding
```

```
Teach me [pattern/principle] by:
1. Explaining when it makes sense
2. Showing anti-patterns where it doesn't
3. Identifying when you've over-applied it
```

## Additional Areas to Consider

**On-call & Reliability**
```
Design runbook for [service]. Include:
- What "healthy" looks like (metrics)
- Top 5 failure modes with symptoms
- Escalation criteria
- Common false positives
```

**API Design**
```
Design API for [resource]. For each endpoint:
- What consistency guarantees does this offer?
- How does pagination/filtering compose?
- What does versioning look like?
- What does migration look like?
```

**Testing Strategy**
```
Design test strategy for [feature]. Explain:
- What each test type actually proves
- Where over-testing wastes time
- What can't be tested (and how to mitigate)
- Mutation testing targets
```

**Team Dynamics & Technical Leadership**
```
Help me prepare for [technical discussion]. Focus on:
- What objections are likely?
- What evidence matters?
- How to present trade-offs (not just your view)
- When to yield
```

**Dependency Management**
```
Evaluate adding [dependency]. For each:
- Maintenance velocity and signals
- API surface you're coupling to
- Upgrade/removal path
- License/security implications
```
