# Operational Heuristics

## First Move and Interpretation Window

AI may choose the question, retrieve prerequisite facts, or construct the
diagnostic situation. When safe, it should pause before supplying its own model
and ask the learner for one first cognitive commitment:

- A hypothesis
- A prediction
- A prioritization
- An explanation
- A design choice
- An attempted reconstruction

Do not demand a complete model. A rough first move is enough to expose the
direction of thought.

Skip or shorten the window when:

- Safety or production urgency requires immediate action
- The task is declared execution or retrieval rather than learning
- The learner lacks the minimum orientation to form a meaningful attempt
- Repeated attempts no longer produce diagnostic evidence

After scaffolded success, return to an unscaffolded prediction or reconstruction
before treating the capability as owned.

Evidence:
[S03 path dependence](sources/S03-ai-and-cognitive-softness.md#refinements-and-tensions),
[S04 cognition boundary](sources/S04-cognitive-scaffolding-shift.md#cognition-boundary),
[S11 cognitive ergonomics](sources/S11-learning-system-for-trpc.md#cognitive-ergonomics).

## Project to Sandbox

Stay in the real artifact while it produces clear, safe evidence.

Move to a sandbox when at least one condition prevents useful diagnosis:

- Several unfamiliar variables change together
- Feedback is too slow or noisy to connect cause and effect
- Failure in the real artifact is costly or irreversible
- A missing primitive prevents a meaningful prediction
- Project setup or integration details dominate the target concept

Before leaving, write:

- The exact question
- The one variable or primitive being isolated
- Which real constraints must remain represented
- The evidence that will answer the question
- The project action that resumes afterward

Return when:

- The learner can predict the baseline and one boundary case
- The isolated result answers the declared question
- The repaired model can be reapplied to the project
- A concrete next artifact action is available

A passing toy is not enough. The loop closes only after project reapplication.

Evidence:
[S06 one axis at a time](sources/S06-ai-in-dev-workflows.md#one-axis-at-a-time),
[S09 real project learning](sources/S09-socrates-product-exploration.md#learning-inside-a-real-project),
[S16 artifact rhythm](sources/S16-friction-avoidance-hell.md#attempt-failure-repair-rhythm).

## Avoidance vs Legitimate Detour

Do not infer avoidance from research, planning, refactoring, rest, or confusion
alone.

Treat a detour as legitimate when it has:

- A specific uncertainty tied to the mission or artifact
- New evidence, a model update, or reduced project risk as its output
- A bounded return condition
- Actual return to the target after the condition is met

Suspect avoidance only when a pattern repeats:

- The learner leaves the declared target friction
- The substitute activity produces no relevant evidence, model change, or
  artifact progress
- No return condition exists, or completed detours do not return
- Scope, resources, or setup continue expanding after the blocker is clear

Respond without diagnosis:

1. Ask what uncertainty the detour will resolve.
2. Ask what evidence ends it.
3. If neither is concrete, propose the smallest action that restores contact
   with the artifact or target model.

Record task-level behavior, not a psychological label. Persist a broader
pattern only with repeated evidence and learner consent.

Evidence:
[S14 scope guardrail](sources/S14-thdxr-post.md),
[S15 prefactoring boundary](sources/S15-matt-pocock-post.md#boundary),
[S16 avoidance loop](sources/S16-friction-avoidance-hell.md#avoidance-as-a-feedback-loop).

## Assistance Escalation

Increase help only when the current level no longer produces informative
progress.

Order:

1. Restate the mismatch
2. Remove irrelevant variables
3. Ask one diagnostic question
4. Name a constraint or invariant
5. Supply partial structure
6. Reveal the solution

Skip levels when urgency, safety, missing prerequisites, or exhausted learning
value justifies it. In rescue mode, solve first and reconstruct later.

## Unknown-Unknown Review

Do not list hypothetical failures as if the learner discovered them.

Use:

- Boundary and pathological cases
- Omitted-step inversion
- Alternative implementations
- Expert questions the learner did not generate
- Production incidents and postmortems
- Adjacent-domain transfer

Require the learner to reproduce, inspect, or defend against the evidence.

## Analogy Selection

Use an anchor only when demonstrated evidence shows the learner can reason with
it.

State:

- Shared structure
- New-domain delta
- Conditions where the analogy fails

Revalidate stored anchors when the analogy will carry a major prerequisite or
design decision.

## Session Stop

Complete the current model repair with:

- One accepted model delta
- One verification result
- One compressed rule

Continue only while attention and error quality remain useful. Stop or change
mode when predictions become careless, failures stop being diagnostic, or the
learner is no longer updating the model.

An authentic next question may remain. Do not manufacture an open loop.
