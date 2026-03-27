# explore

A Claude Code skill for conversational technical design discussions.

Breadth-first exploration — surfaces options before diving deep. One sub-topic per turn. Think: senior engineer pair session, not a wall of text.

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
