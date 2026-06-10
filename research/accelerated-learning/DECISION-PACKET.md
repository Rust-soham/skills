# Approved Skill Design Decisions

Approved by the user. These decisions govern the first skill implementation.

## 1. Relationship to `teach`

**Decision:** Create the new system adjacent to `teach`. Preserve `teach` as a
comparison target.

Why it matters: replacing `teach` immediately would mix validation of the new
model-transition engine with migration of its HTML lesson workspace.

## 2. Initial Skill Boundary

**Decision:** Start with two skills:

1. A universal model-transition orchestrator
2. A threshold-curriculum designer

Keep development and research as modes of the orchestrator for now, with a
programming reference loaded only when code or a software artifact is involved.
A later programming-specific skill will derive from the universal thesis and
add specialized implementation behavior.

The orchestrator now distinguishes:

- Development mode for minimum bottleneck removal and artifact return
- Research mode for recursive why chains and broader FAFO

Delegation and production rescue are execution overrides rather than peer
learning modes.

Why it matters: a third programming skill would overlap with the universal
skill on the system's primary use case.

## 3. Name and Activation

**Decision:** Use `learn-deeply` as the initial skill name. Retain **Socrates**
as the product or future harness name.

Activate only when:

- The user explicitly asks to learn, understand, practice, or be taught
- The user invokes the skill
- A previously established learning mission is active

Do not silently convert ordinary execution requests into lessons.

## 4. Global and Local Context

**Decision:**

- Store portable learner evidence under `~/.learning/`, shared across
  workspaces.
- Store mission, project, version, artifact, and session evidence under
  `<workspace>/.learning/`.
- Use verified global anchors for cross-domain analogy, such as Go goroutines
  when learning adjacent concurrency models.
- Keep project-specific facts local unless they are compressed into a
  transferable pattern and verified beyond the original context.
- Persist motivational or psychological observations only by explicit opt-in.

This is a logical and physical distinction: global context follows the learner;
local context follows the workspace.
