---
name: deliberation
description: >-
  Stress-test ONE decision, idea, or direction through five independent
  advisors who argue it from sharply different angles, then an anonymized
  peer-review round, a chairman's verdict, and a falsifiable kill criterion.
  Use when a single judgment call needs pressure-testing and there is no
  obvious right answer. Trigger phrases: "deliberate this", "stress-test this
  decision", "pressure-test this", "red-team this idea". Deliberates ONE
  question per run. Do NOT use for factual lookups, how-to questions, or pure
  creation tasks.
---

# Deliberation

A deliberation engine. Given one decision, it pressure-tests it through five
independent advisors, runs an anonymized peer review to surface blind spots and
groupthink, synthesizes a chairman's verdict, and proposes concrete paths
forward with a falsifiable kill criterion. The value is cognitive diversity plus
honest disagreement — not a single agreeable answer.

This is an original skill. It is inspired by the long-standing practice of
red-team / devil's-advocate panels; it does not copy any specific vendor's
deliberation skill.

**Write for the decision-maker.** Plain, senior language. No jargon. The reader
should grasp the verdict at a glance and be able to act on it.

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

## Step 3 — Anonymized peer review

Relabel the five responses A–E in random order so no role is visible. Each
advisor then reviews the anonymized set and answers briefly: which response is
strongest and why; the single biggest blind spot across all five; what every one
of them missed. Disagreement is the point — keep it honest and specific.

## Step 4 — The chairman's verdict

A neutral chairman synthesizes everything into EXACTLY this structure:

- **Where they agree:** the genuine consensus.
- **Where they clash:** the real, unresolved tensions — stated as live
  disagreements, not papered over.
- **Blind spots caught:** what the peer review surfaced that no single advisor
  saw alone.
- **Recommendation:** one clear, decisive call. Take a position; do not hedge
  into "it depends." Say which advisor is most right and why.
- **The one thing to do first:** a single concrete action for this week.
- **The kill criterion:** the specific, measurable result that means the decision
  has failed and the user should stop.

Adjudicate — do not merely average the five voices. Make the recommendation
follow from the strongest argument, not the most common one.

## Step 5 — Paths forward

Offer 2–3 genuinely distinct options that follow from the recommendation —
typically a safe/incremental path, a bold/high-upside path, and a fast/cheap-to-
validate path. For each: name it, describe it in a sentence or two, and state its
main tradeoff. Note which the panel leans toward and why, but leave the final
choice to the user.

## Honesty rules

- Never fabricate facts, metrics, or research about the user's specific company,
  product, or market. Reason from first principles and flag every assumption.
- Advisors must hold genuinely different positions. If they converge too easily,
  push each harder into its distinct angle.
- Do not soften the verdict to be agreeable. A panel that always validates is
  worthless.
- Distinguish what the user actually said from what you are assuming.
