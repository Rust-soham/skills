# Exponential Learning

Use these skills together to turn a learning goal into a compounding path and
then cross its next model transition through learner-owned evidence.

## Skill Roles

- [design-learning-path](./design-learning-path/SKILL.md) works at the
  curriculum scale. It maps the target capability, selects and sequences
  leverage-ordered model transitions, and designs a pit of success.
- [learn-deeply](./learn-deeply/SKILL.md) works at the path-step scale. It
  diagnoses the learner's current model, runs one selected transition through a
  targeted encounter, verifies the repair, and updates the path.

## Default Choreography

```text
mission and local evidence
-> design-learning-path: create or revise the leverage-ordered path
-> learn-deeply: execute one active path step
-> verified model delta and artifact evidence
-> update learner position, then replan the remaining path
```

`learn-deeply` invokes `design-learning-path` after diagnosis when no active
path exists or when new evidence changes prerequisites, leverage, or the
mission. Do not create disconnected exercises: every exercise implements the
active path step.

## Entry Points

- Use **design-learning-path** alone for a roadmap, curriculum, mastery
  sequence, multi-step research goal, or recursive child path.
- Use **learn-deeply** alone for one current concept, blocker, or mental-model
  repair. It creates the shortest path needed and returns to the artifact.
- Use both for an active mission that requires more than one transition. Begin
  with path design, execute one step, and revise from evidence rather than
  treating the curriculum as fixed.

## Modes and Recursion

- In **development** mode, design the shortest dependency path from an
  unfamiliar blocker to a concrete artifact return.
- In **research** mode, design a wider compounding threshold path toward a
  generative capability.
- When a long-path transition has its own target, prerequisites, and multiple
  stages, make it a child curriculum. Its verified completion unlocks the
  parent path.

## State and Evidence

Read portable learner anchors from `~/.learning/` and mission/project state
from `<workspace>/.learning/`. Store only verified model transitions and
evidence-backed path updates. Global context supplies reusable anchors; local
context supplies truth for the active mission.

## Do Not

- Treat path design as a topic inventory.
- Treat one exercise as the whole curriculum.
- Advance on exposure, agreement, confidence, or a passing toy alone.
- Keep learning detached from the mission's artifact or independent success
  condition.
