# Repository Reference Shape

## Evidence Set

Primary references:

- `skills/other/productivity/teach/`
- `skills/other/engineering/diagnose/`
- `skills/other/productivity/grill-me/`
- `skills/other/engineering/zoom-out/`
- `skills/other/engineering/prototype/`
- `skills/other/engineering/tdd/`
- `skills/other/productivity/handoff/`

`teach` supplies the closest state model. The neighboring skills reveal the
repository's stronger instruction style.

## Style Pattern

### Trigger in Metadata

The description names the capability and concrete invocation conditions.
Trigger logic does not need to be repeated in the body.

### One Governing Unit

Strong skills organize around one unit:

- `diagnose`: one reproduced and regression-tested failure
- `prototype`: one question answered by throwaway code
- `grill-me`: one decision branch resolved at a time
- `teach`: one tightly scoped lesson

For the transcript system, the governing unit is one **verified model
transition**.

### Lead With the Operational Thesis

The strongest files state the controlling rule early:

- Build the feedback loop before diagnosis.
- A prototype answers a question.
- Ask one question at a time.

The learning skill should begin with:

> The learner constructs the model. The agent engineers and verifies the next
> model transition.

### Phases Need Gates

Phases are useful only when advancement has observable conditions. Good
instructions say:

- Do not hypothesize before reproducing.
- Do not advance on exposure or agreement.
- Return to the artifact after the isolated model survives verification.

### Artifacts Carry State

Durable files replace repeated prose. `teach` already demonstrates:

- Mission state
- Learning records
- Trusted resources
- Canonical vocabulary

The transcript system adds:

- Current and prior model
- Failed assumption
- Probe and prediction
- Verification evidence
- Transfer and boundary evidence
- Local project findings with provenance

### Negative Rules Protect the Unit

Strong negative rules block close but harmful behavior:

- Do not teach several things at once.
- Do not infer understanding from correct output.
- Do not provide a full solution before the target learning value is exhausted.
- Do not manufacture remembered context, confusion, or compulsion.

### Progressive Disclosure

Keep universal behavior in `SKILL.md`. Load one-level references only when a
mode or domain requires them:

- Programming and project grounding
- Curriculum design
- State formats
- Probe operators

Do not duplicate a rule in both the skill and a reference.

### Compression Standard

Keep a sentence only when it changes:

- Triggering
- Mode selection
- Next action
- State
- Assistance
- Verification
- Safety or trust boundaries

Historical derivation, motivational rhetoric, and theory names belong in the
research archive, not the skill.

## Existing `teach` Fit

Preserve:

- Mission grounding
- Stateful workspace
- Evidence-backed learning records
- Trusted resources
- Canonical glossary
- Tight feedback loops
- Real-world practice and community

Replace or subordinate:

- HTML lesson as the primary unit
- Knowledge-first sequencing
- Topic coverage as evidence of progress
- Zone placement inferred mainly from records

The transcript system begins from learner evidence, chooses a model transition,
and uses explanation only when it is the minimum useful intervention. A lesson
may be an output, but it is not the engine.

## Boundary Implication

Skills are trigger surfaces, not every internal operation. A separate
programming skill would overlap with the universal orchestrator whenever a user
wants to learn while building. Start with:

1. One universal model-transition orchestrator with internal modes and
   conditional programming references.
2. One curriculum-design skill whose artifact is a leverage-ordered threshold
   graph.

Split programming into its own skill only after usage demonstrates an
independent invocation, artifact, and evaluation contract.
