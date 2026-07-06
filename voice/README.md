# voice/ — your voice infrastructure

**This is Zone 1 of your Business Brain.** It's the canonical home for your voice spec, voice-training transcripts, and paired on-brand vs off-brand examples. It exists so every agent working in this brain — Pocket Agent, Claude Code, any downstream tool — auto-loads your voice when drafting copy and produces output that sounds like *you* on the first pass, not after three rounds of correction.

Voice lives native to the brain, alongside `CLAUDE.md` and `AGENTS.md`, because the brain is where you keep the rules of how work happens. Don't outsource voice to a separate plugin or a prompt library — keep it here, versioned, editable, yours.

## Layers

- **Layer 1 — Your voice spec (this directory).** Single canonical voice for you. Files: `voice-spec.md`, `audit.md`, `examples/`, `transcripts/`.
- **Layer 2 — Personas (optional, not yet built).** Voices you sometimes speak *in* but that aren't yours: a client's voice, a stakeholder's voice, a rep's voice. Lives under `voice/personas/` when you need it.
- **Layer 3 — Influences library.** Operators you model for sales / funnel / copy / ad patterns. **Techniques are prescribed moves**; **only branded framework labels stay out** (write the technique in plain English). Library index: `voice/influences/README.md`. Composition rule: voice from Layer 1 + structural patterns from Layer 3; never one without the other.

## Files in this directory

| File | What it is | When to read |
| :--- | :--- | :--- |
| `voice-spec.md` | The canonical voice spec. Load this first before drafting any external copy. | Before every draft of an email, drip, community post, landing page, video script, sales asset, internal task brief, or customer follow-up. |
| `audit.md` | Working ledger of source artifacts the spec is grounded in. Read this if you want to verify a claim in the spec back to its source. | When in doubt about whether a spec rule is grounded vs extrapolated. |
| `examples/` | Paired on-brand vs off-brand artifacts with diagnostics. Cross-check a draft against these before sending. | After drafting, before sending. Pick the example that matches your content type. |
| `transcripts/` | Raw transcripts of you talking (Loom recordings, sales calls, voice memos, podcast guesting). Voice-training material. | Read when calibrating the spec — your actual cadence in audio is the highest-fidelity signal. |
| `influences/` | Operators you model for structural sales-copy patterns (Brunson, Hormozi, etc). | When reaching for a value stack, an anchor, an OTO, a bump — pattern in from here, voice in from `voice-spec.md`. |

## How to use this in a session

1. **Before drafting any external copy:** open `voice-spec.md`. Calibrate against §10 (the calibration cues) once before you start and once before you send.
2. **When in doubt about a rule:** trace it back through `audit.md` to the source artifact. The spec doesn't invent rules — every line cites a source.
3. **When stuck:** open `examples/[content-type].md` and rewrite your draft against the paired on-brand/off-brand pair.
4. **When you have a new artifact you wrote or approved:** add it to `examples/` (graduating it from "constructed" to "verbatim") and update `voice-spec.md` §12 source citations.

## When to *not* use this spec

Three explicit override cases, captured in `voice-spec.md` §11:

1. **Client-voice override.** You are writing in a client's or stakeholder's voice — use their voice (Layer 2 when built; artifacts in the brain as fallback).
2. **Domain-precision override.** Technical specs, ADRs, migration plans — voice tunes toward precision; spec still rules out banned phrases.
3. **Direct operator request.** If you say "make this corporate for legal" / "write a literal Twitter thread," follow the instruction.

Outside these three, the spec is the floor.

## Getting started

The `voice-spec.md` file ships pre-filled with Chase Whited's actual voice spec — the one running Pocket Agent, Buildout Studios, and Tennessee Valley Exteriors right now. It's a working example, not a scaffold. Read it end-to-end. Then edit it to be **yours**. Every mention of "Chase," "Patrick," a specific product or a specific customer is a placeholder for your own reality. Keep the structure and the calibration cues (§10) — those are the point.

## Updating

Update protocol lives in `voice-spec.md` §13. Don't update this README or the spec without checking the protocol first.
