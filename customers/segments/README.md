# customers/segments/ — your top-N segments

**Purpose:** One file per real segment. Named. Ranked by share of your work. Written the way you'd describe them out loud to a friend.

Pocket Agent reads this before it drafts a campaign, a landing page, or a piece of outreach. When you tell it "write to my best segment," this is where it looks.

## What goes in a segment file

Each file at `customers/segments/<slug>.md` should carry:

1. **Name.** One short phrase you actually use. "Insurance restoration contractors doing $2-5M." "Coaches with a course but no funnel." "Ecom brands north of $500k where the founder still ships orders."
2. **Share of work.** Rough number. "~55% of the last 12 months of revenue."
3. **How they find you.** Real channels, not a list of "possibilities."
4. **What they buy.** Specific offering, real range.
5. **What they don't buy.** Where the misfit or the upsell lives.
6. **What they're afraid of when they contact you.** The fear, stated the way they'd state it.
7. **The one line that converts them.** Your best pitch, distilled.
8. **Best-fit flag.** `best-fit: true` on the segment your agent should default to when the operator says "my best customer." At most one file has this.

## Ranking convention

Order the segments by revenue share, highest first. Add a note at the top of segments beyond your top 3 explaining why you're keeping the file even though it's not a lot of revenue (referral engine, brand halo, learning ground for a new offering, etc.).

## The example file

`example-segment-a.md` ships as a working example. Read it once. Replace with your own.
