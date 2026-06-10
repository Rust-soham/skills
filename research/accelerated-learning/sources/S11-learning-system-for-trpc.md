# S11: Learning System for tRPC

Source: `transcripts/Learning System for tRPC.md`

Status: cross-checked

## Evidence Notes

### Source Authority Within the Transcript

The transcript contains strong product and learning formulations alongside
assistant-generated technical examples. Some claims about particular Effect
APIs and their runtime or type semantics may be inaccurate. Those examples show
the intended explanatory shape, not authoritative library behavior.

### Unfamiliarity as Concurrent Unknowns

When entering a new library, the learner simultaneously faces API discovery,
types, syntax, purpose, constraints, and failure boundaries
([27-44](../../../transcripts/Learning%20System%20for%20tRPC.md#L27)).

The goal is to move:

`unknown unknowns -> known unknowns -> known knowns`

while continuing the real project
([39-67](../../../transcripts/Learning%20System%20for%20tRPC.md#L39)).

`SYNTHESIS`: The system must lower concurrent load without flattening the
target concept. It should identify which unknown is currently load-bearing and
make the others cheaply retrievable.

### Three Learning Moments

The initial scaffold separates:

1. **Concept orientation before coding**: problem, primitive, execution model,
   type-level inputs and outputs, replacement, and non-goals.
2. **API grounding while coding**: inspect the shape, constraints, effect, and
   misuse boundaries of the exact symbol.
3. **Crystallization after success**: record the compressed model, sharp edges,
   prior confusion, and what became obvious.

([65-113](../../../transcripts/Learning%20System%20for%20tRPC.md#L65),
[115-210](../../../transcripts/Learning%20System%20for%20tRPC.md#L115))

The full loop is orientation, feature work, just-in-time API grounding, then
crystallization
([214-230](../../../transcripts/Learning%20System%20for%20tRPC.md#L214)).

`QUESTION`: Fixed question counts and fixed time boxes are examples, not
invariants. Later transcripts favor diagnostic minimum exposure over mandatory
pre-study.

### Read APIs by Shape and Constraint

For an unfamiliar function, the source proposes extracting:

- Name and role
- Most general input shape
- Output shape
- Required constraint
- Mental translation
- When not to use it

([115-145](../../../transcripts/Learning%20System%20for%20tRPC.md#L115))

For overloaded APIs, look for the most general form and the semantic channel or
operation shared by ergonomic variants rather than memorizing each signature
([149-173](../../../transcripts/Learning%20System%20for%20tRPC.md#L149)).

Constraint-first questions include what the abstraction cannot do, where it
breaks, and which assumptions it makes
([234-246](../../../transcripts/Learning%20System%20for%20tRPC.md#L234)).

### Explicit Model Checkpoints

The source names a recurring failure: the learner keeps an implicit fuzzy model,
patches behavior when it breaks, and never intentionally stress-tests or
stabilizes the understanding
([276-326](../../../transcripts/Learning%20System%20for%20tRPC.md#L276)).

`SOURCE`: A model checkpoint externalizes the current model so a later
prediction failure can update understanding rather than merely patch code.

### Mental Model Debugger

The tool is reframed from teacher to "mental model debugger." It asks:

- What part of the model is missing?
- Which assumption is false?
- Which invariant does the abstraction rely on?

([365-391](../../../transcripts/Learning%20System%20for%20tRPC.md#L365))

The desired output is the delta between the learner's model and observed
reality, not a complete explanation
([405-429](../../../transcripts/Learning%20System%20for%20tRPC.md#L405)).

A proposed delta card contains:

1. What the learner currently appears to believe
2. What the evidence shows
3. Why the difference matters
4. Where the difference causes later failures
5. A case that breaks the old model

([433-445](../../../transcripts/Learning%20System%20for%20tRPC.md#L433))

`REFINEMENT`: The instructional unit should be the smallest model change that
restores prediction, not the smallest amount of prose.

### Analogy With Explicit Semantic Differences

The `Effect.gen` example compares the new construct to imperative sequencing
and `async`/`await`, then emphasizes where the apparent analogy fails
([530-559](../../../transcripts/Learning%20System%20for%20tRPC.md#L530),
[684-715](../../../transcripts/Learning%20System%20for%20tRPC.md#L684)).

The transcript later describes the successful pattern as correcting one wrong
assumption and replacing it with an invariant
([768-783](../../../transcripts/Learning%20System%20for%20tRPC.md#L768)).

`QUESTION`: Because the technical explanation itself may contain errors, a
model-delta system must ground the "reality" side in source, types, tests, or
runtime evidence. Confident prose is not sufficient.

### Cognitive Ergonomics

The user's clearest formulation is that AI should not replace cognitive work.
It should remove retrieval friction so the learner can alternate building and
repairing models until they survive
([795-825](../../../transcripts/Learning%20System%20for%20tRPC.md#L795)).

The source distinguishes:

- Target work: thinking, debugging, reasoning, designing
- Overhead: finding definitions, reconstructing signatures, reconciling
  overloads or versions, and locating the violated invariant

([829-850](../../../transcripts/Learning%20System%20for%20tRPC.md#L829))

AI's role is to arrange information, stabilize context, surface invariants, and
compress reference material
([853-880](../../../transcripts/Learning%20System%20for%20tRPC.md#L853)).

The governing rule is:

- Removing friction around a learner-owned decision is useful.
- Making the decision for the learner defeats the goal.

([899-904](../../../transcripts/Learning%20System%20for%20tRPC.md#L899))

The desired load allocation is low retrieval cost, low structure-reconstruction
cost, and high useful thinking cost
([931-950](../../../transcripts/Learning%20System%20for%20tRPC.md#L931)).

### Durable State Suggested by the Source

- Current externalized model
- Model delta after evidence
- Core primitive and purpose
- Inputs, outputs, constraints, and non-goals
- Most general API shape
- Invariant and violated assumption
- Sharp edges and misuse boundaries
- Evidence source and installed version
- Crystallized one-line model
- Questions that remain unresolved

### Signals

- Learner can state the abstraction's purpose and non-goals
- Learner predicts behavior from the general API shape
- Retrieval support does not choose the design
- Model delta names one changed assumption
- Learner can identify when an analogy fails
- Working code is followed by explicit crystallization
- Later work reuses the compressed invariant without relearning the API

### Failure Modes

- Juggling all unknowns simultaneously
- Reactive lookup followed by copying
- Fixing behavior without updating the model
- Dumping complete documentation
- Memorizing overloads rather than finding the general semantic shape
- Moving on as soon as code works
- Letting AI make design decisions under the label of reducing friction
- Treating unverified AI explanation as reality
- Over-explaining beyond the model delta

### Refinements and Tensions

`REFINEMENT`: S03's productive-versus-wasted-friction distinction becomes a
product contract: minimize code-to-invariant distance while preserving the
learner's decision and model-repair work.

`REFINEMENT`: S09's global analogy bridge requires local, version-grounded
evidence before it can safely define the delta.

`QUESTION`: Locating "what assumption am I violating?" is described as overhead
([840-849](../../../transcripts/Learning%20System%20for%20tRPC.md#L840)), but
other sources treat discovering the failed assumption as central learner work.
The likely boundary is that AI may retrieve candidate invariants and evidence,
while the learner must predict, diagnose, and accept the repair.

`QUESTION`: Orientation before code and "zero theory first" conflict if treated
as absolutes. Both can be reconciled as minimum sufficient orientation followed
immediately by an executable encounter.
