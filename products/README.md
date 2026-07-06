# products/ — what you sell

**This is Zone 3 of your Business Brain.** Every product or service you sell, in the detail Pocket Agent needs to draft, quote, describe, and defend it.

The rule: real ranges, real scopes, real what's-not-included. If the price is a range because the scope varies, put the range. If a feature is in Tier 2 but not Tier 1, say that. If a customer asks whether X is included, your agent should be able to answer from this zone alone.

## What goes in here

| File | What it captures |
| :--- | :--- |
| `example-feature-inventory.md` | The canonical registry of what's built, what's in flight, what's blocked. The "have we shipped X yet?" file. |
| `example-flagship-product.md` | One product spec in full detail. Scope, deliverables, pricing, delivery, guarantee, upsells. |
| `example-pricing-tiers.md` | Good / Better / Best (or however you actually sell). Named tiers, real prices, real distinguishers. |
| `example-change-log.md` | Ship-by-ship record of what changed. Append-only. |

Add files as you add products. If you sell three distinct products, you have three product-detail files. If you sell one thing with three delivery tiers, you have one product file and one pricing-tiers file.

## What NOT to put here

- **Live customer names in product examples.** Products describe what you sell to *anyone*. Customer specifics live in `customers/`.
- **In-flight pricing experiments you haven't decided on.** Put those in `decisions/` as an open decision, promote to `products/` when locked.
- **Marketing copy.** This zone is the source of truth Pocket Agent reads to write the marketing copy. Never the other way around.

## How to fill this out

The four example files ship pre-filled with a composite operator business — a custom-CRM-build service, blurred but real in shape. Read the shape. Replace with your own products.

The rule Pocket Agent enforces when drafting: if a claim about a product isn't in this zone, it doesn't get made. No inventing features, no rounding a price, no "usually includes." Everything is on the record here or it doesn't ship in copy.
