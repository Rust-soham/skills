# Cross-Source Concept Index

This index deduplicates recurring ideas without erasing later refinements.
Source notes remain the traceable evidence layer.

For standalone concept cards with mechanisms, boundaries, relationships, and
runtime homes, use the [concept library](concepts/README.md).

Status meanings:

- **Core**: repeatedly supported and necessary to the system
- **Contextual**: useful under a particular mission or learner state
- **Candidate**: plausible operator requiring further validation
- **Rejected**: conflicts with the learning objective or trust boundary

## 1. Learner-Owned Model Construction

**Status:** Core

The learner must produce, test, and revise the mental model. AI may choose the
environment, retrieve evidence, and design probes, but borrowed conclusions are
not the target.

Evolution:

- S03 and S04 define the cognition boundary.
- S05 and S06 make assistance and delegation adaptive.
- S07 makes AI an active Socratic probe designer.
- S09 and S13 define the terminal state as self-probing and independent model
  repair.

Sources:
[S03](sources/S03-ai-and-cognitive-softness.md),
[S04](sources/S04-cognitive-scaffolding-shift.md),
[S05](sources/S05-delayed-growth.md),
[S06](sources/S06-ai-in-dev-workflows.md),
[S07](sources/S07-learning-with-ai.md),
[S09](sources/S09-socrates-product-exploration.md),
[S13](sources/S13-threshold-unlocks.md).

## 2. Chosen Friction

**Status:** Core

Preserve resistance that changes the target model. Remove resistance that only
consumes attention through retrieval, syntax, boilerplate, setup, formatting,
or already-understood mechanics.

Refinement:

- The learner declares what they are trying to own.
- The agent identifies incidental load around it.
- The split is dynamic: today's model-building work may become tomorrow's
  delegable labor.
- Avoidance of the selected friction is itself a learning signal.

Sources:
[S03](sources/S03-ai-and-cognitive-softness.md),
[S04](sources/S04-cognitive-scaffolding-shift.md),
[S05](sources/S05-delayed-growth.md),
[S09](sources/S09-socrates-product-exploration.md),
[S11](sources/S11-learning-system-for-trpc.md),
[S16](sources/S16-friction-avoidance-hell.md).

## 3. Evidence-Based Model Diagnosis

**Status:** Core

Do not begin from a self-rating or assumed learner level. Use a small applied
task, causal walkthrough, prediction, comparison, or explanation that reveals
the model producing the response.

The diagnostic phase is already instruction because externalizing a belief can
expose contradictions.

Sources:
[S07](sources/S07-learning-with-ai.md),
[S08](sources/S08-vscode-extension-guide.md),
[S09](sources/S09-socrates-product-exploration.md),
[S13](sources/S13-threshold-unlocks.md).

## 4. Atomic Model-Repair Loop

**Status:** Core

Canonical exercise loop:

`elicit model -> predict -> run targeted case -> observe mismatch -> identify
failed assumption -> minimally repair -> compress -> verify`

The loop should produce inspectable evidence, not merely a correct answer.

Sources:
[S04](sources/S04-cognitive-scaffolding-shift.md),
[S05](sources/S05-delayed-growth.md),
[S06](sources/S06-ai-in-dev-workflows.md),
[S08](sources/S08-vscode-extension-guide.md),
[S11](sources/S11-learning-system-for-trpc.md),
[S13](sources/S13-threshold-unlocks.md).

## 5. Controlled Collision and Inversion

**Status:** Core

A targeted exercise should be solvable enough that the current model engages,
yet constructed so one limiting assumption fails visibly.

Inversion variants:

- Remove a step and trace the first broken invariant.
- Reverse a choice and compare consequences.
- Ask what the construct protects against.
- Find the adjacent plausible solution and why it fails.
- Ask what constraints make the observed design necessary.
- Ask what substitute could preserve the same invariant.

Sources:
[S06](sources/S06-ai-in-dev-workflows.md),
[S07](sources/S07-learning-with-ai.md),
[S08](sources/S08-vscode-extension-guide.md),
[S09](sources/S09-socrates-product-exploration.md),
[S10](sources/S10-forking-and-cloning-workflow.md),
[S13](sources/S13-threshold-unlocks.md).

## 6. Progressive Scaffolding

**Status:** Core

Assistance escalates from nudge to structured hint, partial structure, and full
solution only when needed. The level depends on evidence of progress,
prerequisite sufficiency, urgency, and whether the target model is already
owned.

The agent can reduce overload before revealing an answer by:

- Isolating one variable
- Naming what to ignore
- Retrieving exact evidence
- Providing a skeleton
- Moving to a smaller sandbox

Sources:
[S03](sources/S03-ai-and-cognitive-softness.md),
[S05](sources/S05-delayed-growth.md),
[S06](sources/S06-ai-in-dev-workflows.md),
[S07](sources/S07-learning-with-ai.md),
[S15](sources/S15-matt-pocock-post.md).

## 7. Curriculum as Leverage Architecture

**Status:** Core

A curriculum is a graph of transformations ordered by what unlocks future
learning, not a topic inventory or a universal easy-to-hard list. Its design
target is the steepest defensible compounding curve: each threshold increases
current competency while reducing the cost and increasing the rate of later
learning.

Curriculum-scale sequence:

1. Map the domain and expert perception.
2. Establish sufficient substrate models.
3. Target a high-leverage reachable threshold.
4. Practice under causally relevant use conditions.
5. Recontextualize prior knowledge through the new lens.
6. Integrate, transfer, and produce durable evidence.

Every threshold edge must name how earlier foundations are reused, which future
friction is removed, which successors become easier, and how the environment
makes the correct next action the easiest path.

Sources:
[S01](sources/S01-actual-roadmap.md),
[S02](sources/S02-elite-hacker-roadmap.md),
[S09](sources/S09-socrates-product-exploration.md),
[S13](sources/S13-threshold-unlocks.md).

## 8. Threshold and Unlock Engineering

**Status:** Core at module scale

An unlock is a model transition that reorganizes perception, compresses prior
facts, reveals new relations, and enables novel action. It often replaces a
locally useful but limiting model rather than a simply false one.

Exercise-scale transition:

`baseline -> near-boundary -> breaking case -> minimal reframe -> novel
verification`

Crossing evidence:

- Explain the old and new models
- Identify where the old model breaks
- Detect old-model mistakes in unseen cases
- Build, repair, or predict with the new model
- Connect previously separate ideas

Sources:
[S01](sources/S01-actual-roadmap.md),
[S02](sources/S02-elite-hacker-roadmap.md),
[S05](sources/S05-delayed-growth.md),
[S12](sources/S12-energy-and-engagement.md),
[S13](sources/S13-threshold-unlocks.md).

Not every supporting fact or fluency drill needs its own threshold.

## 9. Compression and Pattern Extraction

**Status:** Core

After a repair, extract:

- The failed assumption
- The invariant that survived variation
- The compressed rule
- The abstract failure pattern
- Other contexts where it may appear

This converts experiences into a reusable pattern library and reduces working
memory cost on later problems.

Sources:
[S01](sources/S01-actual-roadmap.md),
[S02](sources/S02-elite-hacker-roadmap.md),
[S04](sources/S04-cognitive-scaffolding-shift.md),
[S08](sources/S08-vscode-extension-guide.md),
[S09](sources/S09-socrates-product-exploration.md),
[S10](sources/S10-forking-and-cloning-workflow.md),
[S11](sources/S11-learning-system-for-trpc.md).

## 10. Structural Analogy and Isomorphism

**Status:** Core

Start from a demonstrated strong anchor and explain only the structural delta:
shared roles, constraints, causal relations, state transitions, or failure
patterns. Then probe where the analogy breaks.

Analogy is a provisional model and a transfer test, not an explanation endpoint.

Sources:
[S04](sources/S04-cognitive-scaffolding-shift.md),
[S06](sources/S06-ai-in-dev-workflows.md),
[S07](sources/S07-learning-with-ai.md),
[S09](sources/S09-socrates-product-exploration.md),
[S11](sources/S11-learning-system-for-trpc.md),
[S13](sources/S13-threshold-unlocks.md).

## 11. Unknown-Unknown Discovery

**Status:** Core

Unknown unknowns become visible through:

- Outside-frame stress tests
- Boundary and pathological cases
- Adjacent-domain questions
- Expert review questions the learner did not generate
- Production failures and postmortems
- Alternative implementations

The learner must reproduce or inspect the evidence rather than accept a list of
possible failures.

Sources:
[S06](sources/S06-ai-in-dev-workflows.md),
[S07](sources/S07-learning-with-ai.md),
[S09](sources/S09-socrates-product-exploration.md).

## 12. Real Project and Toy World Oscillation

**Status:** Core

Real projects supply stakes, authentic constraints, integration, and failures.
Toy worlds supply causal clarity, safety, and one-variable experiments.

The system should move from project to sandbox when confounding variables,
risk, or missing primitives prevent diagnosis. It should return once the
isolated model survives verification.

Sources:
[S02](sources/S02-elite-hacker-roadmap.md),
[S06](sources/S06-ai-in-dev-workflows.md),
[S09](sources/S09-socrates-product-exploration.md),
[S11](sources/S11-learning-system-for-trpc.md),
[S15](sources/S15-matt-pocock-post.md),
[S16](sources/S16-friction-avoidance-hell.md).

## 13. Dynamic AI Mode and Delegation Boundary

**Status:** Core

The learning engine needs two primary modes:

- **Development**: repair the shortest unfamiliar-concept dependency chain that
  unblocks the next artifact action, then return to building.
- **Research**: recursively explore why chains, primitives, invariants,
  boundaries, alternatives, and unknown unknowns through broader FAFO.

Delegation and production rescue are execution overrides. Delegation grows with
demonstrated auditability, not time or confidence. Rescue prioritizes safety and
completion, then reconstructs learning afterward.

Sources:
[S03](sources/S03-ai-and-cognitive-softness.md),
[S05](sources/S05-delayed-growth.md),
[S06](sources/S06-ai-in-dev-workflows.md),
[S07](sources/S07-learning-with-ai.md),
[S11](sources/S11-learning-system-for-trpc.md),
[S16](sources/S16-friction-avoidance-hell.md).

## 14. Multi-Scope Durable State

**Status:** Core

Global learner state:

- Demonstrated anchors and proficiency evidence
- Belief transitions and dead models
- Recurring reasoning failures
- Helpful analogies and their boundaries
- Transfer and self-probing evidence
- Assistance and interruption calibration

Local mission or project state:

- Current artifact, goal, and constraints
- Installed versions, code, runtime evidence, and diagnostics
- Current model, blocker, and load-bearing gap
- Project-specific findings with provenance and confidence
- Next shippable or diagnostic action

Domain adapter state:

- Primitives and prerequisites
- Threshold graph
- Common misconceptions
- Failure modes and executable probes
- Verification criteria

Sources:
[S04](sources/S04-cognitive-scaffolding-shift.md),
[S07](sources/S07-learning-with-ai.md),
[S08](sources/S08-vscode-extension-guide.md),
[S09](sources/S09-socrates-product-exploration.md),
[S11](sources/S11-learning-system-for-trpc.md),
[S13](sources/S13-threshold-unlocks.md),
[S16](sources/S16-friction-avoidance-hell.md).

## 15. Engagement Through Earned Capability

**Status:** Core with contextual personalization

The durable positive loop is:

`meaningful challenge -> specific mismatch -> learner-owned repair -> visible
capability delta -> increased willingness to re-engage`

Useful support includes real projects, clear immediate success criteria,
adaptive difficulty, visible before-and-after performance, craft identity, and
high-quality reference work.

Sources:
[S07](sources/S07-learning-with-ai.md),
[S08](sources/S08-vscode-extension-guide.md),
[S09](sources/S09-socrates-product-exploration.md),
[S12](sources/S12-energy-and-engagement.md),
[S16](sources/S16-friction-avoidance-hell.md).

Rejected:

- Shame, insults, or identity threats
- Manufactured enemies or fear
- Punitive streaks
- Deliberate lies or random hidden defects
- Forced incompleteness
- Compulsion as a success metric

## 16. Artifact Contact and Avoidance Detection

**Status:** Contextual but important for build missions

For avoidance-prone learning, the project is a behavioral rail. Learning should
advance a concrete artifact, and the system should notice when planning,
research, refactoring, or abstraction becomes an escape from the selected
friction.

The detector must remain humble: rest, scope correction, and genuine blockers
are not avoidance by default.

Sources:
[S14](sources/S14-thdxr-post.md),
[S15](sources/S15-matt-pocock-post.md),
[S16](sources/S16-friction-avoidance-hell.md).

## 17. Environment Transformations

**Status:** Candidate curriculum operators

Before increasing difficulty, change the environment:

- **Isolate** one primitive or variable.
- **Split** a knot into independent responsibilities.
- **Elevate** to the broader problem generating several symptoms.
- **Enable** the target through a preparatory change.
- **Ground** claims in source, types, tests, or runtime evidence.

These operations reduce incidental complexity while preserving the target
model-building work.

Sources:
[S06](sources/S06-ai-in-dev-workflows.md),
[S11](sources/S11-learning-system-for-trpc.md),
[S14](sources/S14-thdxr-post.md),
[S15](sources/S15-matt-pocock-post.md).

## 18. Scaffolding Without Epistemic Dependency

**Status:** Core

External tools can increase output while weakening internal navigability. The
system must therefore distinguish successful orchestration from understanding
and periodically require prediction, reconstruction, judgment, or recovery
without the scaffold.

The same trust rule applies to learner context: retrieved state, current
conversation evidence, and inference must remain distinguishable. The agent
must never manufacture remembered history when context is unavailable.

Sources:
[S03](sources/S03-ai-and-cognitive-softness.md),
[S04](sources/S04-cognitive-scaffolding-shift.md),
[S07](sources/S07-learning-with-ai.md),
[S09](sources/S09-socrates-product-exploration.md).

## 19. Comparative Taste and Constraint Artifacts

**Status:** Core for build missions

Taste is trained by comparing plausible alternatives against explicit
requirements, non-goals, invariants, failure behavior, and maintenance costs.
High-quality reference work supplies calibration; the learner must still state
why a design fits the present constraints.

Sources:
[S02](sources/S02-elite-hacker-roadmap.md),
[S06](sources/S06-ai-in-dev-workflows.md),
[S09](sources/S09-socrates-product-exploration.md).
