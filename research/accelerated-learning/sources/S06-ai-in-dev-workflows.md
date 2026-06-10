# S06: AI in Dev Workflows

Source: `transcripts/AI in Dev Workflows.md`

Status: cross-checked

## Evidence Notes

### Senior Leverage

`SOURCE`: AI compresses idea-to-code feedback, but experienced developers gain
more because they can simulate systems, predict failures, constrain solution
space, and judge output before or shortly after implementation
([18-32](../../../transcripts/AI%20in%20Dev%20Workflows.md#L18),
[56-70](../../../transcripts/AI%20in%20Dev%20Workflows.md#L56)).

"Only generate what I already understand" prevents cargo-culting but also
freezes the learner's frontier. The refinement is to explore adjacent unknowns
while validating assumptions
([36-52](../../../transcripts/AI%20in%20Dev%20Workflows.md#L36)).

### Capabilities to Train

- Failure-mode prediction
- Mental simulation
- Constraint and invariant definition
- Taste through comparison
- Judgment of maintainability, concurrency, integrity, and performance
- Ability to explain code independent of its surface form

Evidence:
[80-134](../../../transcripts/AI%20in%20Dev%20Workflows.md#L80),
[166-184](../../../transcripts/AI%20in%20Dev%20Workflows.md#L166).

Taste develops through comparison: implement or inspect alternatives, compare
their state handling, failure paths, extensibility, and maintenance costs, then
explain why one design fits the constraints better
([115-134](../../../transcripts/AI%20in%20Dev%20Workflows.md#L115)).

Constraint thinking should produce an explicit pre-code artifact containing
requirements, non-goals, invariants, valid transitions, observability needs,
and failure behavior. This gives AI a bounded solution space and gives the
learner something concrete against which to judge its output
([166-184](../../../transcripts/AI%20in%20Dev%20Workflows.md#L166)).

The source highlights concurrency, distributed failure, data integrity,
performance cliffs, and long-term maintenance as high-signal practice areas
because surface correctness is insufficient there
([138-162](../../../transcripts/AI%20in%20Dev%20Workflows.md#L138)).

### Three AI Modes

#### Implementation Delegate

The learner designs, AI implements known patterns, and the learner reviews.
Suitable for syntax, boilerplate, and repetition
([290-309](../../../transcripts/AI%20in%20Dev%20Workflows.md#L290)).

#### Guided Unknown Exploration

For an unfamiliar tool or paradigm:

1. Identify its problem, mental model, primitives, and smallest example.
2. Build an isolated toy.
3. Investigate beginner mistakes, footguns, and production failures.

([313-353](../../../transcripts/AI%20in%20Dev%20Workflows.md#L313))

#### Adversarial Learning

After an unfamiliar attempt, ask for hidden assumptions, ignored edges,
concurrency failures, scaling failures, and senior criticism. Reproduce and
verify rather than merely accepting the list
([357-373](../../../transcripts/AI%20in%20Dev%20Workflows.md#L357)).

### One Axis at a Time

The major blocker is simultaneous cognitive load from learning a paradigm,
architecting a system, implementing details, and debugging ecosystem behavior
([248-269](../../../transcripts/AI%20in%20Dev%20Workflows.md#L248),
[377-393](../../../transcripts/AI%20in%20Dev%20Workflows.md#L377)).

Strict sequence:

1. Reduce the paradigm to a primitive model.
2. Isolate it in a tiny sandbox.
3. Integrate it into the product only after the model is usable.

([397-433](../../../transcripts/AI%20in%20Dev%20Workflows.md#L397))

Compressed rule: struggle on one axis at a time
([515-523](../../../transcripts/AI%20in%20Dev%20Workflows.md#L515)).

### Known vs Unknown Unknowns

- Known unknowns: use conceptual reduction, sandboxes, and edge-case questions.
- Unknown unknowns: use adversarial prompts, postmortems, review, and alternate
  implementations. Repetition gradually exposes them.

([436-467](../../../transcripts/AI%20in%20Dev%20Workflows.md#L436))

### Stable Domain, Changing Paradigm

Instead of repeatedly building unrelated systems, evolve one familiar system
through multiple paradigms and constraints. Keeping the domain stable makes
design differences legible and accelerates pattern matching
([471-500](../../../transcripts/AI%20in%20Dev%20Workflows.md#L471)).

This is a concrete mechanism for analogical comparison and controlled transfer.

### Controlled FAFO

The user defines their natural loop:

`poke -> predict -> observe -> update model -> repeat`

([564-573](../../../transcripts/AI%20in%20Dev%20Workflows.md#L564))

`REFINEMENT`: Random experimentation becomes controlled chaos by isolating
variables and stripping the system to one primitive
([603-646](../../../transcripts/AI%20in%20Dev%20Workflows.md#L603)).

Models form faster when one variable changes, signal exceeds noise, and feedback
is immediate
([684-694](../../../transcripts/AI%20in%20Dev%20Workflows.md#L684)).

Known-unknown FAFO:

1. Write the current model.
2. Predict the outcome.
3. Test the smallest case.
4. Break it intentionally.
5. Write the updated model.

([697-717](../../../transcripts/AI%20in%20Dev%20Workflows.md#L697))

For unknown unknowns, AI suggests omitted edge cases and failures; the learner
recreates them locally
([721-740](../../../transcripts/AI%20in%20Dev%20Workflows.md#L721)).

Senior FAFO begins by defining boundaries, invariants, valid transitions, and
illegal states, then probing those edges
([744-766](../../../transcripts/AI%20in%20Dev%20Workflows.md#L744)).

Final protocol:

1. Reduce to a primitive
2. State a hypothesis
3. Test the smallest case
4. Test a boundary case
5. Test a pathological case
6. Document the model update

([770-796](../../../transcripts/AI%20in%20Dev%20Workflows.md#L770))

### Model Quality Signal

Growth is described as shrinking the mismatch between prediction and
observation
([770-781](../../../transcripts/AI%20in%20Dev%20Workflows.md#L770)).

This is stronger than testing only whether the final output works: predictions
make the learner's hidden model inspectable.

### Failure Modes

- Treating AI as code generation rather than an epistemic environment
- Remaining inside only fully known work
- Learning a new paradigm inside a production feature
- Random FAFO with many changing variables
- Asking for unknown unknowns but not recreating them
- Copying abstractions without identifying their constraints and tradeoffs
- Letting AI make architecture decisions implicitly
- Evaluating syntax instead of design decisions
- Accepting a design without comparing it against explicit constraints or a
  plausible alternative

### Refinements and Tensions

`REFINEMENT`: S03's "AI after thinking, never before" becomes three modes. AI
may help map an adjacent unknown before implementation, while still requiring
the learner to predict and verify.

`REFINEMENT`: Sandboxes are not merely simplified examples. They are controlled
experiments designed to isolate causal primitives.

`QUESTION`: "Never accept code you could not rewrite from scratch" is stricter
than the later ownership criterion of simulation and validation. Exact
reproduction may be unnecessary once delegation becomes legitimate.

`QUESTION`: A fixed weekly percentage split is offered
([527-537](../../../transcripts/AI%20in%20Dev%20Workflows.md#L527))
but appears illustrative, not a universal rule.

`SYNTHESIS`: Local project learning needs access to real code and task context,
but the experiment may need to move temporarily into a minimal isolated world.
