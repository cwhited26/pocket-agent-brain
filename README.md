# Your Business Brain

Five folders. One repo. Everything your Pocket Agent knows about your business.

This is the template every Pocket Agent user starts with. It ships pre-filled with a real, working example — the shape of the brain running three real businesses (Whited Consulting, AthleteOS, Tennessee Valley Exteriors) right now — so you have something to model on, not a Lorem-ipsum scaffold.

Fork it. Edit it to be yours. Connect Pocket Agent to it. Your agent starts drafting in your voice, quoting your prices, knowing your customers, defending your positioning — from turn one.

---

## The five zones

The brain has five zones. Every zone is a folder. Every folder answers one question.

| Folder | Question it answers |
| :--- | :--- |
| `voice/` | How do you talk? |
| `customers/` | Who buys from you? |
| `products/` | What do you sell? |
| `competitive/` | Who else do they compare you to? |
| `decisions/` | What calls have you made, and what rules don't you break? |

Read those five READMEs and you know what Pocket Agent knows.

## How Pocket Agent reads this repo

Zone-scoped retrieval. When your agent drafts an email to a customer, it reads `voice/` + the relevant `customers/` file + `decisions/standing-rules.md`. When it drafts a landing page, it reads `voice/` + `customers/segments/` + `products/` + `competitive/positioning.md`. When it quotes a price, it reads `products/` + `decisions/decision-log.md`.

**It only reads what it's allowed to.** Personas you configure in Pocket Agent get scoped access to specific zones. The "Public brochure" persona might read `products/` and `competitive/positioning.md` only. The "Internal assistant" persona reads everything. **You control who sees what.**

## Your account, your data, your control

- The repo lives **in your GitHub account**, not ours. Fork it and it's yours.
- Pocket Agent reads it via a GitHub app you install and can revoke any time.
- Nobody at Anthropic, at Pocket Agent, or anywhere else can see your brain repo without you giving explicit access.
- No AI service will read your brain unless you connect it. Pocket Agent's default is: read this repo, do not send its contents to third-party APIs beyond the model that drafts your response, and never persist a copy outside the session.
- Secrets don't live in this repo. Ever. Reference env var names in `CLAUDE.md`; keep the values in your password manager.

## How to fill this out

Two paths:

**During the workshop.** You bring the workbook (`pocketagent.com/workshop/workbook.pdf`), fill in the blanks live, then walk through the five zones with Pocket Agent — it reads your answers back into these folders as you go.

**On your own.** Read the five zone READMEs. Delete the example files. Write your own using the shape they demonstrated. Or edit the examples in place — every "Chase," "Patrick," "APA," "BOS," "TVE," or specific product is a placeholder for your own reality.

Both paths work. Both end with your agent reading a brain that knows your business.

## What's in this repo — full map

| File or folder | What it is |
| :--- | :--- |
| **The five zones** | |
| `voice/` | How you talk — spec, examples, transcripts, influences |
| `customers/` | Who buys from you — profiles, segments, anti-personas |
| `products/` | What you sell — feature inventory, product specs, pricing, change log |
| `competitive/` | Who else they look at — intel, deep dive, positioning |
| `decisions/` | Your calls + your standing rules |
| **The plumbing** | |
| `CLAUDE.md` | Master context every agent reads first |
| `AGENTS.md` | Cross-agent behavior rules |
| `MEMORY.md` | Standing facts your agent should always know |
| `memory/` | One file per topic-level memory |
| `memory-types/` | Explainers for each memory category |
| `memory-conventions/` | Brain-hygiene patterns (4-place rule, supersession pattern, etc) |
| `daily-log.md` | Append-only timeline of what happened |
| `decision-log.md` | Deprecated — moved to `decisions/decision-log.md` |
| `change-log.md` | Commit-style ledger |
| `feature-inventory.md` | Deprecated — moved to `products/example-feature-inventory.md` |
| `handoff-doc.md` | Session-handoff template |
| `bin/` | Helper scripts (lane summaries, staleness audits) |
| `hooks/` | Ambient-capture hooks |
| `prompts/` | Starter prompts |
| `.github/pull_request_template.md` | Short PR template for edits |

The five zones are new. The plumbing was already there from the previous scaffold and stays — it's how the brain stays organized as it grows.

## Getting started right now

1. **Click "Use this template"** at the top of this page. Give the new repo a name like `my-business-brain`. Keep it private if you like — everything in this file assumes you own it.
2. **Read the five zone READMEs** in order: voice → customers → products → competitive → decisions. Ten minutes, tops.
3. **Connect Pocket Agent.** In the Pocket Agent dashboard, paste your repo URL. Your agent starts reading from this point on.
4. **Edit or replace the example files.** Every zone ships with real working examples. Read them once, then make them yours.
5. **Your agent is ready.** Ask it to draft an email to your best customer. Watch it sound like you.

---

## Privacy

This repo is yours. Pocket Agent reads it, but nobody else does — not us, not Anthropic, not the model providers beyond the specific draft in flight, not any third party. GitHub's own privacy applies. If you make the repo public, that's your call.

**Don't put API keys, passwords, tokens, or live customer data in this repo.** For real customers, blur the names in this repo and keep the real data in your CRM. For secrets, reference env var names only.

## Questions

Visit [pocketagent.com](https://pocketagent.com) or reach out via your Pocket Agent dashboard. If you're stuck on what belongs where, the answer is almost always: real over pretty, specific over abstract, honest over corporate.

---

*Business Brain template — Pocket Agent × Buildout Studios × 2026.*
