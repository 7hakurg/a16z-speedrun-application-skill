# a16z Speedrun Application — Claude Skill

A [Claude Code / Claude](https://docs.claude.com/en/docs/claude-code/skills) skill that helps founders build, pressure-test and polish an **a16z Speedrun** application.

It acts as a direct early-stage startup coach. It asks only the questions it needs, drafts specific answers, scores your application against a Speedrun-style rubric, and tells you plainly where it is weak.

> Not affiliated with, endorsed by, or connected to Andreessen Horowitz (a16z). It never submits anything for you: you review and submit your application yourself.

## What it does

- Asks targeted intake questions in small batches: your unfair advantage, the customer and problem, the first wedge, proof and traction, distribution.
- Drafts a one-liner, "why now", "why you" and "why this wedge".
- Scores 8 categories from 1 to 10 (earned insight, customer specificity, wedge clarity, speed signal, distribution, market timing, business potential, founder-market fit) and proposes the fastest fix for anything below 6.
- Refuses to invent traction, metrics, users, revenue or credentials. Unknowns are marked `[NEEDS INPUT]`.
- Produces six files: `one_liner.md`, `application_answers.md`, `founder_story.md`, `wedge_and_roadmap.md`, `proof_plan.md`, `interview_prep.md`.
- Ends with a candid assessment, a 7-day plan to fix the weakest part, and five interview questions to practise.

## Install

### Claude Code

```bash
git clone https://github.com/7hakurg/a16z-speedrun-application-skill.git
mkdir -p ~/.claude/skills
cp -r a16z-speedrun-application-skill/a16z-speedrun-application ~/.claude/skills/
```

Restart Claude Code. The skill loads when you ask something like "help me apply to a16z Speedrun".

For one project only, copy the folder to `<your-project>/.claude/skills/` instead.

### Claude.ai

Zip the `a16z-speedrun-application` folder and upload it under **Settings → Capabilities → Skills**.

## Use

```
Help me apply to a16z Speedrun. My startup is <one sentence>.
```

Answer its questions, then review the drafts in `application_answers.md` and the rest.

## License

MIT — see [LICENSE](LICENSE).
