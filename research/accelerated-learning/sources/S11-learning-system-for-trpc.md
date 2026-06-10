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
([21-43](../../../transcripts/Learning%20System%20for%20tRPC.md#L21)).

The goal is to move:

`unknown unknowns -> known unknowns -> known knowns`

while continuing the real project
([38-68](../../../transcripts/Learning%20System%20for%20tRPC.md#L38)).

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

([72-128](../../../transcripts/Learning%20System%20for%20tRPC.md#L72),
[132-210](../../../transcripts/Learning%20System%20for%20tRPC.md#L132))

The full loop is orientation, feature work, just-in-time API grounding, then
crystallization
([203-213](../../../transcripts/Learning%20System%20for%20tRPC.md#L203)).

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

([132-148](../../../transcripts/Learning%20System%20for%20tRPC.md#L132))

For overloaded APIs, look for the most general form and the semantic channel or
operation shared by ergonomic variants rather than memorizing each signature
([152-179](../../../transcripts/Learning%20System%20for%20tRPC.md#L152)).

Constraint-first questions include what the abstraction cannot do, where it
breaks, and which assumptions it makes
([217-232](../../../transcripts/Learning%20System%20for%20tRPC.md#L217)).

### Explicit Model Checkpoints

The source names a recurring failure: the learner keeps an implicit fuzzy model,
patches behavior when it breaks, and never intentionally stress-tests or
stabilizes the understanding
([296-326](../../../transcripts/Learning%20System%20for%20tRPC.md#L296)).

`SOURCE`: A model checkpoint externalizes the current model so a later
prediction failure can update understanding rather than merely patch code.

### Mental Model Debugger

The tool is reframed from teacher to "mental model debugger." It asks:

- What part of the model is missing?
- Which assumption is false?
- Which invariant does the abstraction rely on?

([369-384](../../../transcripts/Learning%20System%20for%20tRPC.md#L369))

The desired output is the delta between the learner's model and observed
reality, not a complete explanation
([404-430](../../../transcripts/Learning%20System%20for%20tRPC.md#L404)).

A proposed delta card contains:

1. What the learner currently appears to believe
2. What the evidence shows
3. Why the difference matters
4. Where the difference causes later failures
5. A case that breaks the old model

([434-450](../../../transcripts/Learning%20System%20for%20tRPC.md#L434))

`REFINEMENT`: The instructional unit should be the smallest model change that
restores prediction, not the smallest amount of prose.

### Worked Model-Repair Example: `Effect.gen`

The user supplies a compact provisional model: `Effect.gen` provides
imperative-looking syntax, infers three type channels, uses generator machinery,
and has confusing `yield*` and `return yield*` behavior
([538-542](../../../transcripts/Learning%20System%20for%20tRPC.md#L538)).

The response does not begin from zero. It preserves that model, makes several
implicit claims explicit, and organizes the explanation around:

- The problem the construct is intended to solve
- A one-sentence generative model
- The success, error, and environment channels
- Why generator syntax is used
- The semantic distinction between yielding and returning
- Where an `async`/`await` analogy helps and fails
- Common misuse boundaries and non-use cases

([546-825](../../../transcripts/Learning%20System%20for%20tRPC.md#L546))

The branch then reflects on its own instructional method: it corrected one
limiting assumption, replaced it with an invariant, and stopped instead of
dumping all available documentation
([829-850](../../../transcripts/Learning%20System%20for%20tRPC.md#L829)).

`SOURCE`: This is a concrete demonstration of model-delta teaching. The
learner's own compressed account determines what the explanation preserves,
what it challenges, and how much it needs to say.

### Analogy With Explicit Semantic Differences

The `Effect.gen` example compares the new construct to imperative sequencing
and `async`/`await`, then emphasizes where the apparent analogy fails
([554-593](../../../transcripts/Learning%20System%20for%20tRPC.md#L554),
[720-768](../../../transcripts/Learning%20System%20for%20tRPC.md#L720)).

The transcript later describes the successful pattern as correcting one wrong
assumption and replacing it with an invariant
([821-845](../../../transcripts/Learning%20System%20for%20tRPC.md#L821)).

`QUESTION`: Because the technical explanation itself may contain errors, a
model-delta system must ground the "reality" side in source, types, tests, or
runtime evidence. Confident prose is not sufficient.

### Cognitive Ergonomics

The user's clearest formulation is that AI should not replace cognitive work.
It should remove retrieval friction so the learner can alternate building and
repairing models until they survive
([866-894](../../../transcripts/Learning%20System%20for%20tRPC.md#L866)).

`SOURCE`: This is a restored direct user requirement, not merely an assistant
interpretation: AI supplies environmental tools around retrieval while the
learner repeatedly builds, breaks, and repairs the model
([866-868](../../../transcripts/Learning%20System%20for%20tRPC.md#L866)).

The source distinguishes:

- Target work: thinking, debugging, reasoning, designing
- Overhead: finding definitions, reconstructing signatures, reconciling
  overloads or versions, and locating the violated invariant

([898-926](../../../transcripts/Learning%20System%20for%20tRPC.md#L898))

AI's role is to arrange information, stabilize context, surface invariants, and
compress reference material
([930-967](../../../transcripts/Learning%20System%20for%20tRPC.md#L930)).

The governing rule is:

- Removing friction around a learner-owned decision is useful.
- Making the decision for the learner defeats the goal.

([990-995](../../../transcripts/Learning%20System%20for%20tRPC.md#L990))

The desired load allocation is low retrieval cost, low structure-reconstruction
cost, and high useful thinking cost
([1029-1050](../../../transcripts/Learning%20System%20for%20tRPC.md#L1029)).

The closing product principle is to shorten the distance from code to its
assumption and invariant, not from code to an answer or fix. The intended
experience is calm continuity of thought, with meaningful model-repair work
preserved and wasted effort removed
([1054-1135](../../../transcripts/Learning%20System%20for%20tRPC.md#L1054)).

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
([917-924](../../../transcripts/Learning%20System%20for%20tRPC.md#L917)), but
other sources treat discovering the failed assumption as central learner work.
The likely boundary is that AI may retrieve candidate invariants and evidence,
while the learner must predict, diagnose, and accept the repair.

`QUESTION`: Orientation before code and "zero theory first" conflict if treated
as absolutes. Both can be reconciled as minimum sufficient orientation followed
immediately by an executable encounter.
