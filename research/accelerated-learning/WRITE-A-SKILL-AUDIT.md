# Write-a-Skill Audit

Validated against
[`skills/other/productivity/write-a-skill/SKILL.md`](../../skills/other/productivity/write-a-skill/SKILL.md).

## Process

### Requirements

- Domain: accelerated learning through model repair and compounding paths
- Use cases: development, research, roadmaps, and multi-step deep learning
- Resources: instructions and formats; no runtime scripts required
- References: transcript research, state format, programming adapter, path
  format, and concrete examples

### Draft and Review

The first drafts were reviewed against user feedback. Revisions added:

- Development and research modes
- Mandatory composition between path design and model repair
- Per-step compounding and pit-of-success tests
- Protected first-move diagnosis
- Grounded threshold mining and representation rotation
- Concrete examples
- Narrower research triggering
- Consistent `path step` terminology

## Checklist

| Requirement | `learn-deeply` | `design-learning-path` |
| --- | --- | --- |
| Description includes `Use when` triggers | Pass | Pass |
| Description is third person and under 1024 characters | 463 characters | 320 characters |
| `SKILL.md` is under 100 lines | 99 lines | 99 lines |
| No time-sensitive information | Pass | Pass |
| Consistent terminology | `path`, `path step`, `model transition` | `path`, `path step`, `model transition` |
| Concrete examples included | `EXAMPLES.md`: development and research | `EXAMPLES.md`: research path and development micro-path |
| References are one level deep | Pass | Pass |

## Progressive Disclosure

`learn-deeply/SKILL.md` contains the universal orchestration contract and links
directly to:

- `WORKSPACE-FORMAT.md` for state
- `PROGRAMMING.md` for software-specific behavior
- `EXAMPLES.md` for concrete runs
- `design-learning-path/SKILL.md` for path selection

`design-learning-path/SKILL.md` contains the path-design contract and links
directly to:

- `PATH-FORMAT.md` for output schemas
- `EXAMPLES.md` for concrete paths

No reference requires traversing another reference to discover required
behavior.

## Scripts

No scripts were added. The skills perform judgment-heavy orchestration rather
than a repeated deterministic transformation. Repository validation uses the
existing `skill-creator` validator.

## Result

Both skills satisfy Matt's local `write-a-skill` checklist and the repository's
stronger reference-shape constraints: concrete triggers, one governing unit,
observable gates, negative rules, and progressive disclosure.
