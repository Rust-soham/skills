# Skill Implementation Readiness

The four decisions in [DECISION-PACKET.md](DECISION-PACKET.md) are approved.
This execution plan has been implemented. See [VALIDATION.md](VALIDATION.md).

## Repository Placement

Both proposed skills belong in `skills/productivity/` because their trigger is a
learning workflow, not software implementation:

```text
skills/productivity/
├── learn-deeply/
│   ├── SKILL.md
│   ├── WORKSPACE-FORMAT.md
│   └── PROGRAMMING.md
└── design-learning-path/
    ├── SKILL.md
    └── PATH-FORMAT.md
```

Do not add a skill-local README, changelog, research history, or duplicated
theory.

## `learn-deeply`

Primary unit: one verified model transition.

`SKILL.md` owns:

- Core invariant
- Development and research mode selection
- Diagnostic model-repair loop
- Composition with `design-learning-path`
- Assistance ladder
- Verification and persistence gates
- Trust and engagement boundaries
- Conditional links to workspace and programming references

`WORKSPACE-FORMAT.md` owns:

- Global `~/.learning/` and local `<workspace>/.learning/` layouts
- Mission, learner, project, and session scopes
- Model-transition record
- Evidence lifecycle and context integrity

`PROGRAMMING.md` is loaded only for software artifacts. It owns:

- Code, version, source, type, test, diagnostic, and runtime grounding
- Target-versus-incidental friction
- Project-to-sandbox and return gates
- Controlled FAFO and inversion forms
- Constraint artifacts and comparative taste
- Return to artifact and pattern crystallization
- Development micro-path and research exploration implementations

## `design-learning-path`

Primary unit: one threshold module inside a leverage-ordered path.

`SKILL.md` owns:

- Domain autopsy
- Steepest defensible compounding-curve objective
- Target capability and independent success
- Reachable high-leverage threshold selection
- Module sequence
- Pit-of-success and per-edge acceleration tests
- Generative gates
- Distinction between thresholds and supporting fluency

`PATH-FORMAT.md` owns:

- Domain adapter fields
- Threshold graph
- Limiting-model entries
- Probe specifications
- Artifacts, gates, provenance, and revision rules

## Metadata

Use only portable frontmatter:

```yaml
---
name: skill-name
description: Capability and concrete trigger conditions.
---
```

Do not use Claude-only fields such as `disable-model-invocation` or
`argument-hint`. Encode explicit learning intent in the description. Keep
Socrates as a product name, not a trigger dependency.

Do not create `agents/openai.yaml` in the first repository version. The current
repo has no such metadata, and platform-neutral skill behavior should stabilize
before adding product-specific interfaces.

## Repository Integration

Shipping requires:

- Add both paths to `.claude-plugin/plugin.json`
- Add both skills to `skills/productivity/README.md`
- Replace or extend the top-level `README.md`, currently `WIP.`, with linked
  entries required by `CLAUDE.md`
- Leave `teach` unchanged

## Validation

### Structural

Run for both skills:

```bash
python3 /home/soham/.codex/skills/.system/skill-creator/scripts/quick_validate.py \
  skills/productivity/<skill>
```

Also verify:

- `.claude-plugin/plugin.json` parses as JSON
- Every promoted skill appears in the plugin manifest
- Every promoted skill appears in its bucket README and top-level README
- All local Markdown links resolve
- No duplicated rules across `SKILL.md` and references

### Compression

For every sentence in `SKILL.md`, require that it changes:

- Triggering
- Mode or next action
- State
- Assistance
- Verification
- Safety or trust behavior

Move formats and conditional detail into one-level references.

### Behavioral

Run the scenarios in [EVALUATION-SCENARIOS.md](EVALUATION-SCENARIOS.md).

Required passes:

- Explicit learning requests activate the orchestrator
- Ordinary execution requests do not become lessons
- Programming requests load one adapter rather than a competing skill
- Correct output does not count as understanding without model evidence
- Missing prior context is never fabricated
- Rescue mode does not block urgent execution
- Curriculum output is a transformation graph, not a topic inventory

## Known Integration Constraint

The repository has no native skill linter. `quick_validate.py` checks portable
frontmatter and naming only; behavioral confidence must come from scenario
tests and inspection of emitted artifacts.
