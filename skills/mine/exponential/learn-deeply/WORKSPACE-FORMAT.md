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
├── GLOSSARY.md
├── RESOURCES.md
├── records/
└── sandboxes/
```

`CURRICULUM.md`, `GLOSSARY.md`, `RESOURCES.md`, `records/`, and `sandboxes/`
are optional until needed.

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
- Mission type: unblock-build | abstraction-untangle | research-map | layered-capability | transfer-synthesis
- Out of scope:
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

### `GLOSSARY.md`

Create this only when repeated or ambiguous terminology would distort later
reasoning. Add a term only after the learner uses it correctly; define it in
one or two sentences and record any rejected aliases or local resolution.
This is a shared compression layer, not a dictionary to preload.

### `RESOURCES.md`

Create this for research-mode work or externally grounded, version-sensitive
claims. Keep a short annotated source map:

```md
# Resources
## Ground truth
- Source, version or date, and claims it supports

## Practice context
- Practitioner or community source, the judgment it informs, and its limits

## Gaps
- Important claims or conditions not yet grounded
```

Treat primary sources, executable evidence, and official documentation as
ground truth when appropriate. Practice context can sharpen judgment but does
not replace technical verification.

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

A record is decision-grade learning state, not a session log. Do not write one
for material merely covered, an answer supplied by the agent, or a passing toy
without independent evidence. When a later repair replaces an earlier model,
mark the old record as superseded and retain the learning history.

Revalidate when context changes, evidence conflicts, or a claim will justify a
skipped prerequisite, major analogy, or delegation decision. Age alone does not
invalidate evidence.
