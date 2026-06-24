# Examples

## Development: Unfamiliar Retry Library

Request:

> Help me add retries with this job library while learning what I need.

Run:

1. Set the return gate: a failed job retries without duplicating its side
   effect.
2. Ask how the learner currently thinks delivery and retry interact.
3. Use a micro-path: delivery semantics -> idempotency boundary.
4. Create one duplicate-delivery case that breaks "the job runs once."
5. Verify that the learner can predict the duplicate, place the idempotency
   guard, and inspect the result.
6. Return immediately to the feature.

Park scheduler internals and distributed deduplication for research mode.

## Research: Runtime Scheduler

Request:

> Help me understand this runtime scheduler deeply. Keep asking why and let me
> experiment.

Run:

1. Diagnose the learner's model of task state and wakeups.
2. Build a path through task state -> wakeup contract -> polling -> fairness ->
   cancellation.
3. For each step, require a prediction and inspect source or runtime evidence.
4. FAFO with delayed wakeups, duplicate wakeups, starvation, cancellation, and
   an alternative scheduling policy.
5. After each verified repair, recontextualize earlier steps and revise the
   remaining path.
