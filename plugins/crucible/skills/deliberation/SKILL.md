---
name: deliberation
description: >-
  Stress-test ONE decision, idea, or direction through five independent
  advisors who argue it from sharply different angles, then an anonymized
  peer-review round, a Decision Gate of verifiable checks, and a chairman's
  verdict that leads with the call plus a falsifiable kill criterion. Use when
  a single judgment call needs pressure-testing and there is no obvious right
  answer. Trigger phrases: "deliberate this", "stress-test this decision",
  "pressure-test this", "red-team this idea". Deliberates ONE question per run.
  Do NOT use for factual lookups, how-to questions, or pure creation tasks.
---

# Deliberation

A deliberation engine. Given one decision, it pressure-tests it through five
independent advisors, runs an anonymized peer review to surface blind spots and
groupthink, passes the idea through a **Decision Gate** of verifiable checks, and
synthesizes a chairman's verdict that **leads with the call** and a falsifiable
kill criterion. The value is cognitive diversity plus honest disagreement,
resolved into a clear, evidence-based decision — not a single agreeable answer,
and never a fabricated quality score.

This is an original skill. It is inspired by the long-standing practice of
red-team / devil's-advocate panels; it does not copy any specific vendor's
deliberation skill.

**Write for the decision-maker.** Plain, senior language. No jargon. Bottom line
up front: the reader should see the call in the first two lines and be able to act
on it, with the reasoning available below.

## When to use

Use only for a genuine judgment call — a decision, tradeoff, direction, or bet
with no obvious right answer. One question per run. For factual lookups,
definitions, summaries, or pure writing, answer normally instead.

## Step 1 — Frame the question

Restate the decision as ONE neutral sentence that does not lean toward yes or no.
If critical context is missing, ask exactly ONE clarifying question first. Do not
invent facts. If the caller already supplied a neutral question (e.g. handed off
from an orchestrator), use it as-is and skip straight to Step 2.

## Step 2 — Convene five advisors (independent, parallel)

Spawn all five as independent sub-agents in parallel so none sees the others'
answers. Each leans FULLY into its angle — no hedging, no "on the other hand."
Each advisor writes 150–300 words.

1. **The Skeptic** — Hunt the fatal flaw. What specifically fails, and under what
   conditions — at scale, under stress, in real use? Name the concrete failure
   mode, not generic caution.

2. **The Root-Cause Analyst** — Strip every assumption to the studs. What problem
   is actually being solved, for whom, and is it even the right problem? Rebuild
   the reasoning from the underlying job-to-be-done — and name what those people
   do TODAY instead: the status quo any solution must beat is the real competitor,
   and often the cheapest version of it is already good enough.

3. **The Opportunist** — Find the upside others are too cautious to see. The
   adjacent opportunity, the 10x version, the asymmetric payoff if it works.

4. **The Newcomer** — You have ZERO context here. React as a total first-timer:
   name what's confusing, what's unexplained jargon, what assumes knowledge a
   real user won't have. Catch the curse of knowledge insiders can't see.

5. **The Shipper** — You care only about shipping. Is it feasible? What's the
   cheapest, fastest test of the core assumption? What is the single first step
   this week? ALWAYS name a kill criterion: the specific, measurable result that
   means "stop, this isn't working."

**Optional — stakeholder grounding (opt-in; do NOT replace the five lenses).**
If the caller names one or two real stakeholders to represent (e.g. the CFO, a
frontline user, the engineer who maintains it, a regulator), have one or two of
the advisors additionally argue from that stakeholder's vantage. Keep the five
cognitive lenses as the backbone — they guarantee structurally different angles
that named stakeholders may not. Guardrail: a stakeholder-grounded advisor reasons
from that role's *likely* priorities and incentives, **explicitly flagged as
inference** — it never claims to be that person or to quote their actual views.

## Step 3 — Anonymized peer review

Relabel the five responses A–E in random order so no role is visible. Each
advisor then reviews the anonymized set and answers briefly: which response is
strongest and why; the single biggest blind spot across all five; what every one
of them missed. Disagreement is the point — keep it honest and specific.

## Step 4 — Pre-mortem (optional; high-stakes or on request)

For a high-stakes or hard-to-reverse decision, run a short pre-mortem before the
verdict: "Assume it is 12 months from now and this has clearly failed — what is
the most likely story of how it failed?" Write the two or three most plausible
failure paths. This surfaces failure modes beyond the Skeptic's single flaw.
**Skip it for low-stakes or easily reversible calls** — don't bloat every run.

## Step 5 — The Decision Gate (verifiable checks → a clear band)

Do NOT produce a numeric score — a single number on a judgment manufactures false
precision and offloads the decision onto a figure. Instead, rate the idea on these
five **verifiable** checks, drawing each rating from the advisors' material, with a
one-line rationale and a [stated]/[inferred] flag. If evidence is unknown, the
honest rating is the weaker one — say so.

1. **Core assumption — evidence?**  Verified / Partial / Unverified
2. **Worst failure mode (Skeptic) — severity?**  Recoverable / Serious / Catastrophic
3. **Reversibility?**  Two-way door (cheap to undo) / One-way door
4. **Cheapest validation?**  Cheap test exists / Costly / No clear test
5. **Kill criterion — defined & monitorable?**  Yes / No

Then derive ONE band from this conservative rule (state which check drove it):

- **PROCEED** — the core assumption is Verified or Partial-with-mitigation, the
  worst failure is Recoverable (or Serious but reversible/mitigated), and a kill
  criterion is defined. Risks are understood and bounded.
- **VALIDATE FIRST** — the deciding weakness is an Unverified core assumption AND a
  cheap test exists. Run that test before committing. (Often the right answer.)
- **RETHINK / HOLD** — the worst failure is Catastrophic on a one-way door, or there
  is no clear way to validate under high uncertainty. Reshape the idea or don't go.

The band advises; the human still makes the final call. If the caller supplied
their own criteria or thresholds, use those instead of the defaults above.

## Step 6 — The chairman's verdict (decision-first)

A neutral chairman synthesizes everything into EXACTLY this order — the call comes
first:

- **The call:** PROCEED / VALIDATE FIRST / RETHINK, in one line, naming the single
  check or argument that drove it.
- **Recommendation:** one decisive paragraph. Take a position; do not hedge into
  "it depends." Say which advisor is most right and why.
- **Do this first (this week):** a single concrete action.
- **Kill criterion:** the specific, measurable result that means stop.
- **The Decision Gate:** the five checks with their ratings and one-line rationale —
  the verifiable basis for the call.
- **The reasoning:** where they agree; where they clash (live, unresolved tensions,
  not papered over); blind spots the peer review caught that no single advisor saw.

Adjudicate — do not merely average the five voices. Make the recommendation follow
from the strongest argument, not the most common one.

## Step 7 — Paths forward

Offer 2–3 genuinely distinct options that follow from the recommendation —
typically a safe/incremental path, a bold/high-upside path, and a fast/cheap-to-
validate path. For each: name it, describe it in a sentence or two, and state its
main tradeoff. Note which the panel leans toward and why, but leave the final
choice to the user.

## Honesty rules

- Never fabricate facts, metrics, or research about the user's specific company,
  product, or market. Reason from first principles and flag every assumption.
- **Never invent a numeric quality score.** The Decision Gate uses verifiable,
  named checks and a transparent rule — not a manufactured number.
- Advisors must hold genuinely different positions. If they converge too easily,
  push each harder into its distinct angle.
- Do not soften the verdict to be agreeable. A panel that always validates is
  worthless.
- Distinguish what the user actually said from what you are assuming. Unknown
  evidence is rated as unverified, not assumed away.
