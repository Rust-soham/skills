# Controlled Collision and Inversion

**Status:** Core

## Core Claim

A diagnostic exercise should be solvable enough to engage the current model,
then make one limiting assumption fail visibly.

## Collision Shape

`baseline -> near boundary -> breaking case -> minimal reframe -> novel test`

The baseline confirms the old model's useful range. The breaking case supplies
causal evidence. The reframe should be no larger than the mismatch requires.

## Inversion Operators

- Remove a step and trace the first broken invariant.
- Reverse a choice and compare consequences.
- Ask what the construct protects against.
- Present an adjacent plausible solution and find its failure.
- Ask which constraints make the observed design necessary.
- Find a substitute that preserves the same invariant.
- Change one variable, ordering, timing, retry, or failure point.

## Quality Test

A strong collision:

- Targets one belief
- Requires a prediction
- Produces inspectable evidence
- Preserves enough context for the result to transfer
- Does not depend on a hidden trick or deliberate lie

## Sources

[S06](../sources/S06-ai-in-dev-workflows.md),
[S07](../sources/S07-learning-with-ai.md),
[S08](../sources/S08-vscode-extension-guide.md),
[S09](../sources/S09-socrates-product-exploration.md),
[S10](../sources/S10-forking-and-cloning-workflow.md),
[S13](../sources/S13-threshold-unlocks.md).

## Related

[Atomic Model Repair](04-atomic-model-repair-loop.md),
[Threshold Engineering](08-threshold-and-unlock-engineering.md),
[Environment Transformations](17-environment-transformations.md).

Runtime:
[learn-deeply](../../../skills/mine/exponential/learn-deeply/SKILL.md),
[programming adapter](../../../skills/mine/exponential/learn-deeply/PROGRAMMING.md).
