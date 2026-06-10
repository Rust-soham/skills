# Candidate Skill Boundaries

These boundaries are approved for the first implementation.

## Existing Skill Fit

### `teach`

Useful:

- Mission grounding
- Stateful workspace
- Learning records
- References and resources
- Zone-of-proximal-development intent

Mismatch:

- HTML lesson is the primary unit.
- Knowledge is taught before practice.
- The transcript system's primary unit is an evidence-backed model transition,
  often inside a real artifact.
- It needs belief transitions, failed assumptions, probes, and verification,
  not only lessons and references.

Conclusion: preserve `teach`; build an adjacent system unless the user later
wants a deliberate redesign.

### `grill-me`

Useful one-question-at-a-time interaction, but it stress-tests plans rather than
diagnosing subject-matter models.

### `diagnose`

Strong reference for feedback loops, falsifiable hypotheses, one-variable
probes, and evidence before fixes. Its unit is a software bug, not a learner
belief.

### `zoom-out`

Useful programming operation for restoring system context. It is one possible
environment transformation, not the learning orchestrator.

### `scaffold-exercises`

Mechanical course-directory generation. It does not design diagnostic
exercises.

## Minimal Candidate Set

### 1. Stateful Learning Orchestrator

Working name: `learn-deeply`

Responsibility:

- Establish mission and target friction
- Select mode
- Assemble global, mission, project, and domain context
- Run model-repair sessions
- Persist verified belief transitions
- Fade assistance as self-probing improves

Primary unit: one verified model transition.

Primary learning modes:

- Development: shortest blocker-to-artifact path
- Research: recursive, FAFO-heavy compounding threshold path

Delegation and production rescue remain execution overrides.

This is the universal core. **Socrates** can remain the product or system name
without weakening skill discoverability.

### 2. Curriculum Designer

Working name: `design-learning-path`

Responsibility:

- Autopsy a domain
- Identify primitives, prerequisites, thresholds, and common limiting models
- Order transformations by leverage
- Define artifacts and generative gates
- Produce or update a domain adapter

Primary unit: one threshold module in a leverage graph.

This should remain separate because designing a curriculum is a different task
from teaching one learner in real time.

The skills still form one loop: `design-learning-path` always chooses the active
edge, even when the path has one edge; `learn-deeply` executes it and returns
learner evidence that can change the remaining path.

## Programming as a Conditional Adapter

Do not create `learn-while-building` initially.

When the universal orchestrator detects a software artifact or an explicit
build mission, it should load a one-level programming reference that adds:

- Local code, versions, diagnostics, source, tests, and runtime evidence
- Target-versus-incidental friction classification
- Project-to-sandbox transition and return conditions
- Blocker-to-artifact-progress rhythm
- Production constraints and comparative implementation review
- Crystallization of incidents into transferable patterns
- Development and research mode implementations

Reason: "teach me this while we build it" would trigger both a universal
learning skill and a programming learning skill. One orchestrator with a
conditional adapter preserves a single owner for mode, state, assistance, and
verification.

Split the adapter into a standalone skill only if usage establishes:

- A distinct invocation that does not also require the orchestrator
- A distinct durable artifact
- A separate evaluation contract

## Possible Internal Operations, Not Initial Skills

- Diagnose current model
- Generate controlled collision
- Run inversion sequence
- Select progressive hint
- Crystallize model delta
- Transfer pattern
- Review unknown unknowns
- Shape the learning environment

Keep these inside the two primary skills initially. Split one out only if it
becomes independently invoked, has a distinct artifact, or accumulates enough
rules to obscure the parent skill.

## Domain Adapters, Not Skills

Store domain-specific material as references or data:

- Ground-truth sources
- Prerequisite and threshold maps
- Misconception patterns
- Probe templates
- Verification criteria

A Rust adapter and an organizational-design adapter should use the same
learning engine without pretending their domain models are interchangeable.

Use [DOMAIN-ADAPTER-CONTRACT.md](DOMAIN-ADAPTER-CONTRACT.md) as the logical
format. It remains independent of learner and project state.

## Suggested Workspace Artifacts

Names are provisional:

```text
.learning/
├── MISSION.md
├── LEARNER.md
├── PATTERNS.md
├── domains/
│   └── <domain>.md
├── missions/
│   └── <mission>/
│       ├── STATE.md
│       ├── CURRICULUM.md
│       └── records/
└── projects/
    └── <project>/
        ├── CONTEXT.md
        ├── FINDINGS.md
        └── records/
```

For version one:

- Global learner evidence lives in `~/.learning/` and follows the learner
  across workspaces.
- Local mission and project evidence lives in `<workspace>/.learning/`.
- Project facts become global only after compression and transfer evidence.
- Sensitive motivational state remains opt-in.

The logical fields and lifecycle are defined in
[STATE-CONTRACTS.md](STATE-CONTRACTS.md).

## Shape Rules From This Repository

When drafting eventually:

- Put the trigger and behavioral contract in the description.
- Keep one primary unit per skill.
- Use sharp positive and negative rules.
- Define required artifacts and gates.
- Put long domain material in one-level references.
- Avoid pedagogy essays in `SKILL.md`.
- Include examples only when they distinguish close behaviors.
- Prefer observable completion criteria over aspirational language.

See [REFERENCE-SHAPE.md](REFERENCE-SHAPE.md) for the evidence behind these
rules.

Use [EVALUATION-SCENARIOS.md](EVALUATION-SCENARIOS.md) to test the boundary
before splitting internal modes into more skills.
