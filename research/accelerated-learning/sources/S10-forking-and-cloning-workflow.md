# S10: Forking and Cloning Workflow

Source: `transcripts/Forking and Cloning Workflow.md`

Status: cross-checked

## Evidence Notes

### Source Authority Within the Transcript

The learning-relevant material is concentrated in the opening workflow
inversion and the final attempt to encode the behavior as an agent rule. The
middle discussion about AI labor markets is topical drift and does not add a
distinct learning mechanism.

### Omitted-Step Inversion

The user's request is not for the normal contribution workflow alone. They ask
for every step to be removed or inverted and for the resulting failure to be
traced
([11-35](../../../transcripts/Forking%20and%20Cloning%20Workflow.md#L11)).

The transcript applies this to:

- No fork: the learner lacks a writable remote.
- Fork but clone the upstream repository: the local `origin` still points to a
  remote the learner cannot write.
- No feature branch: unrelated work accumulates and the change boundary becomes
  unstable.
- No push: the remote has no branch from which to open a pull request.
- No pull request: the change never enters the review and merge process.

([41-235](../../../transcripts/Forking%20and%20Cloning%20Workflow.md#L41))

`SOURCE`: The omission test reveals each step's causal responsibility. The
learner does not memorize "fork, clone, branch, push, PR"; they understand which
permission, isolation, transport, or coordination problem each step solves.

### Compression After Failure Simulation

After exploring failures, the workflow is compressed into:

`read-only upstream -> writable fork -> local workspace -> one-idea branch ->
upload -> merge request`

([261-284](../../../transcripts/Forking%20and%20Cloning%20Workflow.md#L261)).

Common symptoms are then mapped back to missing or incorrect steps, such as a
failed push, unexpectedly large pull request, or absent pull-request action
([288-315](../../../transcripts/Forking%20and%20Cloning%20Workflow.md#L288)).

`SYNTHESIS`: A strong inversion exercise has three phases:

1. Remove or reverse one operation.
2. Predict the first broken invariant and downstream symptom.
3. Recompress the operation by the responsibility it restores.

### Context-Dependent Necessity

The transcript later notes that a fork is one permission strategy rather than a
universal Git requirement. Collaborators with direct write access may use
branches in the upstream repository
([318-330](../../../transcripts/Forking%20and%20Cloning%20Workflow.md#L318)).

`REFINEMENT`: Inversion must ask "under which constraints is this step
necessary?" A deleted step may be harmless when another mechanism preserves the
same invariant.

### Agent Behavior Proposed at the End

The final rule restates several corpus-wide behaviors:

- Ask for the current model and a prediction.
- Remove lookup, syntax, setup, and boilerplate friction.
- Add assumption, why, edge-case, and failure-scenario friction.
- Use progressive hints.
- Extract a reusable rule.
- Measure success by unaided prediction.

([844-911](../../../transcripts/Forking%20and%20Cloning%20Workflow.md#L844))

The transcript also says that when the learner has not supplied a current model,
the agent should request it before proceeding
([915-947](../../../transcripts/Forking%20and%20Cloning%20Workflow.md#L915)).

`QUESTION`: This should not be unconditional. For urgent execution, trivial
lookup, or a learner who cannot yet form a model, forcing elicitation may add
friction without diagnostic value.

### Durable State Suggested by the Source

- Workflow operations
- Invariant protected by each operation
- Preconditions under which each operation is necessary
- Failure caused by omission or reversal
- Observable symptom of that failure
- Substitute mechanisms preserving the same invariant
- Compressed causal workflow

### Signals

- Learner predicts what fails when a step is omitted
- Learner distinguishes the first broken invariant from downstream symptoms
- Learner can map a symptom back to the likely missing operation
- Learner identifies when a step is optional because constraints differ
- Learner restates steps as responsibilities rather than commands

### Failure Modes

- Memorizing a happy-path sequence
- Treating one implementation of an invariant as universally required
- Showing failures without asking for a prediction
- Confusing symptoms with root causes
- Inverting several steps at once
- Ending without a compressed causal model

### Refinements and Tensions

`REFINEMENT`: S09's general inversion questions become a concrete
decision-tree protocol for procedural workflows.

`REFINEMENT`: "What breaks without this?" should be paired with "what else
could preserve the same invariant?" to prevent ritualized rules.

`QUESTION`: The final agent rule says to shift mechanical questions toward
conceptual principles. Sometimes the user's chosen friction is deliberately
mechanical; the agent should follow the declared learning target rather than
always privileging abstraction.
