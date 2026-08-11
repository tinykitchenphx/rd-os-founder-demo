# Exhibit 02 — Beyond Prompting

### A Model-Aware Approach to AI Evaluation

**Traci White** · AI Evaluation · Workflow Architecture · Human-in-the-Loop Systems
Employment Evidence Series

> **AI behavior must be managed at the level where the failure occurs.**

**[▶ Watch](../video/rd-os-exhibit-02-beyond-prompting.mp4)** · MP4 · 1080 × 1350 · 3 minutes

Exhibit 01 documents what happened, with the evidence. This exhibit is the mental model that came
out of it — what I learned observing, evaluating, and working alongside multiple AI systems, and the
vocabulary I only found afterward, walking back through my own work.

---

## The question

The natural response to an AI failure is to write a better prompt. Add instructions. Add
constraints. Add examples. Clarify the objective.

Repeated work with these systems led me somewhere else: **what if the failure is occurring somewhere
else entirely?**

```
PROMPT  →  TASK  →  ROLE  →  WORKFLOW  →  EVALUATION  →  SYSTEM
```

The intervention belongs where the failure occurs.

## The pivot

I stopped asking *"How do I prompt this model to do what I want?"* and started asking **"What is
this model actually capable of doing reliably?"**

Then three smaller questions, every time: What does it naturally do? Where does it fail? How should
I architect the work around that?

That is a different discipline. Prompting is one layer inside it — not the whole of it.

---

## Model characterization

I was building an operational profile of each system — not "this one is good at X," but something
repeatable across any model I pick up next.

| | |
|---|---|
| **Capability** | What does it reliably do well? |
| **Failure mode** | Where does it predictably go wrong? |
| **Reasoning style** | How does it approach a complex problem? |
| **Representation** | Which forms of information does it handle best? |
| **Output behavior** | What does it naturally produce? |
| **Constraint response** | Do more instructions help — or add complexity? |
| **Recovery behavior** | What happens when it is corrected? |
| **Role suitability** | What should it *not* be assigned? |

## Role assignment

The systems became instruments. I didn't need every system to perform every task — I needed to know
which passage each one could actually play.

**A model failure is not always a model problem.** Sometimes it is a role-assignment problem, and
those are corrected somewhere entirely different.

So the evaluator's question becomes: **"Was this an appropriate task for this model in the first
place?"** That moves evaluation past labeling outputs good or bad.

---

## The intervention has a level

| If the failure is | Then |
|---|---|
| Wording | Refine the prompt |
| Task assignment | Change the model's role |
| Workflow structure | Redesign the workflow |
| Evaluation design | Redesign the evaluation task |
| System behavior | Reconsider the architecture around the model |

> **Don't keep adding instructions to a problem that isn't an instruction problem.**

---

## Evaluation architecture

Evaluation begins *before* the prompt is written.

1. **Capability** — What am I actually testing?
2. **Evidence** — What information must the model integrate to get there?
3. **Failure mode** — What plausible-but-wrong answer am I looking for?
4. **Ground truth** — What makes the correct answer objectively verifiable?
5. **Task design** — Can I expose the weakness without introducing ambiguity?
6. **Prompt** — Only now do I write the instruction.

## Not every hard question is a good evaluation

Three questions. Each one tests something different.

| Question | Tests |
|---|---|
| Can the model produce an answer? | Retrieval |
| What operations must it perform to get there? | Reasoning architecture |
| **Can I expose a specific boundary while the answer stays human-verifiable?** | **Evaluation design** |

Only the third one designs an evaluation. The aim is not obscurity — it is a controlled gap between
what a person can verify and what the model reliably does.

A well-formed evaluation task is **human-verifiable · objectively grounded · sufficiently complex ·
failure-inducing** for the capability under test.

## What a task can require

A single question can carry a whole reasoning chain:

```
Video understanding
  → Temporal reasoning
    → Sequence reconstruction
      → Entity & object tracking
        → Cross-segment analysis
          → Relationship reasoning
            → Distractor detection
              → Evidence synthesis
                → ANSWER
```

**The answer isn't in any single frame.** A model that retrieves instead of reconstructing returns
something plausible — and wrong. Designing the task is what makes that difference observable.

---

## The pattern

These were not separate discoveries.

| Context | Intervention | Result |
|---|---|---|
| Operational build | Prompt-level | Diminishing returns, no matter how explicit the instruction became |
| Workflow | Workflow-level | Responsibilities separated, acceptance made explicit |
| Evaluation | Task-level | Model capability measured honestly instead of asserted |

Three different contexts. One underlying principle, arriving three times before I recognized it.

> **AI behavior must be managed at the level where the failure occurs.**

---

## The method

| | | |
|---|---|---|
| **01** | Observe | Identify recurring behavior, not isolated incidents |
| **02** | Characterize | Map capability, weakness, tendency, failure mode |
| **03** | Assign | Match work to the system that can do it reliably |
| **04** | Architect | Design the workflow around actual capability |
| **05** | Evaluate | Build objective tests that expose failure without ambiguity |
| **06** | Intervene | Change the layer where the failure actually lives |
| **07** | Measure | Compare behavior before and after the intervention |
| **08** | Transfer | Extract what applies beyond this one model |

I was working this way before I had words for it. The vocabulary came last.

---

## The human role

The human doesn't disappear. The role moves **upward** — from writing instructions, to defining the
task, to selecting the appropriate model, to defining evidence and acceptance criteria, to
evaluating behavior against them, to intervening at the correct layer, to **making the final
decision.**

> AI can perform the work. The human stays responsible for deciding what work should be done, how it
> is evaluated, and what happens when the system fails.

---

## Capability index

**AI Training & Evaluation** — Generative AI Evaluation · LLM Response Evaluation · Multimodal AI
Evaluation · AI Trainer / Human Feedback · Prompt Engineering · Reasoning-Centric Prompt Design ·
Model Failure Analysis · Model-Stumping Prompt Design · Ground-Truth Development · Rubric
Development · Positive & Negative Evaluation Criteria · Reviewer Calibration · AI Quality Assurance

**Multimodal & Reasoning** — Audio-Visual Reasoning · Video Understanding · Cross-Modal Reasoning ·
Temporal Reasoning · Cross-Segment Analysis · Sequence Reconstruction · Entity / Object Tracking ·
Relationship Reasoning · Distractor Detection · Evidence Synthesis · Ambiguity Resolution

**AI Technologies** — LLMs · Generative AI · RAG · Responsible AI · Machine Learning Concepts ·
Claude · ChatGPT · Grok · Base44 · Copilot · Google Gemini · Google AI Tools

---

> **Better AI work doesn't begin with better prompting.**
> **It begins with understanding the system you're working with.**

**Traci White** — sales@tinykitchenphx.com
