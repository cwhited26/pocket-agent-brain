# customers/ — who buys from you

**This is Zone 2 of your Business Brain.** It's the read-only reference every agent hits when it needs to know the person on the other end. Not a persona doc invented from thin air — real customers, real texture, real language they use.

Pocket Agent reads this before it drafts anything customer-facing. If it's drafting a follow-up to Alice, it reads Alice's file. If it's drafting a cold email to a lead who looks like your best segment, it reads the segment file. If you tell it to "write to my ideal customer," it reads the segment marked `best-fit: true`.

## What goes in here

| Kind of file | What it captures |
| :--- | :--- |
| **Individual customer profiles** — one file per person, or per household in service businesses | Their real language, what they bought, what they didn't, what they're afraid of, who referred them, how they pay. |
| **Segments** — one file per customer segment (`segments/`) | Who they are, how they find you, what they need to hear, what share of your work they are. |
| **Anti-personas** — one file per "not my customer" | The buyer who takes 3× the time for 1/2 the money. Named, so nobody sells to them by mistake. |

## The privacy rule (hard)

**Customer names never appear in public copy without the customer's explicit permission.** This is a standing rule you'll find in `decisions/standing-rules.md`. Files in this zone can carry real names because the zone is private to your brain repo. Anything Pocket Agent drafts that references a customer strips the name unless the customer said "yes, use my name."

For sensitive segments (medical, legal, finance, minors), use initials or codenames even in the brain files. If a file feels too spicy to have on a laptop screen at a coffee shop, use a codename.

## How to fill this out

The three example files below ship pre-filled with composite customers (names blurred). They're modelled on real customer profiles from three actual businesses running on Pocket Agent right now. Read them once to see what the depth looks like. Then replace with your own.

The rule: real over pretty. A messy true customer profile beats a clean generic one every time.

## Files in this directory

- `example-active-customer.md` — composite of a current customer with a full profile
- `example-past-customer.md` — composite of a closed / referral-source customer
- `example-not-a-fit.md` — composite of a buyer who is NOT your customer
- `segments/` — one file per segment, plus a segments README

## When a customer graduates

- **Active → Past.** When the work closes. Add a "how it ended" section, keep the file.
- **Past → Referral source.** When they send you someone. Add a "referred us to" list at the bottom.
- **Anywhere → Not-a-fit.** When the work is done and the answer is "never again for this reason." Move the file to a `not-a-fit/` sub-folder (or just relabel) and add a "why not again" section — that's the signal your ICP filter should catch.

Nothing is deleted. Customers are the highest-value memory in your brain. Keep them all.
