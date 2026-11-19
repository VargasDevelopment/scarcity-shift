# First-time setup

The framework judges ideas for a specific person. Setup captures that person's constraints and assets once, so later runs need no preamble. Keep it to one round of questions, and finish in a couple of minutes.

## Ask

Explain in one sentence why you're asking. Then ask these questions in a single message, numbered. Say that short answers are fine and any question can be skipped.

1. **Work and employer adjacency:** What field do you work in? Are there topics, customers, or technologies your employer would consider too close to your work? You don't need to name the employer.
2. **Time and energy:** How many hours a week can you realistically give a side project? What time is protected, such as family, sleep, health, or rest?
3. **Public exposure:** Which are you comfortable with: staying anonymous, using your name, your voice, your face?
4. **Customer contact:** Are you OK with sales calls, support requests, or ongoing client work? Or do you want low-touch only?
5. **Money:** How much are you willing to risk? Do you need income soon, or is this long-term?
6. **What you already have:** Skills, an audience, a reputation, professional relationships, domain access, local or physical access, data, or equipment that others lack.
7. **Goals:** What would make a project worth it: income, career growth, learning, reputation, fun, or helping someone specific?
8. **Hard nos:** Anything you won't do?

## Save

Write the answers to `~/.config/scarcity-shift/profile.md` with this shape, in the user's own words where possible. Leave skipped items as "unknown" rather than guessing.

```markdown
# Scarcity Shift profile
Updated: <YYYY-MM-DD>

## Constraints
- Work and employer adjacency: ...
- Time and protected time: ...
- Public exposure: ...
- Customer contact: ...
- Money: ...
- Hard nos: ...

## Assets
- ...

## Goals
- ...
```

Create the folder if needed. If the environment blocks writing outside the project, show the profile and tell the user the one command to save it, such as a `mkdir -p ~/.config/scarcity-shift` plus a heredoc.

Tell the user where the profile lives, that it never leaves their machine, and that `/scarcity-shift setup` updates it. Then continue with the idea they asked about, if any.

## Updating

When rerunning setup, show the current profile first. Ask only what they want to change.
