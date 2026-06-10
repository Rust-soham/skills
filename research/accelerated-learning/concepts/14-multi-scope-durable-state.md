# Multi-Scope Durable State

**Status:** Core

## Core Claim

Persist evidence-backed claims at the scope where they remain valid. Separate
portable learner evidence, local mission and project facts, domain truth, and
ephemeral session hypotheses.

## Scopes

### Global Learner

- Demonstrated anchors and depth
- Verified model transitions and dead models
- Recurring reasoning patterns
- Analogy bridges and failure boundaries
- Transfer and self-probing evidence
- Assistance calibration

### Local Mission and Project

- Capability target and independent success
- Artifact, versions, constraints, and architecture
- Current blocker, model, and target friction
- Project findings and sandbox return conditions

### Domain Adapter

- Primitives, invariants, and prerequisites
- Threshold graph and limiting models
- Failure modes, probes, and verification criteria

### Session

- Prediction, candidate diagnosis, probe, hint level, and unverified repair

## Evidence Contract

Every durable claim needs scope, evidence, provenance, status, boundary, and
last verification. Use `candidate -> verified -> challenged -> superseded`.

## Boundaries

- Current evidence overrides stale state.
- Never fabricate unavailable context.
- Promote local findings globally only after compression and transfer.
- Sensitive motivational state requires opt-in.

## Sources

[S04](../sources/S04-cognitive-scaffolding-shift.md),
[S07](../sources/S07-learning-with-ai.md),
[S08](../sources/S08-vscode-extension-guide.md),
[S09](../sources/S09-socrates-product-exploration.md),
[S11](../sources/S11-learning-system-for-trpc.md),
[S13](../sources/S13-threshold-unlocks.md),
[S16](../sources/S16-friction-avoidance-hell.md).

## Related

[Compression](09-compression-and-pattern-extraction.md),
[Structural Analogy](10-structural-analogy-and-isomorphism.md),
[Persistent context tension](../TENSIONS.md#18-persistent-context-vs-privacy-and-staleness).

Runtime:
[state format](../../../skills/productivity/learn-deeply/WORKSPACE-FORMAT.md),
[path format](../../../skills/productivity/design-learning-path/PATH-FORMAT.md).
