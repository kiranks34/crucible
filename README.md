# Crucible

**Stress-test any idea or decision before you commit.** A crucible refines raw
material into something finished under heat — this does the same for your thinking.
A rough idea, a plan, or a decision you've already made goes in; a pressure-tested
decision comes out, with you in control the whole way.

Crucible is a **decision-quality engine, not a brainstorming toy.** Every idea is
pressure-tested by five independent advisors, passed through a **Decision Gate** of
verifiable checks (no fabricated scores), and returned as a **decision-first
verdict** — the call up front, then the reasoning — with a falsifiable "kill it
if…" line. In a hurry? A fast **Quick Check** gives you a triage read in one pass.

## What you can get done with it

- **"I have a rough idea — is it any good?"** → It brainstorms the idea into a
  clear one-page brief, then stress-tests it through a panel of advisors and gives
  you a verdict with a concrete next step and a clear "kill it if…" condition.
- **"I have a few ideas and don't know which to pursue."** → It shapes them into a
  shortlist, you pick which to test, it runs each through the panel, then compares
  the verdicts so you can choose.
- **"I'm worried I'm missing better options."** → It can surface adjacent ideas you
  hadn't considered — and parks every promising one so nothing gets lost.
- **"I've already decided — just tell me if it holds up."** → It skips the
  brainstorming and takes your decision straight to the stress-test.
- **"I just want a fast gut-check."** → A **Quick Check** returns the 2–3 biggest
  risks, one kill criterion, and a lean — then offers the full panel if it matters.

You stay the decision-maker. Crucible explores, pressure-tests, and advises — it
never makes the call for you.

## The three skills inside

| Skill | What it does for you |
|-------|----------------------|
| **crucible** | Runs the whole journey: explore → choose → stress-test → compare → decide. |
| **deliberation** | The stress-test itself: five independent advisors argue your idea from different angles, peer-review each other, pass it through a Decision Gate of verifiable checks, and hand you a decision-first verdict (the call up front) plus a clear "stop if this happens" line. |
| **visualize** | Turns the thinking into something you can see and present: comparison tables, idea cards, a decision matrix, a verdict dashboard, or a polished decision deck. |

## How it works

It first reads your situation and picks the lightest path that fits:

- **Just a gut-check?** A Quick Check triages it in one pass — no full panel.
- **Already decided?** Skips brainstorming, goes straight to the stress-test.
- **One idea to vet?** Brainstorms and sharpens that idea, then tests it.
- **Exploring?** Brainstorms widely, surfaces adjacent ideas, and lets you choose
  what to test.

```
Your request
   ↓
Pick the path ── gut-check ───────────────────► Quick Check (triage) → offer full panel
              ├─ already decided ─────────────► frame it → confirm ─┐
              ├─ one idea ─► brainstorm & sharpen ──────────────────┤
              └─ exploring ► brainstorm + surface more ideas ───────┤
                                            you choose; rest parked   │
                                                                      ▼
                            Stress-test, one idea at a time (in order)
                            → Decision Gate → decision-first verdict
                                                                      ▼
                            Compare verdicts (if you tested more than one)
                                                                      ▼
                            You decide: refine / go ahead / revisit later
```

The **Decision Gate** is how a verdict stays honest: five verifiable checks —
is the core assumption backed by evidence? how bad is the worst failure? is it
reversible? is there a cheap way to test it? is a kill criterion defined? — feed a
transparent rule that returns a clear band: **Proceed**, **Validate first**, or
**Rethink**. No invented scores; you still make the final call.

Three promises worth knowing: **one idea = one stress-test** (never blended, so
each verdict is clean); **it won't over-work a simple request** (decided ideas skip
the brainstorm; single clear ideas skip the idea-expansion step); and **nothing
promising is lost** (unpicked ideas wait in a Parking Lot and come back at the end).

## See it and present it

Crucible isn't just walls of text. At the right moments it offers to turn the
thinking into a visual — and you choose whether you want it:

- **A Decision Brief card** when a single idea is framed for the go/no-go.
- **Idea cards** when ideas are being generated.
- **A comparison table** when you're choosing what to test.
- **A verdict report** after each stress-test — skim the call at the top, expand
  for the full advisor arguments, peer review, and verdict.
- **A decision matrix** comparing the verdicts.
- **A decision deck or one-pager** to present the call — at the end it offers
  *both* a leadership-ready PowerPoint (when `designleadership-pptx-desktop` is
  installed) and a clean one-page summary, and you pick.

Mid-session visuals are fast, self-contained light-mode HTML that open anywhere —
skim-first, with details a click away; the final deck or one-pager is the polished,
shareable one. Visuals are always *offered, never forced*, and you can also just
ask for one (including an image or infographic) any time.

## Already have a Council-style skill?

Crucible is self-contained — it ships its own `deliberation` engine and needs
nothing else. But if you *also* have a separate council-style skill installed, it
notices: with only one engine present it just uses it, and with two comparable
engines it asks you once which to use for the session, so you never get redundant
runs.

## Install

### Claude desktop app

**Customize → Plugins → +  → Add marketplace → Add from a repository**, point it at
this GitHub repo, then click **Install** on **Crucible**.

### Claude Code (CLI)

```
/plugin marketplace add kiranks34/crucible
/plugin install crucible@crucible
```

Then in any chat or task, say things like `vet this idea: …`, `help me choose
between these ideas: …`, `stress-test this decision: …`, or `quick check this: …`.

## Repository layout

```
.claude-plugin/marketplace.json        ← marketplace definition
plugins/crucible/
  .claude-plugin/plugin.json           ← plugin definition
  skills/crucible/SKILL.md             ← the orchestrator
  skills/deliberation/SKILL.md         ← the five-advisor stress-test
  skills/visualize/SKILL.md            ← tables, cards, dashboards, decks
LICENSE                                ← MIT
```

## Credits & provenance

- The **brainstorm** stage adapts the convergent design-dialogue method
  popularized by [obra/superpowers](https://github.com/obra/superpowers)
  (`skills/brainstorming`), independently corroborated by
  [duthaho/claudekit](https://github.com/duthaho/claudekit)'s brainstorming skill.
- The optional **idea-expansion** step draws on the 14 ideation-pattern categories
  catalogued by
  [Jamie-BitFlight/claude_skills](https://github.com/Jamie-BitFlight/claude_skills)
  (`brainstorming-skill`) — generic creativity techniques, described in original
  wording.
- The **deliberation** skill is original — inspired by the long-standing practice
  of red-team / devil's-advocate panels, it copies no third-party skill text.

## License

MIT — see [LICENSE](./LICENSE).
