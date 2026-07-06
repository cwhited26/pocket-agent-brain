# Standing Rules — what Pocket Agent (and every human) reads before drafting anything

**Every rule below is the operating floor.** Read this file before you draft. Read it before you quote. Read it before you reply to a customer. If a rule doesn't make sense to you when you first read this file, keep it anyway until you understand it — most of these were written after a specific mistake.

**Ships with 12 defaults from a real operator business. Edit them, add your own, delete the ones that don't fit.**

---

## Customer & communication rules

1. **Never use a real customer's name in public copy without their explicit permission.** Composite examples fine. Real names get one round of approval each. This is not paranoia — this is why customers trust us with the actual business.

2. **Never quote a real dollar figure from a live deal in public.** Ranges are fine ("$2,500 - $6,000"). Post-mortems on closed deals are fine with the customer's blessing. Live deals stay private.

3. **Never send anything after 8pm on a customer's local clock.** Draft it, sit on it, send it at 7am. The only exception is when the customer has explicitly said "text me anytime."

4. **Never write "just following up" without saying why you're following up.** If there's no reason, don't send it. If there's a reason, name it: "following up on the SRA question you asked Tuesday."

5. **Never promise a timeline the operator hasn't confirmed.** No "should ship this week" from an agent. Real dates or "we'll confirm once scope is locked."

---

## Money rules

6. **Never work on a deal without a signed scope and a cleared deposit.** See `decisions/decision-log.md` #1. Every "I'll pay you right after you start" turns into a scope debate.

7. **Never quote a price without a real scope attached.** If someone asks "what would this cost?" without a scope, the answer is "let me get on a call and scope it — should take 20 minutes."

8. **Never take equity in lieu of cash.** See `customers/example-not-a-fit.md`. Equity is not currency for us.

9. **Never discount below Standard-tier pricing.** If they can't afford Standard, they're not a customer yet.

---

## Voice rules

10. **Never use these words in customer copy:** "leverage," "unlock," "seamless," "streamline," "empower," "revolutionary," "game-changing," "cutting-edge," "world-class," "industry-leading." They're marketing register we don't operate in. See `voice/voice-spec.md` §3 for the full list.

11. **Never open a customer email with "Hi [name], I hope this finds you well."** Ever. First-name greet or straight-to-the-ask. See `voice/examples/cold-email.md`.

12. **Never pad a message with a summary at the end.** "In summary" / "hopefully this helps" / "let me know if you have questions" — cut all three. End on the last fact or the next decision.

---

## Feature / product rules

13. **Never invent a testimonial.** Real ones or none.

14. **Never claim a feature is "included" when it's Team-tier-only.** Read `products/example-pricing-tiers.md` before drafting anything scope-adjacent.

15. **Never promise an integration we haven't shipped.** The list of shipped integrations lives in `products/example-feature-inventory.md`. If it's not there, it doesn't exist yet.

---

## Data & privacy rules

16. **Never store secrets in this repo.** No API keys, no passwords, no tokens. Reference env var names only. Secrets belong in your password manager.

17. **Never paste a customer's data in this repo.** Composites and blurred examples are fine. Real records stay in the customer's own CRM.

18. **Never send a customer's information to a third-party tool without their explicit permission.** This includes uploading their data to a "helpful" AI service. Especially includes that.

---

## Meta rules

19. **Never delete a rule from this file.** If a rule is no longer active, mark it superseded with a date and a pointer to the decision that changed it. See `memory-conventions/supersession-pattern.md`.

20. **When you break a rule for a real reason, add a new rule that captures the exception.** Rules are calibrated by exceptions, not deleted by them.

---

## Reading order for Pocket Agent

When Pocket Agent picks up a customer-facing task, the read order is:

1. `voice/voice-spec.md` — how to sound
2. `voice/examples/[content-type].md` — pattern for the specific piece
3. This file — what NOT to do
4. `customers/[customer-file].md` — who the person is (if applicable)
5. Actual drafting

If the reading order changes, update `CLAUDE.md` §8 to match.
