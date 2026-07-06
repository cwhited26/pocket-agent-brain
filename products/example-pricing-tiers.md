# Pricing Tiers — Custom-CRM Build

**Type:** Example, blurred. Three tiers, anchored on the middle. Prices are real ranges from a real business.

The tiers are Standard / Team / Enterprise. Every tier ships the same **core**. What changes between tiers is scope, integrations, guarantee window, and included lanes.

---

## Standard — $2,500

For solo operators or small crews (<10 people) who need the CRM to run the way *they* run.

**Includes:**
- Custom CRM with core modules (intake, pipeline, calendar, documents, comments).
- Primary workflow engine tuned to the client's own process, up to 30 steps.
- 2 PDF templates (damage report + one other).
- E-signature round-trip.
- Photo album with annotation + before/after + share link.
- Owner dashboard with a client-vocabulary ROI chart.
- 30-day punch list.
- Deployment to the client's own Vercel + Supabase.

**Ships in:** 4-6 shipping lanes across 6-8 weeks.

**Best for:** the buyer who just wants the tool. Not multiple crews, not multiple offices, not an integration-heavy stack.

---

## Team — $4,500

For crews of 10-20 with reps who need onboarding, workflows for insurance + retail, and one custom integration.

**Includes everything in Standard, plus:**
- Second workflow engine (retail path), up to 15 steps.
- Rep onboarding checklist + knowledge base with walkthrough placement.
- 3 PDF templates.
- AI intake from transcript.
- One custom integration (a specific carrier, a specific vendor system, or an existing data source).
- Documents auto-routing.
- 30-day punch list.

**Ships in:** 6-8 shipping lanes across 8-10 weeks.

**Best for:** the operator with a real desk staff + field crew and a Yes-path branching workflow (insurance vs retail, residential vs commercial, etc.).

---

## Enterprise — $6,000

For established shops with a second office, complex workflows, or a specific vertical need (permits, subcontractor management, multi-crew scheduling).

**Includes everything in Team, plus:**
- Photo checklist per job type.
- Inspections module with property walkthrough.
- Production notes + work orders + crew-facing production PDF.
- Color library (per-org catalog).
- Two custom integrations.
- 60-day extended punch list.
- Post-launch training session (60 minutes) with the office manager.

**Ships in:** 8-12 shipping lanes across 10-14 weeks.

**Best for:** the shop scaling past $3M revenue where the CRM has to hold the field crew as well as the office.

---

## What sits above Enterprise

Nothing productized. If the ask is bigger than Enterprise, it's a custom scope with a custom quote. Enterprise is the ceiling of the productized offering.

## What sits below Standard

Nothing. If the buyer can't afford Standard, they're not a customer yet. See `customers/example-not-a-fit.md` — pre-revenue prospects go on the "when you're there, come back" list, not into a discounted tier.

## Hosting (all tiers)

The client owns Vercel + Supabase on their own credit card. We provision the projects at build-time; the keys and access stay with them from day one. Expected monthly cost after the free tier: $30-$100 depending on data volume and photo storage.

## Payments (all tiers)

- Standard + Team: 100% up-front via Stripe payment link.
- Enterprise: 50% up-front, 50% on landing on main.
- No net-30, no invoicing on trust. Every build starts once the deposit clears.

## Why the tiers are named this way (delete when you replace)

- No cutesy names. "Starter / Pro / Business" would work too, but "Standard / Team / Enterprise" reads more grown-up on a proposal to an owner-operator.
- Middle tier is the anchor. Standard is the "no, this is the real minimum" tier. Enterprise is the "here's what we can do if you need it" tier. Team is where most sales close.
