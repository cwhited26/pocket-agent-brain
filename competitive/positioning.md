# Positioning

**This file holds the operator's positioning lock — the sentences your agent uses when it needs to say WHY somebody picks you.**

Everything else in `competitive/` describes the field. This file is the pitch.

---

## The one-line why-us

> **You'll own the code, we'll ship in weeks not months, and I still have skin in the game after the launch.**

This is the sentence Pocket Agent reaches for when it needs to answer "why you?" in a cold email, a landing hero, a sales-call rebuttal. Every word earns its place — see `customers/segments/example-segment-a.md` for the breakdown of why each phrase catches the primary segment.

## Do not use these variants

- ~~"We're the best in the industry."~~ Meaningless.
- ~~"Award-winning software."~~ Also meaningless.
- ~~"Trusted by hundreds of contractors."~~ Not true, and even if it were, the number is either too small to be impressive or too big to be honest.
- ~~"Enterprise-grade."~~ Corporate deck word. Off-brand for us.

## Positioning by segment

### For the primary segment (owner-operated storm restoration contractors, $1-5M)

> **You've built a real business. You know your workflow. You need software that fits the way *you* work, not another SaaS you'll fight for the next 3 years.**

The hook: acknowledge the business is real, acknowledge the workflow is theirs, name the alternative as the fight it actually is.

### For the secondary segment (adjacent verticals — cleaning, HVAC, small commercial)

> **We build for how *you* run a job. Not a category, not a template. Your workflow, your language, your code.**

The hook: adjacent-vertical buyers will assume our system is roofing-shaped. Kill that assumption up front.

### For the referral-source segment (past customers)

> **Text me who you're thinking of. I'll qualify them before you have to.**

The hook: past customers refer us into their groups. Make the referral one-tap and pull the qualification burden off them.

## What we are NOT

- A SaaS.
- A no-code platform.
- A managed service.
- A consulting firm.
- An agency (in the traditional retainer sense).

We are a build shop that ships owned software. Every sentence in customer-facing copy is checked against this list. If the sentence could be said by any of the above, rewrite it.

## Positioning notes for the person on the phone

If a prospect asks how we're different from a specific competitor, the honest answer is on file — see `competitive/deep-dive-example.md` and `competitive/competitor-intel.md`. The sales-call rule: don't attack, describe. "They're a horizontal SaaS. We're a custom build. Here's what that means for you specifically." Then read the specific line from `customers/segments/*.md` that matches the prospect.

## When positioning changes

Positioning changes when the win/loss ratio in a segment shifts, or when a competitor makes a move that erodes a differentiator. When it changes:

1. Amend the "one-line why-us" here.
2. Add an entry to `decisions/decision-log.md` explaining the change.
3. Never delete the old version — mark it superseded (see `memory-conventions/supersession-pattern.md`).
