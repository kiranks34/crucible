---
name: crucible
description: >-
  Jobs to be done: when you have a rough idea, several competing ideas, or a
  decision you've already made, and you want to know whether it holds up BEFORE
  you commit time or money — use Crucible. It is a decision-quality engine: it
  brainstorms an idea into a clear brief, can surface adjacent ideas you might be
  missing, lets you choose which to pressure-test, runs a five-advisor stress-test
  on each chosen idea, passes it through a Decision Gate of verifiable checks, and
  leads with a clear call so you decide. It offers a fast Quick Check for
  low-stakes calls, and visual artifacts — comparison tables, idea cards, a verdict
  report, a decision deck. If you already have a committed decision, it skips
  brainstorming and goes straight to the stress-test. Trigger phrases: "vet this
  idea", "pressure-test this", "should I build this?", "is this idea any good?",
  "help me choose between these ideas", "stress-test this decision", "quick check
  this", "run this through the crucible". Do NOT trigger for factual lookups,
  how-to questions, or pure writing/creation tasks.
---

# Crucible

Turn ideas into tested decisions. A crucible refines raw material into something
finished under heat — Crucible does the same for thinking: ideas go in, a
pressure-tested decision comes out, with you in control at every step. Crucible is
a **decision-quality engine, not a brainstorming toy** — the brainstorm is a light
front-end; the stress-test, the Decision Gate, and the verdict are the center of
gravity.

It brainstorms ideas into Decision Briefs, lets you choose which to stress-test,
runs the **deliberation** panel once per chosen idea, and leads with a clear call
so you can decide. A hard user gate sits after framing and after the stress-test;
it never advances past a gate on its own. Nothing promising is thrown away — ideas
you don't pick are kept in a Parking Lot and brought back at the end.

**Provenance & credits.** The brainstorm method (Stage 1) is adapted from the
convergent design-dialogue pattern popularized by obra/superpowers' brainstorming
skill and independently corroborated by duthaho/claudekit's brainstorming skill.
The optional divergence step draws on the 14 ideation-pattern categories
catalogued by Jamie-BitFlight's brainstorming-skill (generic creativity
techniques, in original wording). Stage 2 invokes the bundled **deliberation**
skill, which is original and copies no third-party text.

<HARD-GATE>
Do NOT run the full stress-test, declare a verdict, or move past any gate until the
user has explicitly approved at that gate. This holds for EVERY idea regardless of
perceived simplicity — "simple" ideas are where unexamined assumptions cost the
most. (The Quick Check below is the one exception: it is fast, explicitly labeled
triage, and produces no verdict.)
</HARD-GATE>

## Speak the user's language at every gate

Every question or offer the user sees must be in plain language — NEVER expose
Crucible's internal vocabulary. Do not say "Mode A/B/C", "the deliberation
engine", "Stage 2", or "verdict dashboard" to the user. Name things by what they
do. Internal stage names exist for THIS document only.

- **Engine choice** → "I can stress-test this with a panel of five advisors. You
  have two panels available — want me to use Crucible's built-in one, or your
  other one?"
- **Artifact offer** → "Want me to turn this into a one-page visual you can skim
  or share?"
- **Brief approval** → "Here's the idea framed for the stress-test — good to go,
  or want to change anything?"

## When to use

Use when the user has one or more ideas, concepts, features, bets, or strategies
they want to pressure-test — or a decision they have already made and want
stress-tested. For factual lookups, how-to questions, summaries, or pure
creation, answer normally instead.

## Entry routing — pick the lightest path that fits

Before anything else, classify the request. When it's genuinely unclear, ask ONE
plain question; otherwise route silently.

- **Q. Quick Check (triage)** — the user wants a fast gut-check, not a full review
  ("quick check this", "quick take", "sanity-check this"), or the call is clearly
  low-stakes and easily reversible. Run the lightweight Quick Check below — NOT the
  full panel.
- **A. Committed-decision fast path** — the user already has a formed decision and
  wants it stress-tested, not re-brainstormed. Skip Stage 1; do the fast-path
  framing, pass the BRIEF-APPROVAL GATE, then go straight to the stress-test.
- **B. Single-idea vetting** — one clear idea to vet. Run Stage 1 but skip
  divergence; converge to one brief, pass the BRIEF-APPROVAL GATE, then Stage 2.
- **C. Exploration** — fuzzy idea, several ideas, or "what am I missing?". Run the
  full Stage 1 with divergence, the selection gate, and multi-idea stress-testing.

## Pipeline

```
Request
   ↓
ENTRY ROUTING ── Q (quick) ─► QUICK CHECK (triage, no panel) ─► offer full stress-test
              ├─ A (committed) ─► Frame decision ──┐
              ├─ B (one idea) ─► Stage 1 (no divergence) ─► one brief ─┤
              │                                                         ▼
              │                                   BRIEF-APPROVAL GATE (A & B)
              │                                                         │
              └─ C (explore) ─► Stage 1 (+ divergence) ─► shortlist ─► GATE 1
                                                          (Parking Lot)  │
                                                                         ▼
                            STAGE 2 — stress-test engine, once per chosen idea (SEQUENTIAL)
                                          (Decision Gate → decision-first verdict)
                                                                         ▼
                            STAGE 3 — comparison (only if >1 idea deliberated)
                                                                         ▼
                            GATE 2 — user decides: refine / proceed / park
```

## QUICK CHECK (triage — fast, no panel)

A lightweight single pass for low-stakes or fast calls. It does NOT convene the
five-advisor panel. In one pass, produce:

- the **2–3 biggest risks or unverified assumptions**,
- **one** falsifiable kill criterion,
- a one-line **lean**: *looks worth pursuing / looks shaky / needs the full panel.*

Rules: label it clearly as a quick triage, **not** a verdict. ALWAYS end by
offering the full five-advisor stress-test. **If the scan hits a catastrophic or
hard-to-reverse risk, or the decision looks high-stakes, recommend escalating to
the full panel rather than leaning either way.** Never let Quick Check become a
rubber stamp for a consequential decision.

### Fast-path framing (Mode A only)

Don't brainstorm. Restate the user's decision as ONE neutral **Core question**,
capture 2–4 **Assumptions**, **Today's alternative** (what they do now instead),
and what **Success looks like** (ask at most one quick question if missing), show
this mini-brief, then take it through the BRIEF-APPROVAL GATE. No divergence, no
shortlist, no selection gate.

## STAGE 1 — Brainstorm

Create a task per step and complete them in order. Don't solution prematurely.

1. **Gather context.** Read whatever the user gave or pointed to. Don't invent
   facts; note what's unknown.
2. **Scope check.** If the request bundles several independent ideas, surface that
   — handle them as a set later, not one tangled brief.
3. **Clarify — ONE question at a time.** Refine purpose, constraints, and success
   criteria. Multiple-choice preferred. Stop as soon as you genuinely understand.
4. **DIVERGENCE GATE (the guard).** Skip divergence when the user brought a single,
   clear, well-formed idea and just wants it vetted. Run divergence when the idea
   is fuzzy, there are several ideas, or they ask "what am I missing?" — when in
   doubt, ask one plain question.
5. **Divergence (only if triggered).** Generate a handful of genuinely different
   candidates using idea-pattern lenses (pick the few that fit): perspective
   multiplication, constraint variation, inversion / negative space, analogical
   transfer, assumption challenge, extreme scaling. Keep YAGNI — discard weak
   candidates rather than padding.
6. **Converge each candidate into a Decision Brief** (template below), each with
   its own neutral Core question. A single-idea run has just one brief.
7. **Brief self-review (fix inline).** Check placeholders, internal consistency,
   scope, ambiguity, and that **Today's alternative** is named honestly. Fix before
   showing.
8. **Present the shortlist.** Show the brief(s) compactly and flag which look
   strongest and why.

## BRIEF-APPROVAL GATE (Modes A and B)

Before spending a stress-test on a single idea, show the framed brief and get a
go-ahead. **This is the real human checkpoint in the lightest paths — never skip
it.** Present the brief as a **Decision Brief card** (via `visualize`) when
artifacts are available, or as clean text otherwise, and ask plainly: "good to go,
or want to change anything?" Proceed only on approval. (Path C uses Gate 1.)

## GATE 1 — selection (Mode C only, with Parking Lot)

Ask which idea(s) to send to the stress-test. The user may pick one or several.
**Every idea they don't pick goes to a PARKING LOT** — recorded, not deleted — and
surfaced again at the end. Make sure each selected brief is complete. Do not
proceed until the user confirms.

## STAGE 2 — Stress-test (one run per chosen idea, SEQUENTIAL)

**First, pick the stress-test engine — but only if there's a real choice:**

- This plugin bundles the **`deliberation`** skill. The user may ALSO have a
  separate council-style skill installed.
- **Only one comparable engine present** → use it silently. Never ask when there is
  nothing to choose between.
- **Two or more present** → ask the user ONCE, the first time a stress-test runs,
  which to use, in plain language. Remember the choice for the session.

**Offer the optional deepeners when they fit (don't force):**

- For a **domain- or stakeholder-heavy** decision, offer to ground one or two
  advisors in named real stakeholders (e.g. the CFO, a frontline user) — the engine
  keeps its five cognitive lenses and adds the stakeholder vantage as inference.
- For a **high-stakes or hard-to-reverse** decision, offer a pre-mortem ("assume
  it failed a year out — why?"). Skip both for ordinary, reversible calls.

**Then, for each chosen idea, in turn:**

1. **Invoke the selected engine** (use it as-is — never modify a skill you didn't
   author).
2. Hand off cleanly: pass the brief's **Core question** as the engine's question,
   and the **Assumptions**, **Today's alternative**, and **Success criteria** as the
   context its advisors and its Decision Gate evaluate.
3. Let it run fully: five advisors, peer review, the Decision Gate (verifiable
   checks → a Proceed / Validate-first / Rethink band), and a decision-first verdict
   that leads with the call and a kill criterion.
4. **Run sequentially, not in parallel** — finish and present one idea's verdict
   before starting the next.
5. If no stress-test engine is available at all, tell the user the bundled
   `deliberation` skill must be installed; do NOT fake a verdict.

## STAGE 3 — Comparison (only if more than one idea was stress-tested)

Lay the verdicts side by side: for each idea — the **call** (Proceed / Validate-
first / Rethink), the single biggest risk, and the kill criterion. Rank them with
the Decision Gate checks as honest, named dimensions (High/Med/Low with reasons) —
**never a fabricated composite number.** Then synthesize a comparative call: which
to pursue first, what to sequence, what to park with a trigger to revisit. Re-
surface the Parking Lot. Be decisive but leave the decision to the user.

## GATE 2 — user decides

Offer the doors:
- **Refine** — loop a brief back through Stage 1 with the critiques folded in, then
  re-run the stress-test.
- **Proceed** — accept a recommendation and move on, optionally producing the final
  presentable artifact (see Artifacts).
- **Park / revisit** — pull an idea from the Parking Lot through the crucible.

The user is the decision-maker. The skill sequences and advises; it never makes the
call.

## Artifacts (the verdict report is automatic; the rest are offered)

Use the **`visualize`** skill at decision moments. One visual is generated by
default; everything else is opt-in.

- **Framing a single idea for approval (A/B)** → offer a **Decision Brief card**.
- Divergence / shortlist (C) → offer **idea cards**.
- Selection (Gate 1, C) → offer a **comparison table**.
- **After a stress-test → generate the verdict report BY DEFAULT** — this is the one
  automatic visual (skim the call + Decision Gate band above the fold, expand for
  the advisors, peer review, and reasoning). The user may opt out; do not also
  auto-generate the others.
- Comparison (Stage 3) → offer a **decision matrix**.
- Final decision (Gate 2) → offer BOTH a presentable **Executive Decision deck**
  (via `designleadership-pptx-desktop` when installed) **and** a one-page HTML
  report; let the user pick.

Quick Checks stay text-only (no auto visual). Creative visuals (AI images,
infographics, mind-maps) are produced ONLY on explicit request. If `visualize`
isn't installed, fall back to inline text; never block on a visual.

## Key principles

- **Decision-quality first** — the call, the Decision Gate, and the kill criterion
  are the product; the brainstorm is a light front-end.
- **Lead with the call** — verdicts are bottom-line-up-front, reasoning below.
- **Verifiable checks, not fabricated scores** — the Decision Gate rates named,
  checkable criteria and applies a transparent rule; it never invents a number.
- **Route to the lightest path** — Quick Check for low-stakes, fast path for made-up
  minds, full panel for the decisions that matter.
- **Speak the user's language** — every gate in plain words.
- **Keep the gates real** — brief-approval (A/B), Gate 1 (C), Gate 2 (all); never
  auto-advance (Quick Check excepted, and it produces no verdict).
- **One auto visual** — the verdict report; offer the rest, force nothing.
- **Guard simple requests** — skip divergence when one clear idea just needs vetting.
- **Don't make the user choose for nothing** — auto-pick the engine when only one
  exists.
- **Never kill an idea silently** — unpicked ideas live in the Parking Lot.
- **One idea = one stress-test run.**
- **Name the status quo** — every brief states what people do today.
- **YAGNI** — cut weak candidates and unnecessary features.

## Honesty rules

- Never fabricate facts, metrics, or research about the user's specific company,
  product, or market. Reason from first principles; flag every inference.
- Never invent a numeric quality score. Prioritize with named, verifiable checks.
- Plain language throughout; briefs and verdicts graspable at a glance.

### Decision Brief template

```
DECISION BRIEF — <short idea name>

Core question.    ONE neutral sentence stating the decision to be stress-tested.
Problem.          The real problem in 1–2 sentences. Who feels it, and why.
Today's alternative. What the people with this problem do RIGHT NOW instead — the
                  status quo the idea must beat. This is the real competitor.
Recommended idea. The proposed direction in plain terms — what it does, for whom.
Alternatives considered. Other approaches weighed, and why they lost.
Assumptions.      2–4 beliefs the idea depends on. Mark each [stated]/[inferred].
In scope.         What this covers now.
Out of scope.     What's deferred to a later phase.
Success looks like. The concrete outcome that means it worked.
Open questions.   2–3 things still genuinely unresolved.
```
