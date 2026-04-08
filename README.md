# explore

A Claude Code skill that fixes Plan Mode's decision problem.
Plan Mode is execution-focused — it buries design decisions inside walls of implementation detail. You end up rubber-stamping choices you never consciously made.
/explore sits before Plan Mode. It surfaces every decision point, discusses them with you breadth-first, and records your choices. By the time you generate a plan, every architectural call is yours.

## What it does

When you invoke `/explore`, the skill:

1. **Recon** — scans the relevant parts of your codebase
2. **Opens with the big picture** — problem statement, decision areas, suggested starting point
3. **Walks through decisions one at a time** — surfaces all viable options, presents tradeoffs, lets you decide
4. **Maintains a decision log** — writes settled choices, open questions, and scope to `explore-context.jsonl` so context survives into plan/code mode

## Install

```bash
npx skills add https://github.com/lot-agent/explore --skill explore
```

## Usage

In Claude Code, type:

```
/explore
```

Then describe the topic you want to think through — architecture decisions, API design, migration strategy, etc.

## License

MIT
