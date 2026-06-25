# Leverage Selection

Use recursive Pareto as the path-selection heuristic: after each verified
model update, choose the reachable next transition with the largest expected
capability gain, friction reduction, or future reuse for the mission.

This is a planning heuristic, not a literal 80/20 growth claim.

## Loop

1. Classify the mission and target capability.
2. Pick the highest-leverage reachable threshold.
3. Add only prerequisites needed to cross and verify it.
4. Let `learn-deeply` produce learner-owned evidence.
5. Recompute leverage over the remaining gap.
6. Repeat until the mission success gate is met.

## Prefer Steps That

- Unlock several later steps or make them cheaper.
- Replace many local rules with one generative invariant.
- Expose hidden control flow, boundaries, or failure modes.
- Improve the learner's questions or judgment of agent output.
- Return to the mission artifact faster without hiding the model transition.
- Convert a recurring blocker into a reusable chunk.

## Guardrails

- Optimize for verified capability per effort, not speed alone.
- Preserve productive struggle needed for the learner to own the transition.
- Do not choose a threshold that needs so much scaffold it becomes agent-owned.
- Replan after meaningful model evidence; do not freeze the first Pareto pass.
