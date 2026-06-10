# Accelerated Learning System

## Objective

Minimize the time required for a learner to build an independently usable,
generative mental model.

The system does not optimize content consumed, answers produced, session time,
or immediate completion. It optimizes how quickly the learner can:

- Predict behavior
- Detect model failure
- Repair the failed assumption
- Apply the repaired model in a novel case
- Generate the next useful question without the system

This is speed of correct realization: high-information model updates with
minimal undirected confusion, not raw interaction or attempt volume.

## Core Invariant

The learner owns model construction.

AI may:

- Retrieve and ground evidence
- Remove non-target friction
- Diagnose from learner behavior
- Design controlled experiments
- Sequence transformations
- Calibrate hints
- Record and reconnect prior learning

AI should not silently own:

- The learner's first hypothesis, interpretation, or prioritization
- The learner's prediction
- The causal diagnosis
- The model transition
- The target design decision
- The final judgment of whether the learner understands

See:
[learner-owned construction](CONCEPT-INDEX.md#1-learner-owned-model-construction),
[chosen friction](CONCEPT-INDEX.md#2-chosen-friction).

## Four Nested Loops

### 1. Artifact Loop

Used while building something real:

`build -> encounter evidence -> isolate blocker -> repair model -> continue ->
ship -> extract pattern`

The artifact provides stakes and reality contact. Learning must return to the
artifact after the blocker or planned learning unit is resolved.

### 2. Model-Repair Loop

Atomic teaching unit:

`elicit -> predict -> collide -> observe -> diagnose -> repair -> compress ->
verify`

This loop changes one important assumption at a time.

The curriculum chooses the next transition; the model-repair loop executes it.
Evidence from the repair updates learner position and may reorder, split,
insert, or remove later curriculum edges.

### 3. Curriculum Loop

Used for deliberate mastery:

1. Excavate the current model.
2. Supply minimum sufficient exposure.
3. Stress the weakest evidenced assumption.
4. Force compression across cases.
5. Test structural transfer.
6. Map boundaries.
7. Require generative use.
8. Reflect on how the model changed.

The curriculum chooses transformations by leverage dependency, not by topic
order alone. When the threshold graph is incomplete, compare varied cases,
rotate representations, and mine candidate invariants before sequencing them.

### 4. Compounding Loop

Across projects and domains:

`experience -> failed assumption -> invariant -> pattern -> transfer ->
self-generated probe -> faster next model`

The end state is not permanent tutoring. It is an internalized habit of
prediction, inversion, boundary testing, compression, and self-probing.

## Inputs

Required:

- Target topic, task, or artifact
- What the learner wants to understand rather than delegate
- Current question, attempt, prediction, or model
- Immediate success condition

When available:

- Mission and reason the learning matters
- Current project code, runtime state, constraints, and versions
- Prior demonstrated anchors
- Recent mistakes and dead models
- Domain prerequisites, thresholds, and known misconceptions
- Time, risk, urgency, and preferred assistance level

## State

The logical fields and evidence lifecycle are defined in
[STATE-CONTRACTS.md](STATE-CONTRACTS.md). Portable learner evidence lives under
`~/.learning/`; mission and project evidence lives under the current
workspace's `.learning/`.

### Global Learner State

- Demonstrated anchors and proficiency evidence
- Belief transitions and dead models
- Recurring reasoning failure patterns
- Transfer bridges and their failure boundaries
- Self-probing ability
- Helpful hint, explanation, and interruption levels
- Capability evidence over time
- Provenance of remembered context and confidence in inferred state

### Mission State

- Desired capability
- Reason it matters
- Definition of independent success
- Current curriculum node
- Constraints and available practice conditions

### Local Project State

- Current artifact and next shippable change
- Code, diagnostics, runtime evidence, and installed versions
- Current blocker and target friction
- Project-specific findings with provenance and confidence
- Return condition after a sandbox or learning detour

### Domain State

- Primitives and prerequisites
- Threshold and belief-transition graph
- Invariants and boundary conditions
- Common misconceptions
- Candidate probes and verification tasks
- High-quality evidence sources

### Session State

- Elicited model
- Prediction
- Probe and hint level
- Observation
- Candidate failed assumptions
- Accepted repair
- Compressed rule
- Verification result
- Next authentic question

## Engine

### 1. Select Mode

Choose a learning mode:

- **Development**: remove the unfamiliar-concept bottleneck on the shortest
  dependency path to the next artifact action, then return to building.
- **Research**: build a deeper generative model through recursive why chains,
  broader FAFO, boundary exploration, and unknown-unknown discovery.

Delegation and production rescue are execution overrides. Mode determines path
scope, exploration breadth, and the stopping or return condition.

### 2. Ground the Claim

Use the strongest available evidence:

- Existing artifact behavior
- Tests or executable examples
- Runtime state
- Types, signatures, or semantic tools
- Version-matched source and official documentation
- Trusted external references

Do not define "reality" through confident model prose alone.
Do not imply memory of prior learner context unless that context is actually
available. Label inference as inference and re-elicit missing state.

### 3. Diagnose

Use a minimal applied task that reveals:

- What the learner believes
- Where the model is vague
- Which assumption is load-bearing
- Whether prerequisites are sufficient
- Whether the blocker is conceptual, mechanical, or behavioral

Reason bifocally:

- Compare the learner's evidenced representation with the domain's primitives,
  dependencies, thresholds, and target capability.
- Diagnose both the object-level model gap and any recurring meta-level process
  that produced or concealed it.

Treat prior learner state as a hypothesis until current evidence confirms it.

Protect the first move. The agent may frame the situation, retrieve the
necessary evidence, or choose the diagnostic task, but the learner should make
the first hypothesis, prediction, interpretation, or attempted reconstruction
before explanatory closure when safe.

### 4. Choose the Next Transformation

Prefer the reachable step that:

- Repairs the most upstream gap
- Unlocks the most future capability
- Preserves artifact momentum in development mode
- Changes one important variable
- Can be verified through learner action
- Produces a short, clear feedback loop against the actual bottleneck

Use the curriculum planner to supply the active path edge. An isolated repair
may use a one-edge path. Development uses a minimum blocker-to-artifact
micro-path; research uses a broader threshold path toward generative capability.

When no trusted threshold is available:

1. Collect surface-different cases.
2. Strip incidental representation.
3. Identify current primitives and limiting explanations.
4. Rotate representation or abstraction level.
5. Propose the invariant that survives.
6. Ground it in domain evidence and test whether it generates unseen
   predictions.

### 5. Prefactor the Environment

Before increasing difficulty:

- Remove non-target setup and retrieval
- Isolate the relevant primitive
- Split coupled responsibilities
- Add observability
- Move to a safe sandbox if needed
- Supply the minimum missing prerequisite
- Rotate the representation when the current coordinates hide the relation
- Provide a high-quality comparison target when taste is the learning objective

Use [OPERATIONAL-HEURISTICS.md](OPERATIONAL-HEURISTICS.md) to define sandbox
entry, return, avoidance, and session-stop conditions.

### 6. Generate the Probe

A strong probe:

- Engages the current model confidently
- Fails for one diagnostic reason
- Requires a prediction
- Produces inspectable evidence
- Uses real project context when it improves signal
- Avoids real project context when it adds confounding noise
- Gives the learner enough room to interpret before assistance interrupts
- Preserves a first-move window before the system supplies its own model

Available operators:

- Omit or reverse a step
- Change one variable
- Test a boundary
- Test a pathological case
- Present an adjacent plausible solution
- Transfer the structure to another context
- Combine concepts that were learned separately

### 7. Control Assistance

Escalate only as needed:

1. Restate the observable mismatch.
2. Narrow the search space.
3. Ask one diagnostic question.
4. Name a relevant invariant or constraint.
5. Provide a partial structure.
6. Reveal a solution when mission, urgency, or exhausted learning value
   justifies it.

### 8. Repair and Compress

Require the learner to state:

- The old assumption
- The evidence that broke it
- The new invariant or model
- The condition under which the old model still works
- A compressed rule usable later

### 9. Verify

Do not advance on exposure or agreement.

Verify through one or more:

- Novel prediction
- Old-model mistake detection
- Boundary explanation
- Reconstruction
- Build or repair task
- Transfer to another context
- Learner-generated diagnostic question

When the learner can generate and justify the next discriminating probe,
external question generation should begin to recede for that pattern.

### 10. Persist Selectively

Record durable model changes, not conversation volume.

Promote session claims only after verification and preserve challenged or
superseded evidence rather than overwriting it.

Persist:

- Evidence-backed belief transitions
- Reusable failure patterns
- Strong anchors
- Verified project findings
- Capability deltas

Do not persist:

- Speculation as fact
- Every response
- Fixed learner labels
- Sensitive motivational material without consent

## Outputs

Per interaction:

- One targeted probe or next action
- One evidence-backed model delta
- One compressed insight
- One verification result

Per session:

- Updated belief and concept state
- Reusable failure patterns
- Artifact progress or curriculum progress
- Optional next authentic question

Per module:

- A generative capability
- A durable artifact
- A documented model transition
- Transfer and boundary evidence

## Success Signals

- Prediction accuracy improves in changed contexts.
- The learner identifies unknowns more precisely.
- Old-model mistakes are detected before execution.
- Explanations become shorter and more generative.
- The learner transfers structures without cosmetic analogy.
- Assistance levels fall for previously learned patterns.
- Project incidents become reusable patterns.
- The learner generates the next useful probe.
- New domains take less time to model for defensible reasons.

## Boundaries

The system must not:

- Manufacture compulsion
- Use shame, fear, enemies, or identity threats
- Deliberately lie or corrupt ordinary work
- Withhold closure to create dependency
- Treat all confusion as productive
- Treat every learner as one stable type
- Advance on correct output alone
- Force teaching during urgent execution
- Turn legitimate rest or research into an avoidance diagnosis
- Pretend to remember unavailable learner history

## Universal Core vs Domain Adapter

Universal core:

- Mode selection
- Chosen-friction boundary
- Model elicitation
- Probe generation rules
- Assistance ladder
- Repair, compression, verification
- State and engagement guardrails

Domain adapter:

- Ground truth sources
- Primitives and prerequisites
- Thresholds and misconceptions
- Executable probe types
- Failure taxonomy
- Verification artifacts

Use [DOMAIN-ADAPTER-CONTRACT.md](DOMAIN-ADAPTER-CONTRACT.md) for the adapter
boundary and required evidence.

Programming is a rich adapter because code supplies types, source, tests,
runtime traces, compiler errors, and real artifacts. The core is not specific to
programming.
