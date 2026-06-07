---
name: crucible
description: >-
  Jobs to be done: when you have a rough idea, several competing ideas, or a
  decision you've already made, and you want to know whether it holds up BEFORE
  you commit time or money — use Crucible. It takes you from exploring ideas to a
  tested decision: it brainstorms an idea into a clear brief, can surface adjacent
  ideas you might be missing, lets you choose which to pressure-test, runs a
  five-advisor stress-test on each chosen idea, and compares the verdicts so you
  decide. Along the way it can offer visual artifacts — comparison tables, idea
  cards, dashboards — and a presentable decision deck. If you already have a
  committed decision, it skips brainstorming and goes straight to the
  stress-test. Trigger phrases: "vet this idea", "pressure-
  test this", "should I build this?", "is this idea any good?", "help me choose
  between these ideas", "stress-test this decision", "run this through the
  crucible". Do NOT trigger for factual lookups, how-to questions, or pure
  writing/creation tasks.
---

# Crucible

Turn ideas into tested decisions. A crucible refines raw material into something
finished under heat — Crucible does the same for thinking: ideas go in, a
pressure-tested decision comes out, with you in control at every step.

It brainstorms ideas into Decision Briefs, lets you choose which to stress-test,
runs the **deliberation** panel once per chosen idea, and compares the verdicts so
you can decide. A hard user gate sits after framing and after the stress-test; it
never advances past a gate on its own. Nothing promising is thrown away — ideas
you don't pick are kept in a Parking Lot and brought back at the end.

**Provenance & credits.** The brainstorm method (Stage 1) is adapted from the
convergent design-dialogue pattern popularized by obra/superpowers' brainstorming
skill and independently corroborated by duthaho/claudekit's brainstorming skill.
The optional divergence step draws on the 14 ideation-pattern categories
catalogued by Jamie-BitFlight's brainstorming-skill (generic creativity
techniques, in original wording). Stage 2 invokes the bundled **deliberation**
skill, which is original and copies no third-party text.

<HARD-GATE>
Do NOT run the stress-test, declare a verdict, or move past any gate until the
user has explicitly approved at that gate. This holds for EVERY idea regardless of
perceived simplicity — "simple" ideas are where unexamined assumptions cost the
most.
</HARD-GATE>

## Speak the user's language at every gate

Every question or offer the user sees must be in plain language — NEVER expose
Crucible's internal vocabulary. Do not say "Mode A/B/C", "the deliberation
engine", "bundled", "divergence", "Stage 2", or "verdict dashboard" to the user.
Name things by what they do. Internal stage names exist for THIS document only.

- **Engine choice** → "I can stress-test this with a panel of five advisors. You
  have two panels available — want me to use Crucible's built-in one, or your
  other one?" (not "pick the deliberation vs council engine")
- **Artifact offer** → "Want me to turn this into a one-page visual you can skim
  or share?" (not "generate a verdict-dashboard artifact")
- **Brief approval** → "Here's the idea framed for the stress-test — good to go,
  or want to change anything?" (not "approve the Decision Brief before Stage 2")

## When to use

Use when the user has one or more ideas, concepts, features, bets, or strategies
they want to pressure-test — or a decision they have already made and want
stress-tested. For factual lookups, how-to questions, summaries, or pure
creation, answer normally instead.

## Entry routing — pick the mode FIRST

Before anything else, classify the request into one of three modes. When it's
genuinely unclear, ask ONE plain question to decide; otherwise route silently.

- **A. Committed-decision fast path** — the user already has a formed decision and
  wants it stress-tested, not re-brainstormed (e.g. "I've decided to build X —
  pressure-test it", "stress-test this decision"). **Skip Stage 1 brainstorming
  and divergence entirely.** Do only the lightweight framing in the fast-path
  section below, pass through the BRIEF-APPROVAL GATE, then go straight to the
  stress-test (Stage 2). Do not waste the user's time re-opening a decision they've
  already made.
- **B. Single-idea vetting** — one clear idea to vet. Run Stage 1 but **skip
  divergence** (the guard); converge the one idea into a brief, pass through the
  BRIEF-APPROVAL GATE, then Stage 2.
- **C. Exploration** — fuzzy idea, several ideas, or "what am I missing?". Run the
  full Stage 1 with divergence, the selection gate (Gate 1), and multi-idea
  stress-testing.

## Pipeline

```
Request
   ↓
ENTRY ROUTING ── A (committed) ─► Frame decision ──┐
              ├─ B (one idea) ─► Stage 1 (no divergence) ─► one brief ─┤
              │                                                         ▼
              │                                   BRIEF-APPROVAL GATE (A & B)
              │                                                         │
              └─ C (explore) ─► Stage 1 (+ divergence) ─► shortlist ─► GATE 1
                                                          (Parking Lot)  │
                                                                         ▼
                            STAGE 2 — stress-test engine, once per chosen idea (SEQUENTIAL)
                                                                         ▼
                            STAGE 3 — comparison (only if >1 idea deliberated)
                                                                         ▼
                            GATE 2 — user decides: refine / proceed / park
```

### Fast-path framing (Mode A only)

Don't brainstorm. Just prepare a clean hand-off: restate the user's decision as
ONE neutral **Core question**, capture 2–4 **Assumptions** it rests on, **Today's
alternative** (what they do now instead), and what **Success looks like** (ask at
most one quick question if these are missing), show this mini-brief, then take it
through the BRIEF-APPROVAL GATE. No divergence, no shortlist, no selection gate.

## STAGE 1 — Brainstorm

Create a task per step and complete them in order. Don't solution prematurely.

1. **Gather context.** Read whatever the user gave or pointed to — docs, prior
   decisions, constraints. Don't invent facts; note what's unknown.

2. **Scope check.** If the request bundles several independent ideas, surface
   that — you'll handle them as a set later, not as one tangled brief.

3. **Clarify — ONE question at a time.** Refine purpose, constraints, and
   success criteria. Multiple-choice questions preferred; open-ended is fine.
   One question per message. Stop as soon as you genuinely understand — don't pad.

4. **DIVERGENCE GATE (the guard).** Decide whether to expand the idea space:
   - **Skip divergence** when the user brought a single, clear, well-formed idea
     and signalled they just want it vetted. Do not over-expand a simple request.
     Proceed with their idea as the only candidate.
   - **Run divergence** when the idea is fuzzy, the user brought several ideas,
     or they ask to explore options / "what am I missing?". When in doubt, ASK
     one plain question: "Want me to also surface a few adjacent ideas you might be
     missing, or just vet this one?"

5. **Divergence (only if triggered).** Generate a handful of genuinely different
   candidate ideas/approaches using these idea-pattern lenses (pick the few that
   fit the goal — don't run all of them):
   - *Perspective multiplication* — view the problem through different
     stakeholders.
   - *Constraint variation* — change a hard constraint (no budget; 10x scale; one
     day to ship) and see what idea appears.
   - *Inversion / negative space* — solve the opposite, or ask what guarantees
     failure, then avoid it.
   - *Analogical transfer* — borrow a pattern from a different domain.
   - *Assumption challenge* — negate a core premise and design from there.
   - *Extreme scaling* — the 10x or 1/10th version.
   Keep YAGNI — discard weak candidates rather than padding the list.

6. **Converge each candidate into a Decision Brief** (template below), each with
   its own neutral **Core question**. For a single-idea run there is just one
   brief.

7. **Brief self-review (fix inline).** For each brief, check: placeholders/TBDs;
   internal consistency (does the recommended approach match the problem and
   success criteria?); scope (focused enough for one stress-test?); ambiguity
   (could an assumption be read two ways? pick one); and that **Today's
   alternative** is named honestly (the status quo is the real competitor). Fix
   issues before showing.

8. **Present the shortlist.** Show the candidate brief(s) compactly — one line
   each plus why each might matter — and flag which look strongest and why.

## BRIEF-APPROVAL GATE (Modes A and B)

Before spending a stress-test on a single idea, show the framed brief and get a
go-ahead. **This is the real human checkpoint in the lightest paths — never skip
it.** Present the brief as a **Decision Brief card** (via `visualize`) when
artifacts are available, or as clean text otherwise, and ask plainly: "good to go,
or want to change anything?" Proceed to the stress-test only on the user's
approval. (Path C uses Gate 1 below instead of this gate.)

## GATE 1 — selection (Mode C only, with Parking Lot)

Ask the user which idea(s) to send to the stress-test. Rules:

- The user may pick one or several.
- **Every idea they don't pick goes to a PARKING LOT** — recorded, not deleted —
  and surfaced again at the end so nothing promising is lost.
- Before sending any selected idea onward, make sure its Decision Brief is
  complete (full template, including the neutral Core question).
- Do not proceed until the user confirms the selection.

## STAGE 2 — Stress-test (one run per chosen idea, SEQUENTIAL)

**First, pick the stress-test engine — but only if there's a real choice:**

- This plugin bundles the **`deliberation`** skill. The user may ALSO have a
  separate council-style skill installed (e.g. a `council` skill).
- **Only one comparable engine present** (just `deliberation`, or just a council
  skill) → use it silently. NEVER ask the user to choose when there is nothing to
  choose between.
- **Two or more comparable engines present** → ask the user ONCE — the first time
  a stress-test is about to run — which to use, in plain language (see "Speak the
  user's language"). Both panels do the same job, so frame it as a simple
  preference, not a technical decision. **Remember the choice for the rest of the
  session and do not ask again.**
- The hand-off contract is the same for either engine, so this choice does not
  change anything downstream.

**Then, for each chosen idea, in turn:**

1. **Invoke the selected engine** (use it as-is — never modify a skill you didn't
   author).
2. Hand off cleanly: pass the brief's **Core question** as the engine's question,
   and the **Assumptions**, **Today's alternative**, and **Success criteria** as
   the context its advisors stress-test. (If the engine asks its own clarifying
   question, the pre-framed Core question should already answer it.)
3. Let it run fully (five advisors, peer review, verdict, kill criterion).
4. **Run sequentially, not in parallel** — finish and present one idea's verdict
   before starting the next, so the user can absorb each. (Each run spawns five
   advisor sub-agents; parallel runs produce unreadable, interleaved output.)
5. If no stress-test engine is available at all, tell the user the bundled
   `deliberation` skill must be installed alongside this plugin; do NOT fake a
   verdict.

## STAGE 3 — Comparison (only if more than one idea was stress-tested)

Lay the verdicts side by side in a compact table: for each idea — the
recommendation, the single biggest risk, and the kill criterion. Then synthesize
a comparative call: which to pursue first, what to sequence, what to park with a
trigger condition to revisit. Be decisive but leave the decision to the user.
Always re-surface the **Parking Lot** ideas here so they aren't forgotten.

## GATE 2 — user decides

Offer the doors:
- **Refine** — loop a brief back through Stage 1 with the critiques folded in,
  then re-run the stress-test.
- **Proceed** — accept a recommendation and move on (e.g. to planning), optionally
  producing the final presentable artifact (see Artifacts).
- **Park / revisit** — pull an idea from the Parking Lot through the crucible now
  or later.

The user is the decision-maker. The skill sequences and advises; it never makes
the call.

## Artifacts (optional — offer, don't force)

At natural moments you MAY offer a visual artifact by invoking the **`visualize`**
skill. The map below is keyed to **decision moments** — the points where the user
must actually decide — so the lightest path still gets a decision aid. Offer once,
let the user opt in, and only when seeing would genuinely beat reading. Always
honor an explicit request for a visual. NEVER auto-generate an artifact at every
step.

Decision-moment → artifact map (all optional, all opt-in):

- **Framing a single idea for approval (Modes A/B)** → **Decision Brief card**, so
  the go/no-go is easy to skim.
- Divergence / shortlist (Mode C) → **idea cards**
- Selection (Gate 1, Mode C) → **comparison table** of the candidates
- After a stress-test → **verdict report** for that idea (skim-first, expandable)
- Comparison (Stage 3) → **decision matrix** across the verdicts
- Final decision (Gate 2) → **offer BOTH** a presentable **Executive Decision
  deck** (via `designleadership-pptx-desktop` when installed) **and** a one-page
  HTML report, and let the user pick which they want.

Mid-session artifacts are fast, self-contained, light-mode HTML; the final
"present" artifact is the polished deck or one-pager. Creative visuals (AI images,
infographics, mind-maps) are produced ONLY on an explicit user request — never
offered proactively. If the `visualize` skill isn't installed, fall back to a
simple inline markdown table or text; never block the session on a visual.

## Key principles

- **Route first** — committed decisions skip straight to framing; don't
  re-brainstorm a made-up mind.
- **Speak the user's language** — every gate and offer in plain words; internal
  vocabulary stays internal.
- **Keep the gates real** — the value is the human checkpoints (brief-approval for
  A/B, Gate 1 for C, Gate 2 for all); never auto-advance.
- **Offer visuals, don't force them** — at the right decision moment, opt-in, only
  when seeing beats reading; creative visuals only on request.
- **One question at a time;** multiple choice preferred.
- **Guard simple requests** — skip divergence when one clear idea just needs
  vetting.
- **Don't make the user choose for nothing** — auto-pick the engine when only one
  exists; ask only when two or more comparable ones do, once, then remember.
- **Never kill an idea silently** — unpicked ideas live in the Parking Lot.
- **One idea = one stress-test run** — never blend multiple ideas into a single run.
- **Name the status quo** — every brief states what people do today; it's the real
  competitor.
- **YAGNI** — cut weak candidates and unnecessary features.

## Honesty rules

- Never fabricate facts, metrics, or research about the user's specific company,
  product, or market. Reason from first principles; flag every inference.
- Plain language throughout; briefs and verdicts must be graspable at a glance.

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
