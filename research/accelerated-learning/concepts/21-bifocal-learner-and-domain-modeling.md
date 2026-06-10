# Bifocal Learner and Domain Modeling

**Status:** Core

## Core Claim

Effective tutoring needs two simultaneous models:

- The learner's evidenced beliefs, anchors, gaps, and current representation
- The domain's primitives, dependencies, thresholds, invariants, and target
  capabilities

The next exercise is selected by comparing them. Learner modeling without an
expert destination mirrors confusion; domain expertise without a learner model
targets the right concept at the wrong level.

## Procedure

1. Autopsy expert perception, domain primitives, invariants, and use
   conditions.
2. Reconstruct the learner model from an applied response.
3. Locate the corresponding region of the domain or threshold graph.
4. Identify the smallest high-leverage belief transition between them.
5. Design one collision that the learner's current model can attempt.
6. Use the result to update learner position and, when necessary, the domain's
   misconception or threshold map.

Existing learner strengths may shorten or reorder the path. Use them only when
demonstrated, and preserve the semantic differences between the old anchor and
the new domain.

## State Separation

Keep distinct:

- Domain truth and prerequisite hypotheses
- Learner beliefs and supporting evidence
- Candidate diagnosis
- Verified belief transition

The two models may be implemented by one reasoning process. Separate agents are
not required.

## Boundaries

- Do not infer learner position from demographics, confidence, or topic labels.
- Do not treat either graph as a fixed perfect DAG.
- A novel learner response may reveal a misconception absent from the domain
  model.
- Current evidence overrides stored placement.

## Sources

[S02](../sources/S02-elite-hacker-roadmap.md),
[S07](../sources/S07-learning-with-ai.md),
[S09](../sources/S09-socrates-product-exploration.md),
[S11](../sources/S11-learning-system-for-trpc.md),
[S13](../sources/S13-threshold-unlocks.md).

## Related

[Evidence-Based Diagnosis](03-evidence-based-model-diagnosis.md),
[Curriculum as Leverage Architecture](07-curriculum-as-leverage-architecture.md),
[Multi-Scope State](14-multi-scope-durable-state.md),
[Prerequisite graph tension](../TENSIONS.md#12-prerequisite-graph-vs-mutable-belief-graph).

Runtime:
[learn-deeply](../../../skills/productivity/learn-deeply/SKILL.md),
[design-learning-path](../../../skills/productivity/design-learning-path/SKILL.md).
