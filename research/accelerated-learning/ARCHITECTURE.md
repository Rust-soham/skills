# Candidate Architecture

This is a conceptual architecture derived from the corpus. It is not an
implementation plan or a skill draft.

## Components

### Mission Controller

Defines the desired capability, why it matters, independent success criteria,
and current constraints.

### Mode Router

Chooses development or research mode, then applies delegation or rescue when
needed. Prevents open exploration from delaying artifact return and learning
rules from blocking legitimate execution.

### Context Assembler

Builds the smallest useful context from:

- Global learner evidence
- Current mission
- Local project state
- Domain adapter
- Current session

It prefers the delta between known and needed information over a full history.

### Evidence Grounder

Retrieves the strongest available reality signal. In programming this may use
code, diagnostics, tests, runtime values, installed package source, and
version-matched documentation.

### Learner Model

Stores evidence-backed beliefs rather than a flat known/unknown score.

A belief record needs:

- Claim or model
- Evidence and context
- Confidence
- Known boundary
- Prior model
- Last verification
- Transfer evidence

### Bifocal Model Comparator

Compares learner evidence with the domain graph to identify the smallest
high-leverage belief transition. It keeps learner placement, domain truth, and
candidate diagnosis distinct.

### Domain Model

Stores:

- Prerequisite relations
- High-leverage thresholds
- Candidate thresholds and their grounding status
- Invariants
- Common limiting models
- Candidate collisions
- Verification criteria

It is independent from the learner model. The learner may reach the same domain
node through a different misconception path.

### Threshold Miner

When the domain graph is incomplete, compares varied cases, strips surface
differences, rotates representations, and proposes invariants that could explain
multiple cases. Its outputs remain hypotheses until grounded in domain evidence
and verified through changed learner behavior.

### Diagnostic Engine

Infers candidate beliefs from a learner response and ranks the most upstream
gap. It separately checks the object-level domain model and the meta-level
reasoning process. It must expose uncertainty instead of pretending to read the
learner's mind.

### Curriculum Planner

Selects the highest-leverage reachable transformation. It plans at module scale
and may insert prerequisite repair, integration, transfer, or spacing.

### Environment Shaper

Reduces incidental complexity through isolation, decomposition, observability,
or a temporary sandbox.

Use [OPERATIONAL-HEURISTICS.md](OPERATIONAL-HEURISTICS.md) for project-to-sandbox
and return gates.

### Probe Generator

Creates a task that the current model can attempt but one target assumption
cannot survive.

### Interaction Controller

Enforces prediction gates, progressive hints, learner response, and appropriate
silence during productive work. It protects the learner's first hypothesis or
interpretation while allowing the agent to choose the diagnostic situation.

### Feedback Loop Controller

Reduces randomness, isolates one changing variable, shortens evidence latency,
and detects when repetition is aimed at the wrong bottleneck. It optimizes
informative iterations, not interaction count.

### Evaluator

Separates:

- Outcome correctness
- Model quality
- Boundary awareness
- Transfer
- Independence

### Recorder

Persists accepted model transitions, project findings, patterns, artifacts, and
verification evidence. It does not save every conversational claim.

Use [STATE-CONTRACTS.md](STATE-CONTRACTS.md) for claim scope, evidence lifecycle,
and context integrity.

### Engagement Guardrail

Uses visible capability growth and meaningful work to support return. Blocks
coercive engagement tactics and watches for fatigue, dependency, or avoidance.

## State Boundaries

### Global

Stored under `~/.learning/` and portable across workspaces:

- Strong anchors
- Cross-domain reasoning patterns
- Assistance calibration
- Self-probing evidence

### Mission

Stored under `<workspace>/.learning/` and portable across sessions within one
learning objective:

- Capability target
- Curriculum position
- Threshold history
- Artifacts and gates

### Project

Stored under `<workspace>/.learning/` and bound to one codebase or artifact:

- Versions, code, diagnostics, findings
- Architecture and constraints
- Current feature and blocker

### Session

Ephemeral until verified:

- Candidate diagnosis
- Predictions
- Probe attempts
- Unaccepted model updates

## Main Flows

### Research

`mission -> diagnose -> plan threshold -> shape environment -> probe -> repair
-> verify -> integrate -> persist`

### Development

`artifact goal -> attempt -> blocker -> classify friction -> ground -> isolate
-> plan minimum dependency path -> repair -> return to artifact -> ship ->
crystallize`

### Unknown-Unknown Review

`current model -> boundary inventory -> expert/adjacency probes -> reproduce
evidence -> update model or record defended boundary`

### Delegation

`task -> auditability check -> delegate implementation -> review against model
and constraints -> record only novel patterns`

## Programming Adapter

Potential evidence tools:

- LSP hover, definition, references, call hierarchy, and diagnostics
- Compiler and type-checker output
- Tests and minimal reproductions
- Debugger and runtime traces
- Installed package source and type declarations
- Official, version-matched documentation
- Project-local knowledge with source and confidence

Potential probe forms:

- Predict output or type
- Remove a dependency or step
- Change ordering or timing
- Duplicate or retry an event
- Introduce a failure between operations
- Compare two implementations
- Generalize repeated code into a primitive
- Apply one model to an adjacent subsystem

## Design Risks

- Treating model inference as certainty
- Building a giant ontology before validating probes
- Polluting global state with project-specific facts
- Allowing stale proficiency to drive bad analogies
- Generating technically false collisions
- Optimizing visible progress instead of genuine transfer
- Letting curriculum work become an escape from shipping
- Letting shipping erase reflection and compression

## Validation Order

1. Exact-gap diagnosis from a learner response
2. One targeted probe with progressive hints
3. Model-delta capture and novel verification
4. Local project grounding and return-to-artifact flow
5. Durable learner state and analogy retrieval
6. Threshold curriculum planning
7. Cross-domain transfer and metacognitive adaptation

This order follows the user's stated short-term priority and delays the most
speculative infrastructure.
