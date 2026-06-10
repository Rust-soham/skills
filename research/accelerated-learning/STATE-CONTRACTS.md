# Logical State Contracts

These contracts define what the system knows and where the first version stores
it:

- Global learner context: `~/.learning/`
- Local workspace context: `<workspace>/.learning/`

## State Rule

Store evidence-backed claims, not chat history or fixed learner labels.

Every durable claim needs:

- **Claim**: the model, capability, pattern, or finding
- **Scope**: domain, mission, project, and conditions where it applies
- **Evidence**: what the learner predicted, explained, built, repaired, or
  transferred
- **Provenance**: source artifact, conversation, test, runtime observation, or
  reference
- **Status**: `candidate`, `verified`, `challenged`, or `superseded`
- **Last verification**: when and under which context it survived
- **Boundary**: where it is known not to apply

Do not use confidence numbers that imply precision the evidence does not
support.

Evidence:
[S09 global and local context](sources/S09-socrates-product-exploration.md#global-learner-context-vs-local-project-context),
[S11 model checkpoints](sources/S11-learning-system-for-trpc.md#explicit-model-checkpoints),
[S13 belief transitions](sources/S13-threshold-unlocks.md#belief-transition-graph).

## Mission

Required:

- Desired generative capability
- Why it matters
- Observable independent success
- Current constraints
- Chosen target friction
- Priority between artifact progress and deliberate curriculum

The mission changes only with learner confirmation. Record the old mission when
the change alters what evidence or curriculum is relevant.

## Learner Evidence

Store portable evidence in `~/.learning/`:

- Demonstrated anchors and their depth
- Verified model transitions
- Dead or superseded models and the condition they missed
- Recurring reasoning patterns
- Structural analogies and where they break
- Transfer and self-generated-probe evidence
- Assistance and interruption calibration

Do not store:

- Topic exposure as mastery
- Personality types inferred from a few sessions
- Unverified self-ratings as fact
- Sensitive motivational observations without opt-in

Global evidence is shared across workspaces. It may anchor analogies in a new
domain, but must retain scope and boundary. Knowing Go goroutines, for example,
is evidence for a concurrency anchor, not proof that another runtime has the
same scheduling or failure semantics.

## Model Transition

One record represents one accepted learning unit:

- Context and target capability
- Old model
- Learner's first hypothesis, interpretation, or prioritization
- Prediction or attempted action
- Probe or event
- Observation
- Failed assumption
- Repaired model or invariant
- Boundary where the old model remains useful
- Compressed rule
- Verification task and result
- Transfer evidence, if available
- Assistance level used

Create the record only after verification. Before that, keep the diagnosis in
session state.

Evidence:
[S08 compact loop](sources/S08-vscode-extension-guide.md#compact-model-repair-loop),
[S11 model delta](sources/S11-learning-system-for-trpc.md#mental-model-debugger),
[S13 unlock sequence](sources/S13-threshold-unlocks.md#unlock-sequence).

## Project

Store under `<workspace>/.learning/`:

- Artifact goal and next shippable change
- Current constraints, versions, and architecture facts
- Current blocker and evidence
- Declared target friction
- Project-specific findings with source and validity conditions
- Active sandbox question and return condition
- Last return from learning mode to artifact work

Project findings do not become global learner facts. A project incident becomes
portable only after compression and transfer.

## Storage Boundary

`~/.learning/` contains:

- `LEARNER.md`: demonstrated anchors, assistance calibration, and
  self-probing evidence
- `PATTERNS.md`: verified cross-domain reasoning and failure patterns
- `records/`: portable model transitions and supersession history

`<workspace>/.learning/` contains:

- `MISSION.md`: current capability target, success, constraints, and chosen
  friction
- `PROJECT.md`: artifact, versions, constraints, blocker, and next action
- `STATE.md`: current curriculum and unresolved local model
- `records/`: workspace-specific model transitions
- `sandboxes/`: active bounded experiments and return conditions

When promoting local evidence globally, record the originating workspace and
the transfer or reconstruction evidence. Never copy raw project context into
the global store.

## Session

Ephemeral until verified:

- Mode
- Elicited model
- First move
- Prediction
- Candidate diagnosis
- Probe
- Hint level
- Observation
- Proposed repair
- Pending verification

Discard conversational residue after promoting the verified transition and
necessary project findings.

## Evidence Lifecycle

Use:

`candidate -> verified -> challenged -> superseded`

- **Candidate**: inferred from one response or imported without current proof
- **Verified**: survived an appropriate action, prediction, reconstruction, or
  transfer test
- **Challenged**: contradicted or no longer safe to rely on in the current
  context
- **Superseded**: replaced by a more precise model; retain the link and failed
  boundary

Age alone does not make evidence stale. Revalidate when:

- The relevant domain, version, constraints, or use context changed
- New behavior contradicts the claim
- The claim will justify skipping a prerequisite
- The claim will anchor a high-leverage analogy or delegation decision

Prefer current task evidence over stored state. Never silently overwrite a
contradicted record.

## Context Integrity

Distinguish:

- Retrieved learner evidence
- Current-session evidence
- User-supplied claims
- Agent inference

If prior context is unavailable, say so and re-elicit it. Do not manufacture
continuity.

Evidence:
[S07 context integrity](sources/S07-learning-with-ai.md#context-integrity).
