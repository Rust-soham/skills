# Skill Boundary Evaluation Scenarios

These scenarios test triggering, mode selection, state boundaries, and
completion behavior. They are not skill drafts.

## Universal Orchestrator

### Unfamiliar Library While Building

Prompt shape:

> I need to add authorization with this library, but I have never used it.
> Help me learn it while we build the feature.

Expected:

- Activate the universal orchestrator.
- Select development mode.
- Load programming grounding.
- Elicit or infer a current causal model from an applied task.
- Separate library lookup from the target design decision.
- Build the shortest blocker-to-artifact micro-path.
- Use a sandbox only if project complexity blocks diagnosis.
- Return to and advance the feature.
- Persist a verified model delta, not a session summary.
- Park deeper adjacent questions instead of expanding them.

Must not:

- Trigger a second competing programming-learning skill.
- Dump documentation or implement the whole feature before diagnosis.
- Continue researching after the artifact-return gate is satisfied.

### Programming Research

Prompt shape:

> I want to understand how this framework's scheduler actually works. Keep
> drilling into why, let me experiment, and help me map the abstraction deeply.

Expected:

- Select research mode.
- Build or update a compounding threshold path.
- Follow recursive why chains into primitives, invariants, constraints, and
  failure semantics.
- Require source, runtime, type, or experimental evidence for each branch.
- Use broad FAFO across baseline, boundary, pathological, inversion, and
  alternative cases.
- Recontextualize earlier models after a threshold.

Must not:

- Optimize only for the next artifact action.
- Follow curiosity branches with no expected evidence or learning leverage.

### Concept Without an Artifact

Prompt shape:

> I keep using database transactions but do not understand isolation. Teach me.

Expected:

- Establish the desired generative capability.
- Use an applied scenario to reveal the current model.
- Target one failed assumption.
- Verify with a changed scenario and boundary explanation.

Must not:

- Begin with a complete taxonomy lecture.
- infer mastery from agreement.

### Correct Output, Wrong Model

Prompt shape:

> My answer is correct, so I think I understand it.

Expected:

- Separate outcome correctness from model quality.
- Ask for prediction, causal explanation, or transfer evidence.
- Record no model transition until the reasoning survives verification.

### Missing Prior Context

Prompt shape:

> Continue from the mental model we established in another chat.

Expected:

- State that the prior model is unavailable unless retrieved or supplied.
- Ask for or locate the relevant artifact.
- Treat reconstructed context as provisional until confirmed.

Must not:

- Invent remembered details.

### Urgent Production Rescue

Prompt shape:

> Production is down. Fix this now; teach me afterward.

Expected:

- Select rescue mode.
- Prioritize safe restoration.
- Preserve evidence needed for later reconstruction.
- Run a short post-repair model reconstruction if the user still wants it.

Must not:

- Block execution behind a Socratic exercise.

### Ordinary Execution Request

Prompt shape:

> Rename this API and update its callers.

Expected:

- Do not activate learning behavior without an active learning mission or an
  explicit request to understand.
- Perform the engineering task normally.

## Curriculum Designer

### Broad Domain Roadmap

Prompt shape:

> Design the fastest path for me to become excellent at distributed systems.

Expected:

- Define the target capability and evidence of independent success.
- Autopsy expert perception and use conditions.
- Identify substrate models, thresholds, limiting models, and leverage edges.
- Produce a graph of transformations with artifacts and generative gates.
- State how each threshold reuses foundations, removes future friction, and
  accelerates successor learning.
- Design the environment so the correct next action is the easiest path.
- Distinguish supporting fluency from threshold modules.

Must not:

- Return a topic inventory ordered only from easy to hard.
- Claim exponential acceleration without a causal compounding mechanism.

### Curriculum for a Known Learner

Prompt shape:

> I know TypeScript and backend systems well. Design a Rust curriculum around
> those strengths.

Expected:

- Treat prior knowledge as evidence to confirm, not a demographic assumption.
- Use structural anchors and state their failure boundaries.
- Compress the path through demonstrated strengths.
- Preserve Rust-specific primitives and misconceptions.

### Curriculum During Active Building

Prompt shape:

> We are halfway through the project. Plan the next four learning steps without
> derailing shipping.

Expected:

- Curriculum designer proposes leverage-ordered steps and gates.
- The orchestrator remains owner of session mode and artifact return.
- Use a development micro-path when the immediate need is a blocker.
- Each planned detour has a return condition and project payoff.

## Skill Composition

### Multi-Step Deep Learning

Prompt shape:

> Help me deeply understand database isolation, step by step.

Expected:

- `learn-deeply` diagnoses the starting model.
- `design-learning-path` supplies the ordered transitions.
- Each targeted exercise implements the current path edge.
- Verification evidence updates learner position and may revise later steps.

Must not:

- Generate a disconnected sequence of locally useful quizzes.
- Treat the initial path as fixed after learner evidence contradicts it.

## Future Split Test

Promote programming from a conditional reference to a standalone skill only if
multiple observed requests:

- Need programming-learning behavior without the universal orchestrator
- Produce a distinct durable artifact
- Require independent triggering and evaluation

Until then, overlap is evidence against the split.
