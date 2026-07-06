# Feature Inventory — [Composite Custom-CRM Service]

**Type:** Example, blurred. Modelled on the shape of a real BOS Custom client's inventory.
**Purpose:** Brain-level shipped-feature registry. Source-of-truth for "is X built yet?" across every product this business ships.

**Last verified:** 2026-06-15

---

## Shipped

### Core CRM Foundation
- **Lead intake + Job pipeline** — job creation, customer records, jobs-as-the-canonical-lead abstraction. `STAGE_TO_COLUMN` kanban mapping.
- **Kanban drag-drop** — dnd-kit; owner/manager can move jobs between columns; server action with audit trail.
- **Calendar + drag-to-day** — per-event drawer, Quick-Move panel, move-event action across all 3 event sources.
- **Rep management** — roster, activate/deactivate flow, add-team-member flow with auth invite emails.
- **Documents tab** — folders + tags + workflow-context auto-routing. Default folders for the vertical.
- **Comments + @mentions** — comments table, notification trigger, real-time updates.
- **Notification preferences** — per-rep opt-in, email mirror for the boss.

### Workflow Engine
- **Primary workflow** — 50 steps, split-branch routing, per-step validators. Living v4, v3 kept intact for in-flight jobs.
- **Secondary workflow** — 6 steps for the retail path.
- **Insurance vs Retail split** — lead intake radiogroup; each creates a job on the correct template chain.
- **File-Claim-on-Spot Yes-path** — required fields, storm-date chips, phone camera capture for SRA upload.
- **Mark-Complete predicates + bypass scaffold** — validator registry, request-bypass action, approval inbox distinguishes bypass from system gates.

### PDFs
- **Damage report** — full template redesign, custom fonts, 2-up photo layout, per-page running header/footer.
- **Cover photo selection** — per-report cover, badge on editor, PDF resolves before fallback.
- **Bulk photo add** — batched upsert/delete.
- **Scope-of-work multi-select chips** — settings editor, auto-fill English-list into conclusion textarea.
- **Bottom action button mirror** — Save Draft / Preview / Send / Finalize repeated at bottom of editor.
- **Damage report edits audit log** — append-only, admin-only history drawer, before/after JSONB diff.
- **Photo-link TTL config** — 7 to 365 days, default 30. Settings tab.

### Estimates
- **3-tier Good/Better/Best estimate builder** — tier-scoped saves, pricing catalog products.
- **Auto-fill from catalog + custom markup** — substitution report after fill.
- **Send all 3 tiers as one email** — 3 PDFs attached.
- **Estimate status workflow** — DRAFT → SENT → ACCEPTED/REJECTED/SUPERSEDED. Audit columns.
- **Pricing template seed** — line items loaded via SQL function, idempotent, UI button.

### Onboarding + Knowledge Base
- **Rep onboarding checklist** — items table, default items, access-action enum for CRM-access vs manual-tracking.
- **Knowledge base** — categories + articles. Rep-facing search. Admin editor. Ships empty for the client to fill.
- **Walkthrough placement** — articles seeded with narrated transcripts. Per-page help banners on 12 mounts.

### AI Features
- **AI Intake from transcript** — dedicated route, extraction via cheap tool-use, cost metered, editable review, create-job.

### Field Operations
- **Inspections / Photo Checklists** — 26-checkpoint walkthrough, collapsible accordion, camera capture, "general photos" section.
- **Color library** — per-org paint/material catalog, search, job/customer tabs.
- **Production notes + work orders** — production notes table, work orders table, crew-facing production PDF.

---

## Not Yet Shipped — Pending

| Feature | Gate |
| :--- | :--- |
| Mark-Complete validator registry population | Customer email reply on step_keys + min-length + approver scope |
| YouTube walkthrough embeds | Customer confirms channel |
| Payments module | Deferred until v2 |
| Public-facing website | Client decision on scope |

## Not on the roadmap (by decision)

- Native mobile app — PWA covers the use case.
- Multi-tenant / SaaS version — this is a Custom build, one owner only.
- White-label reseller access — not selling the code to third parties.

---

## Cross-references

- Pricing: `products/example-pricing-tiers.md`
- Product-level detail: `products/example-flagship-product.md`
- Change log: `products/example-change-log.md`
- Decisions that shaped these features: `decisions/decision-log.md`
