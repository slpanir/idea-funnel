---
name: idea-funnel
description: Use when the user wants to explore, repair, evaluate, or restart a research idea from a vague direction, prior work, failed result, review feedback, or initial hypothesis. Trigger for finding research ideas, judging whether an idea is worth pursuing, extracting future work from existing work, rebuilding after negative evidence, constructing a motivation chain, or designing a quick motivation check.
---

# Idea Funnel

Use this skill to help the user decide what research idea is worth pursuing next. The core pattern is a motivation funnel: ground in real evidence, organize prior work into a progression, identify either a shared unresolved issue or a specific weakness at the frontier of that progression, then define the smallest useful validation before recommending further work.

## Core Rules

- Do not invent prior work, citations, results, datasets, systems, or consensus. Verify them when needed; if uncertain, mark them as uncertain.
- Do not preserve an old idea by forcing positive interpretations of negative evidence.
- Treat "possible to do" as weaker than "worth doing". A strong idea needs a motivated problem, a non-obvious contribution, and feasible validation.
- Do not expand engineering, writing, or data collection before the key motivation is tested.
- Prefer small falsifiable checks before large plans.
- Keep the main line lean. Add complexity only when it directly strengthens the claim or removes a likely objection.

## Motivation Funnel

Use this as the default thinking pattern when the user wants a persuasive research narrative or a grounded new idea:

1. Start from the broader problem or need.
2. Group prior work by meaningful categories such as problem, method, assumption, setting, or evidence.
3. Explain the progression across categories: what each step solves, what it assumes, and what becomes newly visible.
4. Identify the opening: either a shared unresolved limitation across categories, or a narrower problem that emerges in the most advanced or most relevant category.
5. Connect the proposed idea directly to that opening instead of merely adding another variant.
6. Name the smallest observation or validation that would support or weaken this motivation.

The funnel must be earned from the evidence. If the grouping does not naturally imply the opening, revise the framing instead of forcing the narrative.

## Workflow

1. Clarify the starting point.
   Identify whether the user wants a new idea, a repair of an existing idea, an evaluation of feasibility/novelty, or a stop/pivot decision. Note available evidence or materials, and list assumptions already weakened by prior results.

2. Ground in real prior work or evidence.
   Inspect provided materials and search external sources when the answer depends on current or specific prior work. State what is confirmed, uncertain, and missing; when useful, organize the evidence into a Motivation Funnel.

3. Find the real research gap.
   Use the evidence snapshot, and the Motivation Funnel when applicable, to identify a concrete unresolved problem, weak assumption, missing condition, measurement flaw, implementation barrier, under-tested setting, or frontier-method limitation. Reject gaps that are only invented to justify novelty. Explain why the gap matters if it is real.

4. Generate candidate ideas.
   Propose 2-4 candidates. For each, give: one-sentence idea, target problem, difference from prior work, why it might matter, key uncertainty, and minimal validation.

5. Decide the next action.
   Recommend one path and define a Go / Weak / No-Go decision frame:
   - Go: evidence supports motivation and the minimal validation looks feasible.
   - Weak: narrow the claim, repair a specific issue, or run one more focused check.
   - No-Go: stop or pivot, with the failed assumption stated explicitly.

## Default Output

Use a concise structure unless the user asks for a full memo:

```markdown
## Bottom Line
## Evidence and Motivation Funnel
## Candidate Ideas
## Recommended Direction
## Minimal Validation
## Decision Criteria and Next Step
```

## Optional Expansions

Use only when requested or when project complexity requires it:

- full related-work landscape;
- detailed method or experiment plan;
- independent review or subagent critique;
- versioned exploration log with rejected assumptions and No-Go reasons;
- paper narrative, proposal memo, or presentation-ready summary.

## Practical Guidance

- If one fact is central and uncertain, verify it before building the idea around it.
- If evidence cannot be verified within the current task, say so explicitly and separate verified facts from assumptions.
- If prior results contradict the idea, start by explaining the contradiction rather than repairing the narrative.
- If review feedback asks for many additions, separate claim-critical fixes from optional extensions.
- If the idea depends on a resource, first check whether the resource exists and supports the required variables.
- If the user wants action, make the smallest validation plan concrete enough to run next.
