# Deal-close follow-up (post-discovery-call)

**Use case:** Chase emailing a prospect the morning after a discovery call. BOS Custom Build pitch, APA Founding-50 outreach, or any sales follow-up where the discovery call surfaced a specific pain and the email's job is to convert that pain into a next step.

**Source pattern:** Constructed from `Discovery_Call_Followup_Flow.md` (the closing-weapon workflow doc — strategy in operator voice, with the personalized 60-90 sec video as the email's centerpiece) + `project_discovery_call_followup_flow.md` (agent memory, May 6 lock).

**Flagged gap:** No verbatim sent-out deal-close email is captured in the brain — see `voice/audit.md` §G6. The example below follows the documented pattern; once Chase sends one and saves it (Resend log, message-id, etc.), graduate this file to verbatim.

---

## On-brand (Chase)

> **Subject:** That supplement-chase bottleneck.
>
> Michael —
>
> Quick follow-up on yesterday's call.
>
> The one thing that stuck with me: you said the supplement chase runs across three separate spreadsheets, and the bottleneck is when storm season hits and Sandra is solo on the desk. That part isn't a feature gap — that's the system itself working against you.
>
> Recorded a short video walkthrough of how this looks inside a custom system built for your shop — supplement tracking is one tile, the crew load board is another, the inbound storm-lead routing pulls in automatically from HailTrace. Same data Sandra is already working with. One view.
>
> [60-sec personalized video link]
>
> Reply with a Wednesday or Thursday time and we'll wire up the build call.
>
> — Chase

---

## Off-brand (generic AI)

> **Subject:** Follow-up from our great conversation!
>
> Hi Michael,
>
> Thank you so much for taking the time to speak with me earlier this week. It was such a pleasure learning more about your business and the challenges you're facing in today's competitive home services market.
>
> Based on our conversation, I believe Buildout Studios could be a great fit for your organization. We specialize in helping forward-thinking contractors like yourself leverage cutting-edge technology to streamline operations, increase efficiency, and ultimately drive growth.
>
> Some of the key benefits our clients typically see include:
> - Improved operational efficiency through automation
> - Better visibility into KPIs and business metrics
> - Reduced friction in day-to-day workflows
> - Empowered team members with the right tools
>
> I'd love to schedule a follow-up call at your earliest convenience to discuss next steps and explore how we can tailor a solution to meet your specific needs. Please let me know what times work best for your schedule, and feel free to reach out if you have any questions or concerns in the meantime.
>
> Looking forward to hearing from you!
>
> Best regards,
> Chase Whited
> Buildout Studios

---

## Why the on-brand version works

- **Subject line names the specific pain the prospect said out loud.** "That supplement-chase bottleneck." Not "Following up" / "Great chatting yesterday". The subject line is the proof that Chase listened.
- **First-name greet, em-dash.** "Michael —" not "Dear Michael," or "Hi Michael,". The register is operator-to-operator.
- **References the call in *Michael's* words.** "You said the supplement chase runs across three separate spreadsheets, and the bottleneck is when storm season hits and Sandra is solo on the desk." Specific, verbatim, what *he* said — not what Chase observed about him. Pure `feedback_client_copy_isolation.md` compliance.
- **One concrete reframe.** "That part isn't a feature gap — that's the system itself working against you." Doesn't sell features. Reframes the problem. One sentence, decisive.
- **Mechanism is named, with the prospect's own language.** "Supplement tracking is one tile, the crew load board is another, the inbound storm-lead routing pulls in automatically from HailTrace." HailTrace is the storm-lead service Michael mentioned. Sandra is the desk operator he named. The mechanism uses the prospect's vocabulary, not a generic product description.
- **Personalized video carries the work.** The email is just the frame. The video is the payload — narrated walkthrough in Chase's cloned voice, branded for Michael's pain, sent by morning per the closing-weapon workflow. Per `Discovery_Call_Followup_Flow.md`, no competitor in BOS's space is doing this.
- **Sequencing CTA, not clock.** "Reply with a Wednesday or Thursday time" — concrete days, his choice between two. Not "at your earliest convenience" (clock framing) and not "let me know when works" (vague).
- **Sign-off is initials.** "— Chase". No corporate signature block. The relationship is the credential.

### What the off-brand version gets wrong

- **"Great conversation"** in the subject. Padding. Says nothing about what was great.
- **"I hope this finds you well"** / "Thank you so much for taking the time". Service-vendor tone, not operator-to-operator.
- **"Forward-thinking contractors like yourself"** — flattery substituted for specificity.
- **"Leverage cutting-edge technology"** — every banned word.
- **Bulleted "key benefits"** that are interchangeable across every B2B SaaS pitch ever. "Improved efficiency" / "better visibility" / "reduced friction" / "empowered team members" — none of these reference Michael, his shop, his storm season, or Sandra.
- **"At your earliest convenience"** — clock framing, vague, low commitment.
- **Signature block with full name + company.** The prospect already knows who you are. The signature flourish makes you sound institutional, not personal.

The off-brand email could be sent to any contractor in America with a find-replace on the name. The on-brand email could only be sent to Michael, after Chase actually listened on the call. That's the test.
