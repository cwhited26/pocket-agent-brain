# Product Change Log — Custom-CRM Build

**Type:** Example, blurred. Append-only ledger of what changed in the standard offering. New entries at the top. Nothing gets deleted.

The rule: every non-trivial change to the productized offering — added deliverable, dropped deliverable, price change, guarantee window change, template swap — lands here with a date and a one-line why.

---

## 2026-06 — Photo album lifted to mandatory (was optional in Standard)

Every build shipped in the last 6 months named the photo module as the highest-perceived-value feature. Moved it from Team/Enterprise-only to Standard.

**Impact:** Standard build now takes 1 more shipping lane. Held the price at $2,500 — reads as more value at the same price.

## 2026-05 — 30-day punch list codified as a written guarantee

Was informal ("we'll fix bugs after launch") for the first 8 builds. Made it a written guarantee on the scope doc. See `decisions/decision-log.md` entry on the guarantee lock.

**Impact:** Higher close rate on the first call (three out of the last five). Zero increase in support hours actually consumed — most 30-day windows close with 0-2 bug reports.

## 2026-04 — Enterprise tier launched

Added at $6,000. First customer bought Team + a custom expansion for $2,000 more — that "expansion" became the anchor for the Enterprise tier features.

**Impact:** Team-tier close rate went up. The Enterprise tier's function is to make Team look sensible.

## 2026-03 — Standard raised from $1,500 to $2,500

Was underpricing based on lanes actually shipped. The math: standard build is 4-6 lanes averaging 6-8 hours each = 30-40 hours all-in. $1,500 was $37-$50/hr; $2,500 is $62-$83/hr.

**Impact:** No churn from prospects at the higher price. Two prospects who wanted the $1,500 price were the anti-persona anyway (see `customers/example-not-a-fit.md`).

## 2026-02 — E-signature round-trip added to Standard

Was Team-only. Moved to Standard because a Standard customer asked for it and paid for the lane. Now it's baked in.

**Impact:** Standard build takes 1 more lane. Price held.

## 2026-01 — First productized version shipped

Before this, every build was custom-scoped. The productized version was the pattern that survived four builds in a row. Wrote the scope doc, wrote the tier sheet, put it on the shelf.

**Impact:** Sales cycle dropped from 3-4 weeks to 5-10 days for buyers in the primary segment.

---

## Notes on the append-only rule

- Never delete an entry.
- If a change gets reversed, add a new entry at the top explaining the reversal — don't strike out the old one.
- If a price changes, the old price stays visible in this file — that's how future-you (or your agent) knows what the old customer paid.
