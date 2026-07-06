# Cold email / customer setup email

**Use case:** Chase emailing a client (Patrick, future BOS / Hosted clients, post-sale prospects) to close out a setup phase, frame the next step, or confirm what's owed by whom.

**Source pattern:** Reconstructed from the user-described "Last setup push" Patrick email (Gmail draft v3, 2026-05-12) + `Discovery_Call_Followup_Flow.md` structural cadence + `BOS/Products/Patrick/Patrick_Daily_Log.md` correspondence references. The verbatim send-out copy isn't versioned in the brain — see `voice/audit.md` §G5. The structure below is the documented pattern; the body is a plausible reconstruction.

---

## On-brand (Chase)

> **Subject:** Last setup push.
>
> Patrick —
>
> Last setup push before we hand the keys over. Two lists below — yours and ours — and three things parked with the reason.
>
> **Yours**
> 1. Walk through `/settings/team` and add the two reps we discussed (Jordan + Mike). Auth invite emails go to whatever address you put in.
> 2. Send me the storm-vendor list you mentioned on Tuesday so I can wire the import. CSV with name + phone + service area is enough.
>
> **Together** (Thursday call, 9am ET)
> 1. Conclusion-templates review — confirm Amanda's set looks right against your snippets library.
> 2. Custom dashboard tile layout — pick the 3 you want above the fold.
>
> **Parked**
> - Solar API expansion → unparks after the FPHI roof-details migration lands on `origin/main`.
> - SMS round-robin → unparks once Twilio creds are rotated (waiting on you for the new keys).
> - Storm-event auto-routing → unparks when the HailTrace webhook handler is verified against a real payload.
>
> Reply with "yes Thursday" or push the call.
>
> — Chase

---

## Off-brand (generic AI)

> **Subject:** Following up on next steps for FPHI implementation
>
> Hi Patrick,
>
> I hope this email finds you well! I wanted to circle back regarding the last few items we discussed during our recent conversations. As we move forward toward the final handoff of your custom-built Buildout Studios operating system, I've put together a comprehensive overview of the remaining action items to ensure we're all aligned and ready to launch successfully.
>
> There are several things I'd love for you to take a look at when you get a chance, including some team member additions and a vendor list import that will help us round out the platform. Additionally, there are a few items that we should tackle together during our next touchpoint, and a handful of features that are still in progress and will be revisited at a later date as we continue to iterate.
>
> Please let me know what timeframe works best for your schedule, and feel free to reach out if you have any questions, concerns, or feedback. I'm always happy to hop on a quick call to discuss anything in more detail.
>
> Looking forward to wrapping this phase up soon!
>
> Best,
> Chase

---

## Why the on-brand version works

- **Names the email's job in sentence one.** "Last setup push before we hand the keys over." The reader knows what this is in seven words.
- **Specific tasks with named files / people / triggers.** `/settings/team`, Jordan + Mike, CSV format, Thursday 9am ET, Amanda's set, HailTrace webhook. Every line in the lists has a referent the client can act on.
- **Three lists do the work prose would have done in five paragraphs.** Yours / Together / Parked. Each list answers one question (what does Patrick own, what do they jointly own, what's deferred and why).
- **"Parked" items name the unpark trigger.** Not "we'll get to it" — every parked item has the specific upstream condition that unblocks it. The honesty is the asset.
- **Single-action CTA.** "Reply with 'yes Thursday' or push the call." One reply, one decision. No "let me know what works".
- **No padding.** No "I hope this finds you well", "circle back", "move forward", "looking forward to". The signature is initials, not the corporate flourish.
- **First-name greet, em-dash, lowercase opener.** "Patrick —" not "Dear Patrick,". The register is friend-at-coffee-table, not vendor-to-buyer.
