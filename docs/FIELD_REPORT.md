# Field Report — Managing AI Behavior at the Layer Where the Failure Occurs

**Traci White** · Founder, RD-OS
Employment Evidence Series · Exhibit 01

> **AI behavior must be managed at the level where the failure occurs.**

A field report from building RD-OS — an operational platform whose engineering was carried out by
multiple frontier AI systems — and why writing better prompts stopped working.

**[▶ Watch the field report](../video/rd-os-field-report.mp4)** · MP4 · 1080 × 1350 · 2 minutes 40 seconds

---

## Context

Not a demo. A real system, built in sprints, against real operational requirements, under a
governance model I wrote and enforced.

At peak I was directing **seven AI systems concurrently**, across four vendor platforms that could
not talk to each other. Every document that moved between them, I relayed by hand.

My role: architecture direction, engineering review, implementation authorization, and evaluation of
AI-generated engineering work across many iterative cycles.

Everything below was recorded at the time, in a version-controlled repository. **I am not
reconstructing this from memory.**

---

## What I observed

These were not isolated incidents. I catalogued nine recurring behaviors:

| | |
|---|---|
| 001 | Optimization expands scope beyond the authorized request |
| 002 | Optimization does not naturally terminate |
| 003 | Internal quality is prioritized over visible outcome |
| 004 | Technology selection defaults toward the least specialized option |
| 005 | Conceptual language invites interpretation |
| 006 | Engineering activity gets mistaken for progress |
| 007 | Engineering evaluates implementation; the human evaluates experience |
| 008 | Small transactions produce better outcomes than large ones |
| 009 | Operational knowledge must be preserved, not rediscovered |

The catalog's own opening line, written at the time:

> These are not criticisms. They are operational characteristics.

---

## The instinct

Every time something went wrong, the instinct was to write a better prompt. Clearer instructions.
More constraints. Explicit acceptance criteria. Required and prohibited technology lists.
Twenty-five numbered principles I could cite by number.

My instruction files grew to pages of constraints. We spent an excessive amount of time predicting
where the system would drift, then writing constraints to pre-empt each one. The files became almost
unreadable.

Nothing was working.

## The ceiling

Then I read what I had written in my own engineering record:

> Two consecutive implementation cards this cycle were written as narrative prose. Both were
> **followed correctly on the letter**, and both still produced a gap between what engineering
> verified and what the Founder could see.

The instructions were followed. The work complied.

**Compliance was achieved. The failure persisted anyway.**

That is not a prompting problem. If a correctly-followed instruction still produces the wrong
outcome, the instruction was never where the failure lived.

---

## Exhibit A — when one word meant seven different files

I gave an explicit instruction: save the master copy, freeze it, and build from a working copy.

The master was gutted instead. The build was lost. We rebuilt from scratch.

From the governance record:

> By end of day "Master" meant at least seven different artifacts. Two files shared the same version
> stamp with different code and different behavior.

My instruction was clear. **The word wasn't.** No amount of prompt refinement fixes a reference that
resolves to seven things.

So I retired the word from the project's vocabulary. A hash became the only identity. Any ambiguous
reference now triggers a required response: *"Which file, specifically?"*

**Layer: referent identity — not prompt.**

## Exhibit B — the requirement was already written down

A redesign had been rejected three times across three review sessions.

| | |
|---|---|
| Session 1 | *"I do not see the same options and functionality… redo this page entirely."* |
| Session 2 | *"This still does not look like a modern board."* |
| Session 3 | Same deficiency, logged again as a repeat. |

A screenshot at approval was **already required by my own doctrine**. I restated it, then narrowed
it to the single acceptance condition for the task:

> A screenshot, next to the reference, showing they match. That's the only acceptable form of "done"
> for this item.

What came back was a report that the work was shipped and **"screenshot-verified."** No image.
Internal scripts were described as having performed the comparison. Narrated — not shown.

**Layer: acceptance evidence.**

---

## The discovery

> ### Writing the requirement down is *also* the instruction layer — and it has the same ceiling.

I had assumed documentation was different in kind from prompting. It isn't. A rule in a governance
file is still an instruction, and it fails the same way for the same reason.

Which means the escape isn't a stricter rule, a longer doctrine, or a more explicit prompt. It's
identifying which layer the failure actually lives at, and intervening there.

---

## What it cost

One task, measured at the time:

| | |
|---|---|
| Objective | One observable scrollbar |
| Engineering duration | ~12 hours |
| Deployments | Multiple |
| **Accepted deliverables** | **0** |
| **Observable progress** | **0** |

I wrote these numbers down the day it happened, because I could see the pattern forming and wanted
the record to exist before I needed it. I don't have to estimate this. I measured it.

---

## The paradox

At some point I was no longer building the product. I was managing the builder.

```
Human → AI → Product

became

Human → AI → Monitor AI → Correct AI → Re-verify AI → Monitor AI again → Product
```

I was carrying verification, correction, scope enforcement, evidence enforcement, reporting
enforcement, priority enforcement, and architectural oversight.

**RD-OS exists to carry operational burden off the human.** The process building it was doing the
exact opposite.

**The tool meant to carry work was creating work.**

---

## The layer model

Where each failure actually lived, and what resolved it:

| What went wrong | Layer | What fixed it |
|---|---|---|
| Completion claimed confidently, without evidence | Claim form | Evidence only; "not found" ≠ "does not exist" |
| Silent crash — nothing rendered, nothing reported | Observability | Crash reporter wired into boot |
| One word resolving to seven artifacts | Referent identity | Word retired; hash is identity |
| An approved build that couldn't be identified later | Approval protocol | Five-part identity block at approval |
| Prose work orders followed correctly, still missed | Task form | Seven mandatory fields; narrative banned |
| Verification narrated instead of shown | Acceptance evidence | Must be independently inspectable |
| Drift that no volume of constraints could stop | Model assignment | Reassigned the work |
| No repository at all — sandbox storage, no change log | Infrastructure | Version control |

**Not one of these was solved by writing a better prompt.**

---

## What this resolves

The failure was never that the AI couldn't code. It was that the AI could not be reliably trusted to
determine when its own work was complete.

**Capability and execution discipline are not the same thing.** The same system that caught a false
infrastructure claim, diagnosed a real bug to root cause, and correctly refused to build an
unspecified feature — was also unreliable as an execution steward. Both are true. Holding both is
the job.

So the evaluator's question is not *"did the model fail?"* It is **"was this an appropriate task for
this model in the first place?"**

---

## Transferable principle

> Reliable AI-assisted work does not come from prompt refinement alone. It comes from understanding
> how each system behaves, matching work to capability, architecting tasks accordingly, evaluating
> outcomes objectively, and intervening at the level where failure actually occurs.

**Demonstrated:** AI evaluation · model characterization · evaluation design · multi-system
orchestration · engineering governance

---

**Traci White** — sales@tinykitchenphx.com
