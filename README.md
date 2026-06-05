# Idea Funnel

`idea-funnel` is a Codex skill for evidence-grounded research idea exploration.
It is designed for situations where a vague direction, a failed attempt, review
feedback, or a set of prior work needs to be turned into a defensible next idea.

The central pattern is a **motivation funnel**:

1. Start from a broader research need.
2. Group real prior work into meaningful categories.
3. Explain the progression across those categories.
4. Identify either a shared unresolved issue or a narrower problem at the
   frontier of the progression.
5. Connect the proposed idea directly to that opening.
6. Define the smallest validation that could support or weaken the motivation.

## Why This Skill Exists

Research idea exploration can drift into speculative novelty, oversized plans,
or narrative repair after negative evidence. This skill keeps the process
decision-oriented:

- verify important facts instead of inventing prior work;
- distinguish "possible to do" from "worth doing";
- treat negative evidence as a reason to revise or pivot;
- look for a small method hook beyond engineering assembly when forming ideas;
- run small falsifiable checks before scaling engineering or writing;
- keep optional additions separate from claim-critical work.

## When To Use

Use this skill when you want to:

- find a new research idea from an initial direction;
- evaluate whether an idea is novel, feasible, and worth pursuing;
- extract future work from existing work;
- rebuild after a failed motivation check or negative result;
- turn related work into a persuasive motivation chain;
- design a quick Go / Weak / No-Go validation.

## Default Output

The skill defaults to a compact memo:

```markdown
## Bottom Line
## Evidence and Motivation Funnel
## Candidate Ideas
## Recommended Direction
## Minimal Validation
## Decision Criteria and Next Step
```

It can expand into a full related-work landscape, method plan, independent
review, versioned exploration log, or proposal-style memo when the project
requires it.

## Installation

Recommended installation through the skills CLI:

```bash
npx skills add slpanir/idea-funnel -g --skill idea-funnel
```

The same source can also be written as a GitHub URL:

```bash
npx skills add https://github.com/slpanir/idea-funnel -g --skill idea-funnel
```

The `-g` flag installs the skill globally. Omit it if you intentionally want a
project-local installation.

Manual installation is also possible by cloning this repository into your global
skills directory:

```bash
git clone git@github.com:slpanir/idea-funnel.git ~/.agents/skills/idea-funnel
```

If the directory already exists, update it with:

```bash
cd ~/.agents/skills/idea-funnel
git pull
```

## Files

- [`SKILL.md`](./SKILL.md): the skill definition loaded by Codex when triggered.

## Usage Examples

```text
Use idea-funnel to explore a new research idea from these related papers.
```

```text
This idea failed its initial experiment. Use idea-funnel to decide whether to
repair, narrow, or abandon it.
```

```text
Use idea-funnel to build a motivation chain from prior work and propose a small
validation before we commit to implementation.
```
