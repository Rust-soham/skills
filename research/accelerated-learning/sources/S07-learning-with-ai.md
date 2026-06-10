# S07: Learning With AI

Source: `transcripts/learning with AI.md`

Status: cross-checked

## Evidence Notes

### Source Authority Within the Transcript

This export mixes the user's ideas, model elaborations, search-result clutter,
unsupported scientific claims, and an invented description of an external
product. Preserve the user's conceptual moves; treat model-proposed mechanisms
as candidates requiring cross-source support.

### Central User Thesis

The user states that the learner must create the mental model. AI should
accelerate that construction by presenting examples designed to expose missing
understanding, then use probing questions instead of supplying the correction
([248-264](../../../transcripts/learning%20with%20AI.md#L248)).

This defines three responsibilities:

- The learner owns model construction.
- The agent selects high-information experiences.
- The interaction reveals a gap without immediately closing it.

### High-Fidelity Failure

The source proposes progressively difficult examples containing subtle flaws,
edge-case scenarios where working code fails, and analogical skeletons whose
implementation violates the stated model
([252-290](../../../transcripts/learning%20with%20AI.md#L252)).

Interaction loop:

1. Learner struggles without retrieval.
2. Learner states a hypothesis.
3. If wrong, the agent gives another example of the same misconception in a
   different context rather than explaining it.
4. Learner compresses the resulting model into one sentence.

([293-300](../../../transcripts/learning%20with%20AI.md#L293))

`REFINEMENT`: The corrective unit is not necessarily verbal feedback. A better
counterexample may produce a stronger model update than an explanation.

The earlier exploration also proposes delayed reconstruction from a blank
surface and manually refining an intentionally rough implementation. These are
useful verification variants when they test retained structure or design taste,
but fixed waiting periods and forced retyping are not universal requirements
([185-223](../../../transcripts/learning%20with%20AI.md#L185)).

### From External Probing to Self-Probing

The user asks whether generating the probing question themselves would produce
a sharper thinker
([325-327](../../../transcripts/learning%20with%20AI.md#L325)).

The resulting progression:

1. Ask for a solution.
2. Ask why an answer is wrong.
3. Ask AI for a trap.
4. Detect one's own trap and question the underlying assumption.

([331-352](../../../transcripts/learning%20with%20AI.md#L331))

`SOURCE`: The desired terminal state is internalized adversarial questioning:
anticipating failure and examining assumptions before implementation. AI becomes
a mirror for the learner's self-critique
([346-382](../../../transcripts/learning%20with%20AI.md#L346)).

### Premature Delegation

The source distinguishes:

- Delegating work already understood: labor optimization
- Delegating work outside the learner's model: borrowed intelligence

([395-429](../../../transcripts/learning%20with%20AI.md#L395))

The known territory expands through manual work until difficult logic becomes
auditable labor. This restates the dynamic delegation boundary from S05.

### Metacognitive Correction

The user wants AI to correct not only cognition about a topic, but the process
that produced that cognition
([451-457](../../../transcripts/learning%20with%20AI.md#L451)).

Three proposed audits:

- **Unknown unknowns**: identify concepts absent from the learner's framing.
- **Known unknowns**: inspect whether the blocker is a missing prerequisite,
  faulty analogy, or another learning-process error.
- **Known knowns**: improve problem framing and efficiency after understanding
  is secure.

([459-482](../../../transcripts/learning%20with%20AI.md#L459))

The "hostile mirror" monitors process and interrupts guesswork, unexamined
assumptions, or low-rigor patterns without taking over syntax
([486-500](../../../transcripts/learning%20with%20AI.md#L486)).

`SYNTHESIS`: The agent needs two diagnostic targets:

- **Object-level gap**: what model of the subject is wrong or missing?
- **Meta-level gap**: what recurring learning behavior produced or concealed
  that model?

### Fluid Cognition and Transfer

The user asks for a learning algorithm transferable across unrelated domains
([523-529](../../../transcripts/learning%20with%20AI.md#L523)).

The source proposes:

- Map structural similarities between the new domain and domains already known.
- Find the domain's invariants and expert taxonomy.
- Compare failures across domains to identify recurring cognitive errors.
- Stress-test the mapped model with a domain-specific trap.

([531-568](../../../transcripts/learning%20with%20AI.md#L531))

`REFINEMENT`: Analogy should be structural rather than cosmetic. The intended
bridge maps roles, constraints, feedback loops, failure patterns, or causal
relations.

`QUESTION`: The claim that a learner need not build a new foundation when a
structural analogy exists is too strong. Analogy accelerates orientation but
must still be tested for domain-specific differences.

### Socratic Roles

The user explicitly reconnects the system to the coding-learning agent named
Socrates
([778-784](../../../transcripts/learning%20with%20AI.md#L778)).

Three roles are described:

- **Elenchus**: ask one targeted question that reveals a contradiction.
- **Aporia**: create a scenario the current model cannot solve, then sustain
  useful puzzlement.
- **Midwife**: monitor reasoning, demand definitions and justifications, and
  help the learner produce the idea.

([786-819](../../../transcripts/learning%20with%20AI.md#L786))

The source's useful product distinction is:

- Outcome feedback supplies the result.
- Process feedback changes how the learner reasons.

([853-885](../../../transcripts/learning%20with%20AI.md#L853))

The claims about a real product, multi-agent implementation, and Bayesian belief
modeling at
[849-871](../../../transcripts/learning%20with%20AI.md#L849)
are not reliable evidence. They remain implementation possibilities only.

### Context Integrity

The assistant later claims to remember a prior conversation, invents details,
and only admits after correction that the recent context was unavailable
([908-990](../../../transcripts/learning%20with%20AI.md#L908)).

`SOURCE`: The learner explicitly detects this context failure
([972-978](../../../transcripts/learning%20with%20AI.md#L972)).

`SYNTHESIS`: A stateful tutor must distinguish retrieved evidence, current
conversation context, and inference. When context is missing, it should say so
and re-elicit or retrieve the relevant model rather than manufacture
continuity. False continuity corrupts both trust and the learner model.

### Engagement Loop

The user wants AI to leverage habit formation and make the chosen learning loop
compelling
([598-604](../../../transcripts/learning%20with%20AI.md#L598)).

Useful mechanisms proposed:

- Attach a brief challenge to an existing work trigger.
- Use progressive hints so discovery remains learner-owned.
- Adapt difficulty between boredom and overload.
- Make progress visible.
- Reward clarity and successful model repair rather than praise or output
  volume.

([610-654](../../../transcripts/learning%20with%20AI.md#L610))

The strongest guardrail is explicit: attachment should be to clarity, not
validation
([645-654](../../../transcripts/learning%20with%20AI.md#L645)).

Later gamification ideas include a challenge trigger, temporary information
withholding, explanation-based completion, and tracking metacognitive
attributes rather than hours
([1060-1080](../../../transcripts/learning%20with%20AI.md#L1060)).

### Durable State Suggested by the Source

- Current explanation or model
- Failed assumptions
- Known unknowns
- Suspected unknown unknowns
- Recurring cognitive failure patterns
- Transfer bridges to known domains
- Challenge history and hint level
- Evidence of self-generated questions
- Evidence of reconstruction and transfer
- Engagement preferences and fatigue signals

### Signals

- Learner states their model before instruction
- Learner predicts before observing
- A targeted question reveals a contradiction
- Learner asks the next useful probe without AI
- Learner defines terms precisely enough to survive counterexamples
- Learner recognizes a recurring cognitive error across domains
- Learner transfers the repaired model to a new context
- Learner can explain why the old model failed

### Failure Modes

- Consuming explanations instead of constructing models
- Correcting output without correcting reasoning process
- Asking AI for every probe indefinitely
- Cosmetic analogies that hide causal differences
- Premature delegation
- Gamification that rewards points, praise, streaks, or identity theater instead
  of learning evidence
- Keeping difficulty high at all times
- Treating confusion itself as progress without model updates

### Rejected or Unproven Mechanisms

These appear in the transcript but should not become system rules:

- Fixed silence periods or arbitrary time requirements
- "Exactly 4%" difficulty increases
- Claims about dopamine, BDNF, or neuroplasticity without reliable evidence
- Punitive streak resets
- Insults, shame, or identity attacks
- Deliberately lying to test vigilance
- Random hidden defects in ordinary work without informed consent
- A permanent zero-solution policy
- Pretending to remember unavailable learner history
- Militaristic, nationalist, or character-purity rhetoric as motivation

Relevant passages:
[610-654](../../../transcripts/learning%20with%20AI.md#L610),
[720-777](../../../transcripts/learning%20with%20AI.md#L720),
[908-990](../../../transcripts/learning%20with%20AI.md#L908),
[1074-1116](../../../transcripts/learning%20with%20AI.md#L1074).

These mechanisms risk destroying trust, rewarding performance theater, and
making production work unreliable.

### Refinements and Tensions

`REFINEMENT`: S03 protects first-pass thinking. S07 gives AI an active role
before a solution: it may choose the probe, but it should not author the
learner's model.

`REFINEMENT`: The ultimate success condition is reduced dependence on AI for
question generation, not merely reduced dependence for answers.

`QUESTION`: A Socratic question is only useful if selected from evidence about
the current model. Generic questioning would add friction without information.

`QUESTION`: Engagement features should follow learning quality, not lead it. The
later product transcripts must clarify how progress becomes visible without
turning the system into hollow points and streaks.
