# Programming Adapter

Use only for software artifacts. `learn-deeply` owns model repair;
`design-learning-path` owns the sequence between repairs.

## Ground Reality

Prefer:

1. Current code, tests, types, diagnostics, runtime behavior, and versions
2. Installed source and API surfaces
3. Version-matched official documentation
4. Other high-trust external sources

Retrieve only context relevant to the disputed behavior. Keep version and
provenance visible. Answer incidental lookup directly.

## Development Mode

Goal: remove the unfamiliar concept, library, framework, or domain bottleneck
and get back to building.

1. Name the next shippable artifact action.
2. Ask for the learner's current model only where it affects the blocker.
3. Classify friction as target or incidental.
4. Ground the disputed behavior in code or runtime evidence.
5. Use `design-learning-path` to form the shortest micro-path from blocker to
   artifact return.
6. Execute the current step with the smallest diagnostic example or sandbox.
7. Verify enough understanding to predict, implement, and inspect the relevant
   behavior.
8. Reapply immediately and continue building.
9. Crystallize the verified pattern; park deeper questions for research mode.

Do not expand adjacent why branches once the return gate is satisfied.
Development mode optimizes time-to-unblocked action, not domain mastery.

## Research Mode

Goal: explore the abstraction deeply enough to generate better questions,
experiments, designs, and future learning.

1. Define the generative capability or research question.
2. Use `design-learning-path` to build a compounding threshold path.
3. Follow recursive why chains through implementation, primitives, invariants,
   constraints, and failure semantics.
4. For each why, require evidence or an experiment; stop at ground truth,
   irrelevance to the mission, or unavailable evidence.
5. Run broader FAFO across baseline, boundary, pathological, inversion, and
   alternative-implementation cases.
6. Compare real code, source, runtime behavior, and multiple designs.
7. Recontextualize prior steps after each threshold and update the path.

Research mode may branch. Record and rank branches by expected leverage while
allowing bounded curiosity probes.

## Shape the Environment

- **Isolate:** one primitive or variable.
- **Split:** coupled responsibilities.
- **Elevate:** the broader problem generating several symptoms.
- **Enable:** a preparatory change that permits the target experiment.
- **Ground:** claims in source, types, tests, or runtime evidence.
- **Rotate:** represent the same behavior through another abstraction, diagram,
  trace, type shape, or executable form to expose an invariant.

## Project or Sandbox

Stay in the artifact while it produces clear, safe evidence. Move to a sandbox
when variables are entangled, feedback is noisy, failure is costly, or a
missing primitive blocks a useful prediction.

Before leaving, record the exact question, isolated variable, real constraints,
ending evidence, and project return action. A passing toy is insufficient;
reapply the repaired model to the artifact.

## Controlled FAFO

1. State a hypothesis about the primitive.
2. Build the smallest falsifying case.
3. Change one variable.
4. Probe a boundary or pathological case.
5. Remove or reverse a step and find the first broken invariant.
6. Update the model and the learning path.

## Design and Taste

Before design-sensitive delegation, capture requirements, non-goals,
invariants, illegal states, failure behavior, observability, and maintenance
constraints. Compare viable alternatives under the same constraints.
