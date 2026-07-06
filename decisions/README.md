# decisions/ — the calls you made and the rules you don't break

**This is Zone 5 of your Business Brain.** It's what Pocket Agent reads before it does anything material — draft an email, quote a price, ship a feature, respond to a customer.

Two kinds of file live here:

| File | What it captures |
| :--- | :--- |
| `decision-log.md` | Append-only ledger of every material decision you've made. Numbered, dated, rationale + alternatives considered. |
| `standing-rules.md` | Rules the agent reads BEFORE it drafts. The "you don't cross this line" set. |

The distinction: **decisions** are calls with a date attached — they can be superseded when new information arrives. **Standing rules** are the operating floor — they don't change without you saying so.

## The append-only law (hard)

**Never delete a decision.** Not the ones that turned out wrong. Not the ones that got superseded. Not the ones that are embarrassing in retrospect. The value of the log is that future-you can see the reasoning of past-you and know why things are the way they are.

When a decision gets reversed, add a new numbered entry that supersedes the old one. Both stay in the file. The old one gets a `Superseded by #N` marker. See `memory-conventions/supersession-pattern.md`.

## The rule for what counts as a "decision"

Not every call is a decision. A decision is worth logging when:

1. It has consequences that outlast the session.
2. Future-you (or a future agent) might ask "why did we do it this way?"
3. A different call would produce meaningfully different behavior downstream.

A decision is NOT: which shade of blue you picked in the header, whether Tuesday or Wednesday works better for the standing meeting, what you had for lunch. Log the calls that shape how the business runs, not the calls that shape today.

## Numbering

Decisions are numbered. Simple integer, incrementing. When you supersede one, the new entry gets a new number (never the old number). This is important — the log's power comes from every decision being addressable forever.

## Standing rules — the read-first list

`standing-rules.md` is what Pocket Agent reads BEFORE it drafts a customer message, a landing page, a follow-up. It's the fastest way to prevent a bot from doing something dumb in your voice.

The rules that live there are the ones you'd yell at a new hire for breaking. If a rule doesn't survive the "would you yell?" test, it's not standing — it's a preference.

## How to fill this out

`decision-log.md` ships pre-filled with 8 example decisions from a real operator business. Read them for shape. Then replace with your own real decisions. `standing-rules.md` ships with 12 default rules — read them, keep the ones that apply, edit the rest, add your own.

Both files are living. Update them the day something material happens.
