# S15: Post by @mattpocockuk

Source: `transcripts/Post by @mattpocockuk on X.md`

Status: cross-checked

## Evidence Notes

### Prefactoring

The post proposes inspecting the code before implementation for a preparatory
refactor that makes the requested change easier:

> Make the change easy, then make the easy change.

([12-26](../../../transcripts/Post%20by%20%40mattpocockuk%20on%20X.md#L12))

### Learning Implication

`SYNTHESIS`: The same operation applies to learning tasks. Before increasing
learner effort, modify the environment so the target concept is isolated:

- Reduce unrelated setup
- Expose the relevant primitive
- Add observability
- Construct a minimal sandbox
- Separate coupled variables

The learner then performs the meaningful cognitive change under clearer
conditions.

### Boundary

Prefactoring should simplify the target operation, not move complexity into a
larger abstraction that is harder to inspect. A comment in the source raises
this exact concern
([56-62](../../../transcripts/Post%20by%20%40mattpocockuk%20on%20X.md#L56)).

### Signals

- Preparatory work removes non-target friction
- The target decision remains learner-owned
- The resulting experiment has fewer changing variables
- Total system complexity does not increase without justification

### Failure Modes

- Refactoring as procrastination
- Hiding the concept behind new machinery
- Making implementation easier by delegating the target reasoning
- Changing unrelated code

### Refinement

`REFINEMENT`: S06's isolated sandbox and S11's cognitive ergonomics are forms of
learning prefactoring. The environment is changed first so the meaningful model
update becomes easier to perform and observe.
