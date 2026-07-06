# voice/audit.md — Voice signal audit

**Status:** Working example — replace with your own.
**About this file:** This ships pre-filled with the source audit behind Chase Whited's voice spec (see `voice-spec.md`). It's here as a **working example** of what a real audit looks like — sources cited, signal strength graded, gaps flagged honestly. Read it once. Then replace it with your own audit as you build your voice spec: which artifacts of yours are the strongest signal (voice memos, sales calls, past emails, published writing), which sections of the spec extrapolate beyond them, which gaps you know are open.

The rule: if a line in your voice spec doesn't trace back to a source in this file, it's an assumption, not a rule. Spec authors update the spec; they do not rewrite this audit. Add new sources to §A or §C as they land.

---

## Sources scanned

| Source | Path | Voice signal strength |
| :--- | :--- | :--- |
| Master content rules | `Whited_Consulting_Content_Strategy.md` §1 | **HIGHEST — Chase's own meta-rules** |
| Long-form locked sample | `APA/Products/Dispatch_Playbook_Draft.md` §1–11 | **HIGHEST — first-person locked voice target** |
| Locked product copy | `Skool_Launch_Plan.md` §6 (Sales page copy lock) | **HIGHEST — compressed voice** |
| Recorded narration scripts | `Skool_Module_1_Scripts.md` | HIGHEST — conversational teaching |
| Closing-weapon workflow doc | `Discovery_Call_Followup_Flow.md` | High — strategy in operator voice |
| Hard rule (agent memory) | `feedback_no_time_estimates.md` | High — banned constructions |
| Hard rule (agent memory) | `feedback_no_session_endings.md` | High — banned constructions |
| Hard rule (agent memory) | `feedback_client_copy_isolation.md` | High — honesty rule |
| Standing rule (agent memory) | `feedback_invented_details_ok.md` | Medium — calibration note |
| Standing rule (agent memory) | `feedback_handle_everything_yourself.md` | Low — workflow, not voice |
| Standing rule (agent memory) | `feedback_manual_step_by_step.md` | Low — UX not prose |
| Brand context | `Whited_Consulting_Brand_Architecture.md` | Medium — sub-brand positioning |
| Brand context | `MEMORY.md` (brain root) | Medium — APA-7..14 locks, monospace-pill convention |
| Client domain capture (parallel) | `BOS/Products/Patrick/Patrick_Snippets_Library.md` | Medium — shows the caliber of specificity Chase respects, not Chase's voice |

---

## A. Hard-banned constructions (with source)

| Construction | Source | Rule |
| :--- | :--- | :--- |
| Time estimates of any kind ("~5 min", "quickly", "in a moment", "shortly", "should land in a few", "I'll have this in ~3 prompts") | `feedback_no_time_estimates.md` lines 9–14 | Replace with sequencing or absolute dates. |
| Session-ending framing ("we can pick it up tomorrow", "end of session", "good place to pause", "want to keep going or call it for the day") | `feedback_no_session_endings.md` lines 7–18 | Default to forward motion. Present the next decision; don't offer time-shifted alternatives. |
| Conflating internal observations with client experience ("the issue you saw") | `feedback_client_copy_isolation.md` lines 7–12 | Only reference what the client themselves said/saw. |
| "Let's dive in" / "In this video we will explore" / "I'm so excited to share" / "Smash subscribe" / "Buckle up" | Content Strategy §1 line 15 | Guru framing. Killed. |
| "$10k MRR in 30 days" / "I made $X last month" / "The secret nobody's telling you" | Content Strategy §1 line 16 | Fake urgency / bro-marketing. Killed. |
| "DM me 'BRAIN' for the playbook" / "Comment below if you want the link" | Content Strategy §1 line 18 | Bait. Don't gate links. |
| "Top 10 AI tools for X" / "Hot take: every agency will be dead in X months" / "Just had a great call with a major client" | Content Strategy §5 kill list (lines 107–115), §6 anti-patterns (lines 121–132) | Listicle / vague-flex content. Killed. |
| Empty padding ("genuinely", "honestly", "straightforward" as filler) | System tone rule + absent from all samples | Cut. |
| Predictive ETAs on agent work | `feedback_no_time_estimates.md` line 14 | Replace with sequencing. |

---

## B. Direct quotes — Chase's own voice rule

From `Whited_Consulting_Content_Strategy.md` §1 (verbatim):

> **Operator voice.** Chase is an operator who learned to build software because the work demanded it — not a guru, not a coach, not a "tech founder." Every piece of public content reads like advice you'd give a friend at a coffee table.

> Specific over abstract. "Patrick paid $3,500 + monthly hosting" beats "I help contractors run real businesses."

> Real numbers, real names, real outcomes. If it can't be sourced to a SHA, a commit, a customer, or a date — it doesn't go in the post.

> Short over long when long doesn't earn it. A 60-word X post beats a 600-word LinkedIn humblebrag.

> If a draft starts to drift, run the rewrite test: would Chase actually say this sentence out loud to a friend? If no, kill it.

---

## C. Verbatim on-brand passages (with file + line refs)

### C1 — Dispatch Playbook §1 opener (the locked long-form voice)
**`APA/Products/Dispatch_Playbook_Draft.md` lines 12–18**

> Single-thread Claude Code is one conversation, one context window, one agent doing one thing at a time. When the context fills up — and it always fills up — you start over.
>
> That's the wall. You can be productive inside one chat for a couple hours. After that the agent starts losing track of what it already decided, you start re-pasting paragraphs from earlier, the work slows down, you hit auto-compaction and lose the thread anyway. Single-thread works fine for tight, contained tasks. It breaks the moment your day involves more than one moving piece.
>
> Dispatch is the orchestrator that spawns sub-agents in parallel. Each sub-agent has its own context window, focused on one task. You stay in the main thread. They go off and work. They report back. You decide what to do with the result.

### C2 — Felt experience anchor
**`APA/Products/Dispatch_Playbook_Draft.md` line 18**

> The actual unlock isn't raw speed. It's that you stop *watching* one agent. Watching a single agent type for ten minutes is the worst kind of work — too engaged to do anything else, not engaged enough to feel like you're producing. Spawn four lanes, each one finishes on its own timeline, you check back when they have something to show. **That's the difference between babysitting and orchestrating.**

### C3 — Honest naming of the fear
**`APA/Products/Dispatch_Playbook_Draft.md` lines 30–32**

> Here's the fear, stated honestly. Four agents are running at the same time. They all have write access to your codebase. You can't watch every keystroke. What if one writes a bug? What if two of them edit the same file? What if one decides to refactor something you didn't ask for and pushes it to main while you're not looking?
>
> That fear isn't crazy. I had it too. The first time I ran four lanes I sat there refreshing GitHub like a maniac.

### C4 — Compressed positioning copy
**`Skool_Launch_Plan.md` lines 97–99**

> **Headline:** Run an AI agency from your pocket.
>
> **Subheadline:** Get the AI brain that makes it possible — the system I use to run real software businesses from anywhere, with any agent.

### C5 — Anti-guru product framing
**`Skool_Launch_Plan.md` lines 104–105**

> **Anti-guru section:**
> Tired of $47 AI courses that teach you how to ask Claude better questions? So am I. This isn't a course. It isn't a prompt pack. It's the actual system — the AI brain — that I run my own businesses on. You get the structure, the conventions, the workflows, and the live builds. Platform-agnostic. Model-agnostic. If the agent landscape shifts tomorrow, your AI brain still works.

### C6 — Strategy doc opening (BOS)
**`Discovery_Call_Followup_Flow.md` lines 5–7**

> ## The pitch
>
> Most agencies follow up a discovery call with a template proposal or email recap. Chase sends a 60-90 sec personalized video — narrated in his cloned voice, showing a walkthrough tailored to that prospect's situation — by morning. No competitor in BOS's space is doing this. Differentiator that compounds across every call.

### C7 — Verification-discipline ending (the anti-hype close)
**`APA/Products/Dispatch_Playbook_Draft.md` line 401**

> If you can read these eleven sections and still feel scared, run a fan-out of three lanes on something low-stakes — rename a variable across three files in a small repo, or write three small markdown notes in a doc repo — and watch them work. Confidence here is hands-on, not theoretical. The first clean four-lane day is the day you stop being scared, and there is no shortcut to it. The playbook is the map. The clean four-lane day is the territory.

---

## D. Structural patterns observed

1. **Opens with the problem, not the promise.** Dispatch §1 opens "Single-thread Claude Code is one conversation, one context window…" — not "Here's how to ship 4x faster." Discovery doc opens with "Most agencies follow up a discovery call with a template proposal…" — frames the contrast first.

2. **Pairs declarative claim with mechanism.** "Run an AI agency from your pocket" (outcome) + "Get the AI brain that makes it possible — the system I use to run real software businesses from anywhere" (mechanism + proof of use). Never promise without showing the work.

3. **Felt-experience metaphor before mechanism.** "Watching a single agent type for ten minutes is the worst kind of work — too engaged to do anything else, not engaged enough to feel like you're producing." Then: "Spawn four lanes." The emotional anchor comes first.

4. **Names concepts decisively and repeats them.** "The wall." "Babysitting vs orchestrating." "Worktrees." "Standing rules." "Lane self-report vs disk-verified vs remote-verified vs behavior-verified." No synonym-switching. The named thing is the thing.

5. **Uses numbered lists for sequence, prose for explanation.** Discovery-Call Flow uses 9-step numbered list for the automated loop. Dispatch §3 uses prose for the 3-tier task model but bullets when listing worked examples.

6. **Anti-hype ending / reality check.** Module 1 close: "There is no SaaS to log into. There is no dashboard. The repo on disk is the entire product." Dispatch close: "Confidence here is hands-on, not theoretical." No padded summary. No "in conclusion."

7. **Em-dash for asides + named-thing emphasis.** "the context fills up — and it always fills up — you start over." Used for parenthetical clarification or rhythm, not as decoration. System tone rule says "avoid overusing em dashes" — Chase uses them but the rate is calibrated, ~1–2 per paragraph max.

8. **Bold sparingly, for turning-point concepts.** "**That's the wall.**" "**That's the difference between babysitting and orchestrating.**" Not decorative. Each bold anchors a mental model.

9. **First-person without ego.** "I had it too. The first time I ran four lanes I sat there refreshing GitHub like a maniac." Personal but credible — admitting the same fear the reader has.

10. **Concrete numbers, anonymized only when necessary.** "About three hours of back-and-forth" — specific. "Four lanes reported back inside an hour" — specific. When sanitizing for public, follow Content Strategy §9: "a roofing client" not "Patrick / FPHI" unless permission given.

---

## E. Vocabulary inventory (positive register, recurring)

| Word / phrase | Use | Example |
| :--- | :--- | :--- |
| **the wall** | Named blocker / honest limit | "That's the wall." |
| **babysitting vs orchestrating** | Core orchestration metaphor | "That's the difference between babysitting and orchestrating." |
| **shipped / shipping** | Proof. Past tense, verified. | "We don't tell people what's possible — we show what we shipped." |
| **real numbers / real names / real outcomes / real receipts** | Anti-hype specificity bar | "If it can't be sourced to a SHA, a commit, a customer, or a date…" |
| **specific over abstract / concrete** | Compression bar | "Specific over abstract. 'Patrick paid $3,500 + monthly hosting'…" |
| **the work** | Neutral, grounded effort | "The work moves to the front (the prompt) and the back (the verify)." |
| **running** (businesses) | Operational stance | "the system I use to run real software businesses from anywhere" |
| **in practice** | Bridge from rule to reality | "What that means in practice: [specific list]" |
| **stated honestly** / **honest answer** | Opens a candid section | "Here's the fear, stated honestly." |
| **pattern** / **rhythm** / **discipline** | Repeatable structure language | "Verification discipline" / "rebase rhythm" / "the pattern is exactly what fast recognition is for" |
| **blocker** | Technical obstacle (not "challenge") | "A conflict at session start means main moved in a way that clashes…" |
| **lane / fan-out / sequential dependency / watch-and-merge** | Parallel-orchestration vocabulary | "This is a three-lane fan-out, no shared files." |
| **standing rule / standing file** | Codified guidance | "Drop a one-liner that points at the relevant brain memory entry…" |
| **kill it / cut** | Rejection vocabulary | "If no, kill it." |
| **bake the answer into the prompt** | Operational metaphor | "Don't make the lane figure out the auth dance from scratch on every run. Bake the answer into the prompt." |

---

## F. Anti-pattern words / phrases (absent from Chase's writing)

- "Excited", "amazing", "awesome" — never as a generic intensifier.
- "Genuinely", "honestly", "straightforward" — banned as filler modifiers per system tone rule (Chase does say "honest" when it precedes a candid statement, e.g. "the honest answer is" — that's not the banned pattern).
- "Probably", "likely", "might want to consider" — hedge language. When Chase qualifies, he says "in practice" or "usually" — not modal hedges.
- "Help you", "empower you", "unlock your potential" — hollow benefit speak.
- "Revolutionary", "game-changing", "next-level" — marketing fluff.
- "Best practice", "industry-leading", "world-class" — corporate-deck noise.
- "Circle back", "synergy", "leverage" (as a verb) — corporate-speak. Chase says "use", "fold in", "tie together".
- "I hope this finds you well", "moving forward" — email padding. Never appears.

---

## G. Honest gaps where the audit thinned out

Flagged so future spec readers know what's grounded vs what's been extrapolated.

1. **Customer email tone (warm-context).** Strong samples for sales-page / playbook / strategy-doc voice. No verbatim Chase-written cold or follow-up email captured in the brain. Patrick correspondence references exist (`Patrick_Daily_Log.md` mentions message IDs) but the actual email bodies aren't versioned in the brain repo. **Implication:** the cold-email example pulls from the closest analogues (Discovery_Call_Followup_Flow framing + Content Strategy §1 voice rule) and the user prompt's reference to a "Last setup push" Gmail draft v3. The example is plausible but not a verbatim Chase artifact.

2. **Real-time chat / Slack register.** No captured Slack threads or live-chat samples. The agent-memory feedback corrections (e.g. "Stop telling me…") are the closest signal — Chase is direct, low-word-count, no padding when in real-time. Spec extrapolates this register from those corrections plus the locked long-form voice — but the calibration may be off.

3. **Drip email body.** APA drip-email sequences aren't fully drafted in the brain yet. `APA/Skool_Launch_Plan.md` and `APA/Recurring_Session_Scripts.md` capture cadence and live-session framing but not drip body copy. The drip example in `voice/examples/drip-email.md` is constructed from Dispatch §1 voice + APA positioning, not a verbatim sample.

4. **Deployed landing-hero rewrite SHA `ad9dc06`.** The bos-website rewrite referenced in the user prompt lives in a different repo (`bos-website`, not `whited-brain`). The audit does not include verbatim hero copy from that deployment. The landing-hero example uses the verified Skool launch headline+subheadline (which is in the brain) and notes that the bos-website hero would be the parallel BOS example if/when captured.

5. **Patrick "Last setup push" email (Gmail draft v3).** Referenced by the user prompt as the on-brand cold-email source. Not accessible from inside the brain repo (Gmail isn't in scope). The cold-email example reconstructs the intended structure from the Discovery_Call_Followup_Flow framing + Chase's correspondence patterns in `Patrick_Daily_Log.md` + the user prompt's described structure (greet → frame the ask → solo list → joint list → deferred items → close with single-action CTA).

6. **Deal-close follow-up body.** Pattern exists at `project_discovery_call_followup_flow.md` (agent memory) and `Discovery_Call_Followup_Flow.md` (brain). Neither captures verbatim send-out copy. The deal-close example is constructed from the documented pattern, not a sent email.

---

## H. Synthesis priorities for the spec

The spec at `voice/voice-spec.md` is grounded primarily in:

1. **Voice rule meta-doc** — `Whited_Consulting_Content_Strategy.md` §1 (Chase's own meta-rules; canonical anchor)
2. **Long-form locked sample** — Dispatch Playbook §1–11 (the voice target for teaching content)
3. **Compressed locked sample** — Skool Launch §6 (the voice target for sales copy)
4. **Hard rules from agent memory** — `feedback_no_time_estimates.md`, `feedback_no_session_endings.md`, `feedback_client_copy_isolation.md`

The spec explicitly does not invent rules outside these sources. Where a rule appears in the spec without a citation in this audit, treat it as extrapolation and flag for Chase review.
