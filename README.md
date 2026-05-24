# Your Business Brain

This is your brain — the memory your Pocket Agent reads before it does anything.

Every time your agent starts a session, it opens this repo first. It reads who you are, what your business looks like, what projects are in flight, and what rules apply. Without a brain, your agent starts from zero every time. With one, it picks up where you left off.

---

## How to get started

1. **Click "Use this template"** at the top of this page to create your own copy. Give it a name like `my-business-brain` — it's yours to keep.
2. **Connect it to Pocket Agent.** In the Pocket Agent dashboard, paste in your new repo's URL. Your agent will read it from this point on.
3. **Run the setup wizard.** The wizard asks you about your business, your stack, and how you like to work. It fills in this repo automatically. You don't have to write anything yourself.

That's it. Your agent is ready.

---

## What's in here

| File or folder | What it does |
| :--- | :--- |
| `CLAUDE.md` | The master context file — your business overview, code rules, and agent behavior instructions |
| `MEMORY.md` | A running index of standing facts your agent should always know |
| `AGENTS.md` | Rules for how agents should behave, hand off, and coordinate |
| `memory/` | Individual memory files — one per topic. The setup wizard creates these; you can edit them anytime |
| `memory-types/` | Explainers for each memory category (user, project, feedback, reference) |
| `memory-conventions/` | Patterns for keeping your brain clean and consistent over time |
| `daily-log.md` | A running timeline of what happened — append only, never edited |
| `decision-log.md` | Decisions with rationale — so you and your agent know why, not just what |
| `change-log.md` | Commit-style ledger across all your projects |
| `feature-inventory.md` | What's shipped, what's in progress, what's planned |
| `bin/` | Helper scripts for generating summaries and surfacing stale docs |
| `hooks/` | Agent hooks that can auto-capture context as you work |
| `prompts/` | Starter prompts for common agent tasks |

---

## It's all yours

Everything in this repo is yours to read, edit, and own. Your agent writes to it, but you're in control. You can edit any file directly — add context, correct something the wizard got wrong, or add notes your agent should know.

The more accurate this repo is, the better your agent performs. Think of it like briefing a new team member: the more context they have, the faster they can help.

---

## Privacy

This repo is private by default. Your business information stays on GitHub, which you control. Pocket Agent reads it but never shares it. Treat this like any private repository — don't add API keys, passwords, or sensitive personal data directly. See `MEMORY.md` for guidance on what belongs in memory and what belongs in a password manager.

---

## Questions?

Visit [aipocketagency.com](https://aipocketagency.com) or reach out to support from your Pocket Agent dashboard.
