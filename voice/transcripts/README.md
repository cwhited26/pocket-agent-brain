# voice/transcripts/ — Raw transcripts for voice training

**Status:** Zone 1 sub-folder. Ships empty. Fill with your own.

This directory holds the highest-fidelity voice-training material in the brain: raw transcripts of **you** actually talking. Loom recordings, sales-call audio, voice memos through Whisper, podcast interviews where you're the guest. Anything where your real cadence, vocabulary, and rhythm are on record.

Spec authors read these to calibrate `voice-spec.md`. Future agents drafting new copy can read them as primary-source voice samples — closer to how you actually sound than any written artifact.

## What goes in this directory

- **Root (`voice/transcripts/`)** — transcripts where **Chase is the primary speaker**. His voice on record.
- **`_clients/`** — transcripts where **Chase is silent or secondary** (Patrick walks through his domain, a coach explains his playbook, a customer talks through their workflow). These are *negative controls* for Chase's voice — useful reference for client voices (Layer 2), but **don't train on these as Chase's voice**.

## Filename pattern

```
{YYYY-MM-DD}_{source}_{topic-slug}.md
```

Examples:
- `2026-05-15_loom_bos-sales-call-prep.md`
- `2026-05-20_voicememo_after-tve-customer-walkthrough.md`
- `2026-06-01_podcast-guest_smith-show-on-multi-agent-workflows.md`
- `_clients/2026-05-11_patrick-loom-walkthrough.md` (client voice, not Chase)

Use absolute dates, not relative. Slug is lowercase, hyphenated, descriptive enough to grep.

## Frontmatter

Every transcript file starts with a one-line frontmatter so agents know how to weight it:

```
> Source: {Loom recording / voice memo / sales call / podcast / etc.}
> Audience: {who Chase was talking to — APA member, BOS prospect, internal agent, podcast host, etc.}
> Register: {casual / sales-pitch / teaching / debugging / direct-feedback / etc.}
> Chase voice strength: {primary / secondary / silent}
> Length: {N min / approx N words}
```

Then the transcript body — verbatim, light cleanup (filler word removal optional; mark `[ums removed]` or similar if you cleaned).

## How to use a transcript

When calibrating the spec or drafting new copy:

1. Open a transcript that matches your target content type (e.g., a sales-call transcript before drafting a sales email).
2. Read three paragraphs out loud.
3. Note the cadence — short sentences, em-dash rate, named-thing vocabulary, what Chase says when he's hedging vs committing.
4. Draft against that cadence, not against the spec alone. The spec is the rule. The transcript is the rhythm.

If you find a pattern in the transcript that isn't captured in `voice-spec.md`, add it to the spec and cite the transcript in §12 source citations.

## Privacy

Transcripts may contain customer names, prospect details, internal numbers, and unsanitized financials. The whited-brain repo is private. **Don't quote a transcript in any public artifact without sanitizing** per `Whited_Consulting_Content_Strategy.md` §9 (sanitization rule). Sanitize names → "a roofing client" / "a youth sports org" / etc. before pulling a line into a sales page, blog post, or social.

## Adding a new transcript

1. Get a transcript file (Whisper-local for Loom audio, Otter/Granola/Fireflies export for calls, manual cleanup for short voice memos).
2. Save to `voice/transcripts/` (Chase-primary) or `voice/transcripts/_clients/` (client-primary).
3. Add the frontmatter block at the top.
4. If the transcript surfaces a new voice pattern not in the spec — add it to `voice-spec.md` (§2 cadence, §3 vocabulary, or §6 structural patterns as relevant) and cite the transcript in §12.

## Status at build time

The voice/ infrastructure was built before the first Chase-voice transcript was captured. The placeholder file `_AWAITING_FIRST_TRANSCRIPT.md` notes what would unlock the strongest first calibration: a 5–10 min raw Loom of Chase talking through a real BOS sales call, or a candid voice memo summarizing a discovery call. Once that lands, agents calibrating against the spec have a primary-source baseline instead of the spec alone.

One client-voice transcript exists in `_clients/` as a placeholder for the 2026-05-11 Patrick Loom walkthrough (Chase was silent; Patrick walked through his domain). Useful as a negative control — not as Chase's voice.
