---
name: scarcity-shift
description: Evaluate a business, side project, product, or startup idea with the Scarcity Shift framework. When AI makes production cheap, value moves to what stays scarce, such as distribution, trust, ownership, data, and access. Returns a classification, a gated analysis, the smallest honest test, and a decisive verdict. Use when someone asks whether an idea is worth pursuing or why a venture isn't getting traction, or invokes /scarcity-shift.
---

# Scarcity Shift

Help the user judge an idea honestly. The core claim: **democratizing production does not democratize demand.** When AI makes code, content, and products cheap, being able to make the thing is no longer an advantage. Value moves to scarce complements: distribution, trust, accountability, proprietary data, relationships, and physical or regulated access.

Most ideas fail this test, and saying so plainly is the point. But "not a business" isn't "worthless." A project can be good art, a useful tool, or a worthwhile experiment. Give each idea the label that fits.

The full framework is in [references/framework.md](references/framework.md). Read it before your first evaluation in a session. Everything below assumes it.

## 1. Load the user's profile

The framework judges an idea *for a specific person*, so constraints come first. The profile lives at `~/.config/scarcity-shift/profile.md`.

- **The profile exists:** read it and continue.
- **The user describes their situation in the message:** use that for this run. At the end, offer to save it as their profile.
- **No profile and no situation given:** run first-time setup from [references/setup.md](references/setup.md). Send only the setup questions, plus one line saying they can reply "skip" to get the evaluation now, then wait. Don't include a provisional verdict: a full analysis in the same message buries the questions, and the verdict would change once you know their constraints. If they skip, evaluate anyway, mark Gate 1 (constraints) as unverified, and say what you'd need to know.
- **The user says `setup`, or asks to change their profile:** run setup again, starting from their current answers.

The profile is personal: job, family, money, limits. Keep it on the user's machine. Don't repeat sensitive details in the verdict card, because people share those.

## 2. Understand the idea

Restate the idea in one sentence: who pays, for what outcome, and how they'd find it. If that's clear enough to judge, don't ask questions. State your assumptions and go.

Ask only when an answer would change the verdict, for example "Do you already know any buyers?" Ask at most three questions in one round, and offer to proceed on stated assumptions instead.

If you can search the web, spend a few searches on what matters most: existing competitors, where the buyers already gather, and real demand signals. Cite what you find. Without search, say what you'd check. Never invent market numbers.

## 3. Evaluate

Work through the four scarcity questions and the eight gates in the framework. Some habits make the analysis honest:

- **Constraints before upside.** A great idea that collides with the profile is "Option Vault," not "Pursue now."
- **Make distribution concrete.** Name the actual place buyers gather, or say there isn't one. "Post on social media" and "SEO" aren't distribution plans until you can say why this person would win there.
- **Run the diffusion test literally.** Imagine a competitor with agents 10× better and 10× cheaper rebuilding this over a weekend. What's left?
- **Keep the classification honest.** Sophisticated implementation doesn't upgrade a hobby into a business. Evidence of demand does.
- **Credit what is real.** If the person owns a scarce asset, like relationships, access, a reputation, or data, say so plainly. That's what the framework is looking for.
- **Separate the three judgments:** good idea, valuable business, and actionable for this person now.

## 4. Write the result

Lead with the verdict card. People screenshot and share it, so keep it free of personal details from the profile:

```
SCARCITY SHIFT VERDICT
Idea: <one line>
Classification: <one of the nine>
Verdict: <one of the allowed verdicts>
Scarce asset: <what the person would own, or "none yet">
Smallest honest test: <one line>
```

Then the full analysis, in this order, a few lines each:

1. **Primary classification**, and why.
2. **Economic thesis**, in one sentence.
3. **Steelman:** the strongest honest case for it.
4. **Red team:** the most likely way it fails.
5. **Constraint conflicts** with the profile.
6. **What became abundant.**
7. **What remains scarce.**
8. **Distribution route:** owned, borrowed, or embedded, and specifically where.
9. **Diffusion test:** negative, neutral, or positive, and why.
10. **Economic asymmetry:** strong or weak, and why.
11. **Ownership boundary:** where generated work becomes an accountable outcome.
12. **Compounding asset:** what each run adds that competitors can't regenerate.
13. **Attention-adjusted return:** including the non-money costs.
14. **Smallest honest test:** manual, cheap, and fast, with a clear signal. No pipelines or platforms before demand is proven.
15. **Explicit stop conditions:** the observations that end the experiment.
16. **Decisive verdict:** one of the allowed verdicts, with one or two sentences of reasoning.

Write in plain, direct language. Be kind and blunt. Don't hedge the verdict into mush, and don't overclaim. You're judging the odds and the fit, not predicting the future.

For several ideas, give each its own card and a short analysis, then rank them. For calibration, [references/examples.md](references/examples.md) has worked evaluations. Read it when unsure how strict to be.
