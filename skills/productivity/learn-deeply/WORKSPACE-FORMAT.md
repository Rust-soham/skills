# Learning State

Create state lazily. Do not change version-control treatment without the
user's direction.

## Storage

```text
~/.learning/
├── LEARNER.md
├── PATTERNS.md
└── records/

<workspace>/.learning/
├── MISSION.md
├── PROJECT.md
├── STATE.md
├── CURRICULUM.md
├── records/
└── sandboxes/
```

`CURRICULUM.md`, `records/`, and `sandboxes/` are optional until needed.

## Scope

Global state contains portable, verified learner evidence:

- Demonstrated anchors and their depth
- Transferable model transitions
- Structural analogies and failure boundaries
- Recurring reasoning patterns
- Assistance and self-probing calibration

Local state contains mission and workspace evidence:

- Capability target and independent success
- Artifact, versions, constraints, and architecture
- Current blocker, target friction, and next action
- Curriculum node, unresolved model, and sandbox return condition

Promote a project finding globally only after compression and transfer or
reconstruction evidence. Never copy raw chat or project context globally.

## Required Files

### `MISSION.md`

```md
# Mission
- Desired capability:
- Why it matters:
- Independent success:
- Constraints:
- Target friction:
- Mode: development | research
- Current priority: artifact return | model depth
```

Change the mission only with learner confirmation.

### `PROJECT.md`

```md
# Project
- Artifact:
- Next shippable change:
- Versions and constraints:
- Current blocker and evidence:
- Target friction:
- Active sandbox question:
- Return condition:
- Next project action:
```

### `STATE.md`

```md
# State
- Mode: development | research
- Current model:
- First move:
- Current path step:
- Pending verification:
- Assistance level:
- Artifact return gate:
- Parked research questions:
- Next action:
```

## Evidence Records

Create a record only after verification:

```md
# <Model Transition>
- Scope:
- Old model:
- First move:
- Prediction or attempt:
- Probe or event:
- Observation:
- Failed assumption:
- Repaired model or invariant:
- Boundary:
- Compressed rule:
- Verification and result:
- Transfer evidence:
- Assistance used:
- Provenance:
- Status: verified
- Last verified:
```

Portable global entries also record the originating workspace. Use
`candidate -> verified -> challenged -> superseded`; do not silently overwrite
contradictions.

Revalidate when context changes, evidence conflicts, or a claim will justify a
skipped prerequisite, major analogy, or delegation decision. Age alone does not
invalidate evidence.
