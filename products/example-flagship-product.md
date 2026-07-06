# [Composite Custom-CRM Build] — full product spec

**Type:** Example, blurred. Modelled on the flagship offering of an operator-run consulting practice that ships custom CRMs for owner-operated contractors.
**Status:** Selling. Standard offering.

---

## What it is (one line)

A custom CRM built to how *you* actually run your business — you own the code, we ship in weeks not months, we stay on the hook for the bugs after launch.

## Who it's for

Owner-operated contractors doing $1-5M in annual revenue. Insurance restoration + retail residential. See `customers/segments/example-segment-a.md` for the full segment profile.

## What's in it (deliverables — every one gets shipped)

- **Custom CRM.** Full source in the client's own GitHub organization. Runs on the client's own Vercel + Supabase (we set it up, keys are on their card).
- **The core modules:** lead intake, job pipeline (Kanban), calendar, rep management, documents, comments, notifications.
- **The workflow engine:** primary insurance workflow tuned to the client's actual process; secondary retail workflow; per-step validators.
- **Rich PDFs.** At least 3 templates. Damage report, scope agreement, certificate of satisfaction (or the client's equivalents).
- **E-signature round-trip.** Send-for-signature → recipient view → sign → confirmation.
- **Photo album.** Company Cam equivalent — Konva annotation, before/after compare, share-via-link.
- **AI intake.** Transcript-to-job extraction with owner review.
- **Field app PWA.** Photo checklist, camera capture, offline-tolerant.
- **A branded owner dashboard** with a "where your dollars are coming from" ROI chart in *their* vocabulary.
- **30-day punch list.** Any bug you find in the first 30 days is on us. No new features — bugs only.

## What's NOT in it (say this at intake)

- **A marketing website.** We don't build websites in this scope. If yours is embarrassing, we can quote it separately.
- **Migration from your existing system.** If you have data in another CRM, we can quote the migration separately.
- **Integrations with your specific carriers, adjusters, or vendor systems** beyond the standard set (calendar, email, storage). One custom integration can be added for $XXX.
- **Ongoing feature development.** After the 30-day punch list, new work is quoted per lane.
- **Managed hosting.** You own Vercel and Supabase. We can walk you through their onboarding.

## Pricing

- **Standard:** $2,500 - $6,000 one-time, depending on scope complexity. See `example-pricing-tiers.md` for the tier breakdown.
- **Deposit:** 100% up-front for standard builds. Enterprise-tier builds only can split.
- **Hosting:** monthly on the client's own accounts. Ballpark $30-$100/mo depending on volume, on the client's Vercel + Supabase.

## Delivery

- **Timeline:** measured in shipping lanes, not calendar. Standard build is 4-6 shipping lanes across a 6-10 week window.
- **What a "shipping lane" is:** one autonomous coding session that ships end-to-end. Each lane is scoped in the brain first, then executed and pushed to main.
- **Weekly check-in.** One 30-minute call, same time every week.
- **Async updates.** Loom + text between calls. No standing meetings otherwise.

## Guarantee

- **30-day punch list.** From the day the build lands on main, any bug on the client's punch list gets fixed. Free.
- **60-day extended guarantee** on enterprise-tier builds.
- What's not covered: new features, scope changes, "wouldn't it be nice if…" additions. Those are new lanes with new invoices.

## What we won't do

- White-label the code to another agency.
- Take equity instead of cash.
- Build for pre-revenue clients (see `customers/example-not-a-fit.md`).
- Ship without a written scope and a paid deposit.

## How the customer pays

Stripe payment link, one-time. We send the link once the scope is written and both sides have signed the one-page agreement. Work starts when the link clears.

## Upsells (post-launch)

- **Additional lanes.** Priced $500-$1,500 per lane depending on complexity.
- **A dedicated marketing site.** Separate scope, separate quote.
- **A second workflow module** (say, the client adds a new service line and needs a workflow for it). Separate scope.

## What we learned shipping this repeatedly

- The bar isn't the CRM — the bar is the *photo module*. Every client names the photo tool as their biggest ongoing pain. Ship that lane last, and it's the moment the whole build becomes real.
- Owner vocabulary trumps SaaS vocabulary everywhere. If the client says "kick it back," "front of the house," "adjuster confirmation" — those are the labels in the UI. Never SaaS-generic terms.
- Realistic mock data with math tied out is non-negotiable for the review demo. Anything less looks like a scaffold.

## Cross-references

- Full feature list: `products/example-feature-inventory.md`
- Pricing tiers detail: `products/example-pricing-tiers.md`
- The decisions that shaped this offering: `decisions/decision-log.md`
