# Shot write-up: portfolio write-ups for designers

An agent skill that turns your rough notes, brief or screenshots into a short write-up of one piece of design work: a title, a one-line hook, then context, process and outcome. Use it for a portfolio case study, a LinkedIn post or a Shot. Works in Claude Code, Claude, Cursor, Codex and any agent that reads `SKILL.md` skills.

## Before and after

**Your notes:**

> redesigned checkout for a small coffee roaster's webshop. people dropped off at shipping step, 4 screens → 1. tested with 5 customers. owner says fewer emails about delivery costs now

**The write-up:**

> **One-page checkout for a coffee roaster**
>
> A simpler checkout for a small roaster's webshop, built around one screen.
>
> **Context.** Customers were dropping off at the shipping step, and the owner was answering emails about delivery costs every week.
>
> **Process.** I mapped the four checkout screens, merged them into one, and showed delivery costs before payment. I tested the new flow with five customers and adjusted the address form after their feedback.
>
> **Outcome.** The owner now gets fewer emails about delivery costs, and the checkout fits on one screen.

The skill never invents numbers, quotes or results. If something is missing, it asks you, or leaves a placeholder like `[add your outcome]`.

## Check before you post

After the draft, the skill offers four quick questions: confidentiality (is this OK to share under your NDA?), the problem, your role and credit, and the outcome. In Claude Code they show up as tabs; in other agents as a numbered list with suggested answers.

## Install

**Claude Code**

```
/plugin marketplace add Bazeloth/designer-shot-writeup
/plugin install shot-writeup@designer-shot-writeup
```

**Any agent, with [skills.sh](https://skills.sh)**

```
npx skills add Bazeloth/designer-shot-writeup
```

**By hand:** copy `skills/shot-writeup` into your agent's skills folder (for Claude Code, `~/.claude/skills/`).

Then ask: "Write up this project for my portfolio" and paste your notes or screenshots.

## Made by PixelPorts

[PixelPorts](https://www.pixelports.com/?ref=skill-writeup) is a free portfolio platform for designers at every career stage. Approved designers get 90 days of extra reach for their work while they build an audience.

MIT licensed.
