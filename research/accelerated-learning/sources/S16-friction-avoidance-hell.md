# S16: Friction Avoidance Hell

Source: `transcripts/Friction Avoidance Hell.md`

Status: cross-checked

## Evidence Notes

### Source Authority Within the Transcript

The user's opening is a direct account of a long-running avoidance pattern and
their desired AI contract. The assistant's prescriptions are often absolute and
tailored to that moment. Preserve the behavioral problem and useful constraints;
do not universalize punitive cadence, code limits, or anti-theory rules.

### Avoidance as a Feedback Loop

The user describes repeatedly leaving when work becomes difficult, substituting
courses, planning, lurking, and screens for end-to-end project work. External
structure previously supplied deadlines, reinforcement, and reduced ambiguity
([11-13](../../../transcripts/Friction%20Avoidance%20Hell.md#L11)).

The transcript names the pattern "friction avoidance": discomfort plus an easy
escape route repeatedly terminates the learning loop
([23-56](../../../transcripts/Friction%20Avoidance%20Hell.md#L23)).

`SOURCE`: The system must distinguish a genuine conceptual blocker from an
avoidance transition. Both can look like "I need to learn more," but require
opposite responses.

### Just-in-Time Learning Attached to an Artifact

The source recommends consuming information only when it is immediately used to
advance a concrete project
([62-76](../../../transcripts/Friction%20Avoidance%20Hell.md#L62)).

The project should initially be small enough to finish end to end, with scope
restrictions that prevent ambition from becoming another escape
([149-184](../../../transcripts/Friction%20Avoidance%20Hell.md#L149)).

Progress is defined by a concrete artifact change rather than hours, motivation,
or content consumed
([188-205](../../../transcripts/Friction%20Avoidance%20Hell.md#L188)).

`REFINEMENT`: For this learner, the local project is not merely context for
better exercises. It is the behavioral rail that prevents learning from
becoming avoidance.

### Attempt-Failure-Repair Rhythm

The source proposes:

`concrete problem -> provisional model -> imperfect attempt -> specific
confusion -> targeted question -> model repair -> ship -> repeat`

([243-262](../../../transcripts/Friction%20Avoidance%20Hell.md#L243)).

It later separates:

- **Shipping mode**: act, test, and tolerate imperfection.
- **Learning mode**: resolve one blocker through targeted retrieval and model
  work.

The proposed switch is blockage rather than boredom
([418-439](../../../transcripts/Friction%20Avoidance%20Hell.md#L418)).

`QUESTION`: Waiting until blocked may be appropriate for avoidance-prone
project work, but insufficient for proactive unknown-unknown discovery and
curriculum sequencing. The mode rule should depend on mission.

### Library Orientation

For unfamiliar technology, the transcript recommends:

1. Identify the problem the tool exists to solve.
2. Reduce it to a few core primitives.
3. Build the smallest incomplete or wrong version.
4. Ask about intent and system behavior when evidence becomes confusing.

([348-415](../../../transcripts/Friction%20Avoidance%20Hell.md#L348))

`REFINEMENT`: The smallest wrong version is both progress and a diagnostic
instrument. It creates concrete evidence without requiring broad preparation.

### Agent Contract for Product-Driven Learning

Across the proposed prompts, durable behaviors are:

- Preserve learner ownership of design and reasoning.
- Remove documentation hunting, API trivia, boilerplate, and setup noise when
  those are not the target.
- Explain responsibilities, data flow, control flow, lifecycle, invariants, and
  tradeoffs.
- Use small hints or scaffolds when needed.
- Trace failures through hypotheses rather than jumping to patches.
- Anchor learning to the feature being built.
- Call out over-planning, endless refactoring, premature abstraction, and
  learning detours.
- Prefer a small shippable step that builds reusable judgment.

([99-143](../../../transcripts/Friction%20Avoidance%20Hell.md#L99),
[489-579](../../../transcripts/Friction%20Avoidance%20Hell.md#L489),
[640-758](../../../transcripts/Friction%20Avoidance%20Hell.md#L640))

Success evidence includes explaining the system in one's own words, rebuilding
the feature, shipping an imperfect artifact, and making the next project easier
([566-579](../../../transcripts/Friction%20Avoidance%20Hell.md#L566),
[749-753](../../../transcripts/Friction%20Avoidance%20Hell.md#L749)).

### Growth-Compounding Step Selection

The user explicitly asks the agent to choose steps whose order compounds
competency while building products
([623-625](../../../transcripts/Friction%20Avoidance%20Hell.md#L623)).

The response prioritizes steps that expose reusable abstractions, system
boundaries, state, data flow, and lifecycle over low-signal mechanical work
([671-678](../../../transcripts/Friction%20Avoidance%20Hell.md#L671)).

`SYNTHESIS`: In a build mission, next-step selection has at least two objectives:

- Advance the artifact enough to preserve momentum and reality contact.
- Maximize reusable model growth per unit of project risk.

Neither objective should erase the other.

### Durable State Suggested by the Source

- Current artifact and next shippable change
- Declared target friction
- Current blocker and evidence
- Provisional model and attempted implementation
- Avoidance indicators: scope expansion, content detour, repeated restart,
  premature refactor, or passive consumption
- Finished end-to-end milestones
- Concepts learned through immediate application
- Whether the learner can rebuild the feature

### Signals

- Information consumed is immediately applied
- Project scope reaches an end-to-end completion
- Learner attempts before requesting a solution
- Confusion becomes a specific question tied to evidence
- Learning mode returns to shipping mode after the blocker clears
- The next step improves both artifact and reusable judgment
- Learner can recreate the feature without the agent

### Failure Modes

- Escaping into courses, roadmaps, or planning
- Starting projects too large to close a feedback loop
- Treating every discomfort as a missing-concept problem
- Letting AI complete the project while preserving the appearance of progress
- Remaining in learning mode after the artifact is unblocked
- Shipping repeatedly without crystallizing the model
- Over-planning, endless refactoring, or premature abstraction
- Measuring progress through time or content volume

### Rejected or Context-Dependent Mechanisms

- "No zero days" as a punitive universal rule
- Fixed snippet-length limits
- Never allowing full implementations
- Never learning before implementation
- Switching to learning only when blocked in every mission
- Ignoring all edge cases until a core model is declared solid
- Treating documentation as untrusted by default
- Assuming confusion is always desirable
- Claiming that one prompt or daily cadence will resolve an entrenched avoidance
  pattern

These can be temporary constraints selected for a learner and mission, not the
universal core.

### Refinements and Tensions

`REFINEMENT`: Chosen friction includes a behavioral choice to remain in contact
with the artifact when discomfort appears, not only a cognitive choice about
which concept to learn.

`REFINEMENT`: S09's local project context needs an artifact-progress model in
addition to a concept model.

`QUESTION`: How should an agent infer avoidance without pathologizing legitimate
research, rest, scope correction, or a truly blocked task?

`QUESTION`: The universal curriculum may deliberately pause shipping for a
threshold exercise. The build-mode skill needs an explicit return condition so
the exercise does not become another detour.
