# Structural Analogy and Isomorphism

**Status:** Core

## Core Claim

Use a demonstrated strong model as an anchor, then teach only the structural
delta: shared roles, constraints, causal relations, state transitions, and
failure patterns.

## Analogy Contract

1. Verify that the learner can reason with the anchor.
2. Name the shared structure.
3. Name the new-domain differences.
4. Predict with the analogy.
5. Probe where it fails.
6. Replace it when domain-specific structure becomes more generative.

## Good Transfer

Good analogy preserves causal organization. Cosmetic similarity, shared
vocabulary, or surface syntax is not enough.

Examples of transferable structure:

- Ownership and lifecycle
- Scheduling and coordination
- State transition and invalid states
- Retry and failure semantics
- Constraint preservation

## Boundaries

- Analogy is a provisional model, not an explanation endpoint.
- Revalidate stale or high-leverage anchors.
- Knowing one concurrency model does not prove another runtime shares its
  scheduling or failure semantics.

## Sources

[S04](../sources/S04-cognitive-scaffolding-shift.md),
[S06](../sources/S06-ai-in-dev-workflows.md),
[S07](../sources/S07-learning-with-ai.md),
[S09](../sources/S09-socrates-product-exploration.md),
[S11](../sources/S11-learning-system-for-trpc.md),
[S13](../sources/S13-threshold-unlocks.md).

## Related

[Compression](09-compression-and-pattern-extraction.md),
[Multi-Scope State](14-multi-scope-durable-state.md),
[Scaffolding Without Dependency](18-scaffolding-without-epistemic-dependency.md).

Runtime:
[learn-deeply](../../../skills/mine/exponential/learn-deeply/SKILL.md).
