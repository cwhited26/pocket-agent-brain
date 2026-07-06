# Decision Log

**Type:** Example, blurred. Eight composite decisions from a real operator business (custom-CRM build shop). Written in the shape of a mature append-only log.

**Format:** Append-only. New entries at the top. Numbering never reused. Nothing deleted. When a decision gets superseded, the new entry references the old one; the old one stays visible and gains a `Superseded by #N` marker.

**Numbering convention:** integer counter, prefix-free. When you split this file into per-product logs, prefix them then.

---

## #8 — 2026-06-15 — Written 30-day punch-list guarantee, not verbal

**Decision:** Every scope doc from today forward carries a written 30-day punch-list guarantee. Bugs found in the first 30 days after the build lands on main get fixed for free. New features do not.

**Why:** Close rate on the discovery call jumped after we started saying "written guarantee" instead of "we'll take care of you." The words weren't the difference — the writing was. The buyer read it as a real commitment.

**Alternatives considered:** 60-day guarantee (too much scope creep pressure), no guarantee (too much perceived shipping risk), guarantee tied to a subscription (breaks the "you own the code, no ongoing SaaS" positioning).

**Downstream impact:** `products/example-flagship-product.md` guarantee section, `products/example-pricing-tiers.md` under every tier, sales page copy, first-call script.

---

## #7 — 2026-05-20 — Enterprise tier at $6,000, no productized tier above it

**Decision:** Add an Enterprise tier at $6,000 including two custom integrations, extended 60-day guarantee, and a post-launch training session. Do NOT productize anything above Enterprise — bigger asks are custom scopes with custom quotes.

**Why:** Two prospects in a row asked for scope that didn't fit Team-tier. Rather than cap the offering at Team, added a real anchor above. Middle-tier close rate went up.

**Alternatives considered:** Cap at Team ($4,500), leave everything above Team as pure custom (fine but sales cycle is 2x longer), price Enterprise at $10k (would have been too high — $6k anchor works because it's a stretch, not a discount conversation).

**Downstream impact:** `products/example-pricing-tiers.md`, `products/example-change-log.md` entry.

---

## #6 — 2026-05-05 — Photo album moved to Standard (from Team+)

**Decision:** The photo album module — annotation, before/after, share-link, per-job album — is in Standard tier from now on. Was Team-tier only.

**Why:** Every build shipped in the last 6 months named the photo module as the highest-perceived-value feature. It was underweighted in the tier structure. Moved it. Standard build now takes 1 more shipping lane; price held.

**Alternatives considered:** Raise Standard price to $3,000 (lost the $2,500 anchor advantage), keep it Team-only (kept losing Standard-tier prospects who wanted the photo module).

**Supersedes:** #3 (original tier structure, 2026-01).

**Downstream impact:** All product docs. Also `products/example-flagship-product.md` deliverables section.

---

## #5 — 2026-04-10 — Refuse pre-revenue "co-founder" pitches, no exceptions

**Decision:** Any prospect whose current revenue in the target line is zero is disqualified at intake. The equity-for-work pitch is a hard no. Standing rule; see `decisions/standing-rules.md`.

**Why:** Three of these ate ~50 hours combined in Q1 and closed zero dollars. The anti-pattern is documented at `customers/example-not-a-fit.md`. Cheaper to filter at intake than to disqualify at proposal-stage.

**Alternatives considered:** A cheaper "MVP" tier for pre-revenue buyers (creates a downstream expectation problem for real customers), keep the option open case-by-case (loses discipline, we keep saying yes).

**Downstream impact:** `customers/example-not-a-fit.md`, `decisions/standing-rules.md` rule #7, intake-form disqualifier field.

---

## #4 — 2026-03-15 — Standard raised from $1,500 to $2,500

**Decision:** New Standard-tier price is $2,500. All new scopes from today onward. Existing scopes at the old price honored.

**Why:** Was underpricing based on actual lanes shipped. Math: standard build averages 30-40 hours all-in; $1,500 = $37-50/hr; $2,500 = $62-83/hr. Two prospects who wanted the old price were anti-persona anyway.

**Alternatives considered:** $2,000 (would have felt like an apology), $3,000 (would have moved us out of the "anchor for first-time custom-CRM buyer" spot).

**Downstream impact:** `products/example-pricing-tiers.md`, `products/example-change-log.md`.

---

## #3 — 2026-01-10 — Productize with three tiers (Standard / Team / Enterprise)

**Decision:** Productize the custom-CRM offering. Three named tiers. Written scope for each. Published tier sheet.

**Why:** Sales cycle was 3-4 weeks per custom quote. Realized the last four builds were essentially the same shape with the same modules. Wrote it up as a productized offering; sales cycle dropped to 5-10 days.

**Alternatives considered:** Stay fully custom (protects margin per deal, kills volume), pick a single-tier flat-rate (misses the anchor effect).

**Superseded by:** #6 (photo album moved to Standard, 2026-05), #4 (Standard raised to $2,500, 2026-03).

**Downstream impact:** Every file in `products/`.

---

## #2 — 2025-11-20 — All builds ship on the client's own Vercel + Supabase

**Decision:** No hosted / managed / white-labeled option. Every client owns their Vercel + Supabase projects on their own credit card. We provision at build-time; access transfers day one.

**Why:** The positioning is "you own the code." Managed hosting undercuts that — the moment the client's credit card isn't on the account, we're a SaaS in disguise.

**Alternatives considered:** Offer managed hosting for a monthly fee (rejected — undercuts positioning), require Vercel Pro / Supabase Pro at signup (rejected — starting tier free is fine for the first year for most builds).

**Downstream impact:** `products/example-flagship-product.md`, every scope doc, onboarding walkthrough.

---

## #1 — 2025-10-01 — Written scope + paid deposit before any code

**Decision:** No code gets written until: (a) the scope is written and both sides have signed it, (b) the deposit has cleared. Standing rule.

**Why:** Every "I'll get the invoice paid this week, can you start?" turned into two weeks of work followed by a scope debate. The deposit is signal that the buyer is real.

**Alternatives considered:** Small "starter fee" of $500 to begin scoping (rejected — either the buyer commits to the whole thing or they don't), verbal scope confirmed by email (rejected — every ambiguity got expensive later).

**Downstream impact:** `decisions/standing-rules.md` rule #1, every scope doc, discovery-call script.

---

## Notes

- When a new decision supersedes an older one, the older entry gets a `Superseded by #N` line. It stays in the file. Reading through the log in order tells you not just where you are but how you got here.
- Decisions can be re-opened. That's a new decision, not an amendment to the old one.
- The mature log is boring. Boring is good. If your log reads like a novel, you have too many philosophical decisions and not enough calls.
