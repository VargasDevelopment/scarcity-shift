# Scarcity Shift

**Democratizing production does not democratize demand.**

AI made code, content, and digital products cheap. So "I can build it" stopped being an advantage. Value moved to what is still scarce: distribution, trust, accountability, proprietary data, relationships, and physical or regulated access.

Scarcity Shift is an agent skill for Claude Code and Codex. It judges an idea against that reality, for *your* situation, and gives you a straight answer.

```
SCARCITY SHIFT VERDICT
Idea: AI-generated budget planners, 300 Etsy listings in month one
Classification: Kill / Archive
Verdict: Kill or archive (as framed)
Scarce asset: none yet
Smallest honest test: make 1–3 products for a group you can reach, and ask 10 of them if they'd pay
```

Each verdict comes with a 16-part analysis: steelman, red team, distribution route, a test of what happens when AI gets 10× better, the economics, the smallest honest test, and explicit stop conditions.

It doesn't treat every idea as a startup. A project can be good art, a useful personal tool, or a worthwhile experiment, and the skill will say so while rejecting it as a business.

## Install

```sh
npx skills@latest add VargasDevelopment/scarcity-shift
```

That one command installs the skill for Claude Code, Codex, and other agents that read `SKILL.md`. Pick your agents when prompted.

**As a plugin**, if you want updates through your agent's plugin system:

```sh
# Claude Code
claude plugin marketplace add VargasDevelopment/scarcity-shift
claude plugin install scarcity-shift@scarcity-shift

# Codex
codex plugin marketplace add VargasDevelopment/scarcity-shift
codex plugin add scarcity-shift@scarcity-shift
```

## Use

```
/scarcity-shift I want to sell AI-generated coloring books on Etsy
```

In Codex, use `$scarcity-shift` instead of `/scarcity-shift`. Both agents also pick up the skill on their own when you ask whether an idea is worth pursuing.

**First run:** the skill asks eight quick questions about your constraints and assets, such as time, money, employer overlap, how public you're willing to be, and what you already have. Answer briefly or skip any of them. It saves the answers to `~/.config/scarcity-shift/profile.md`, so later runs need no setup. The profile stays on your machine. Run `/scarcity-shift setup` to update it.

Prefer not to set up? Put your situation in the message, or reply "skip".

## The framework

The full framework is in [`skills/scarcity-shift/references/framework.md`](skills/scarcity-shift/references/framework.md): the four scarcity questions, nine classifications, eight evaluation gates, and the list of things not to confuse. ("Shelf space is not demand. Publishing is not distribution. An algorithm is not a demand strategy.")

[`examples.md`](skills/scarcity-shift/references/examples.md) has worked evaluations, including the author's own failed product launch.

## Evals

The [`evals/`](evals) folder holds test cases with graded expectations: killing a commodity idea, keeping a hobby a hobby, vaulting an employer-adjacent idea, backing an idea built on real relationships, and first-run setup. To run them with Claude Code:

```sh
claude plugin eval . --allow-tools Write,Bash
```

These are real, billed model runs.

## License

MIT. By [Joseph Vargas](https://blog.josephvargas.dev).
