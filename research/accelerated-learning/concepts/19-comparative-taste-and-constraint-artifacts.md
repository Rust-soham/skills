# Comparative Taste and Constraint Artifacts

**Status:** Core for build missions

## Core Claim

Taste develops by comparing plausible alternatives against explicit
constraints, not by accepting one polished generated result.

## Constraint Artifact

Capture before design-sensitive delegation:

- Requirements and non-goals
- Invariants
- Valid and illegal states
- Failure behavior
- Observability
- Performance and operational constraints
- Maintenance costs
- Conditions the implementation must preserve

## Comparative Practice

1. Produce or inspect multiple viable alternatives.
2. Evaluate each under the same constraint artifact.
3. State what each optimizes and sacrifices.
4. Identify which failure modes are acceptable here.
5. Defend the selected design in the current context.
6. Revisit the decision when constraints change.

High-quality reference work provides calibration, but the learner must still
explain why a pattern fits this situation.

## Boundaries

- One implementation cannot establish taste.
- Familiar style is not evidence of fitness.
- Aesthetics, correctness, operability, and maintenance should not be collapsed
  into one vague quality score.

## Sources

[S02](../sources/S02-elite-hacker-roadmap.md),
[S06](../sources/S06-ai-in-dev-workflows.md),
[S09](../sources/S09-socrates-product-exploration.md).

## Related

[Unknown-Unknown Discovery](11-unknown-unknown-discovery.md),
[Dynamic AI Modes](13-dynamic-ai-mode-and-delegation-boundary.md),
[Compression](09-compression-and-pattern-extraction.md).

Runtime:
[programming adapter](../../../skills/mine/exponential/learn-deeply/PROGRAMMING.md).
