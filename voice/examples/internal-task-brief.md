# Internal task brief / lane prompt

**Use case:** Chase writing a lane prompt to a Claude Code / Codex / Dispatch sub-agent. Verbatim instruction, scoped, with explicit success criteria and standing-rule pointers.

**Source pattern:** This file is itself the on-brand example — Chase's voice-build prompt that kicked off the work creating this voice/ directory on 2026-05-12. That prompt is the canonical reference for what a Chase-written lane brief looks like. Dispatch Playbook §6 "How to write a clean lane prompt" (`APA/Products/Dispatch_Playbook_Draft.md` lines 203–234) is the locked written rule-set for the same pattern.

---

## On-brand (Chase)

> Build out the `voice/` infrastructure in whited-brain as a first-class brain surface. Layer 1 only — consolidated voice spec for Chase + transcript intake + examples + CLAUDE.md wiring. Personas (Layer 2) and influences library (Layer 3) are deliberately out of scope.
>
> **Goal:** every agent working in any whited-brain-anchored repo (whited-brain itself, Patrick's FPHI build, AOS, BOS website, APA, wc-admin, aipocketagency-website) auto-loads Chase's voice spec when drafting any copy — emails, drips, Skool posts, landing pages, video scripts, sales assets — and produces output that sounds like Chase the first time, not after 3 rounds of correction.
>
> **Standing rules (read first):**
> - `/Users/chasewhited/whited-brain/CLAUDE.md` for full project rules
> - All memory files under `/Users/chasewhited/Library/Application Support/Claude/local-agent-mode-sessions/.../memory/` for behavior conventions
>
> ---
>
> ## Phase 1 — Audit existing voice signals
>
> Grep through whited-brain and the agent memory directory for everything that's already implicit voice spec. Specific files and patterns to mine:
> [...]
>
> ## Phase 5 — Wire into CLAUDE.md
>
> Edit `/Users/chasewhited/whited-brain/CLAUDE.md`:
>
> 1. Add to **Section 12 Behavior Rules** a new rule (probably #10 or #11): "When drafting any customer-facing or external copy, load `voice/voice-spec.md` first..."
>
> [...]
>
> ## Report
>
> When done, surface:
> 1. SHA of the brain commit
> 2. Path to `voice/voice-spec.md` + word count
> [...]
> 8. Honest gaps — what's in the spec that's a placeholder vs grounded in real audit findings (be ruthlessly honest — if you had to invent a section because the audit didn't surface enough data, flag it so Chase can fill it in)

---

## Off-brand (generic AI)

> Hi there,
>
> I'd like your help setting up a voice infrastructure system for my various projects. This is an important initiative that will help streamline our content creation process across multiple platforms and ensure consistency in how we communicate with our audience.
>
> Please proceed with the following:
> - Take a look at the existing materials we have in the repository
> - Create appropriate documentation that captures the brand voice
> - Set up a folder structure that makes sense
> - Add some examples to help guide future work
> - Make sure to follow best practices throughout
>
> Let me know if you have any questions before getting started! Once you've completed the work, please provide a summary of what you've done so we can review together. Thanks so much for your help with this — really appreciate it!

---

## Why the on-brand version works

- **Verb-first directive.** "Build out the `voice/` infrastructure…" — the verb is the first word. The agent knows the action before it knows anything else.
- **Concrete scope locked early.** "Layer 1 only — consolidated voice spec for Chase + transcript intake + examples + CLAUDE.md wiring. Personas (Layer 2) and influences library (Layer 3) are deliberately out of scope." Three named layers, scope of this prompt locked to one. No drift.
- **Goal stated in operator terms.** "Sounds like Chase the first time, not after 3 rounds of correction." The success metric is observable and binary, not a feeling.
- **Standing rules linked by path.** `/Users/chasewhited/whited-brain/CLAUDE.md` — paste the path, not "the project rules". The agent doesn't have to guess what `CLAUDE.md` means in context.
- **Phased structure with explicit deliverables.** Each phase has a clear output (audit doc, spec doc, examples, CLAUDE.md edits, memory file). The agent grades its own paper against the phase list.
- **Honest-gaps clause at the end.** "Be ruthlessly honest — if you had to invent a section because the audit didn't surface enough data, flag it so Chase can fill it in." Explicit permission to admit limits. This is the anti-hallucination instruction.
- **Closing report format named.** Eight enumerated items the agent must surface when done. The orchestrator can verify each one independently. No "let me know if you have any questions before getting started" — that's reverse delegation.
- **No "thanks so much" / "really appreciate it" / "hi there" softeners.** The register is direct. The agent isn't being asked to perform service-tone — it's being given a brief.
