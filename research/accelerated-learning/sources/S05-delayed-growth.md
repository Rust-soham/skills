# S05: Delayed Growth, Exponential Jump

Source: `transcripts/Delayed Growth, Exponential Jump.md`

Status: cross-checked

## Evidence Notes

### Learner Pattern

The user reports recurring slow initial progress followed by abrupt gains after
fundamentals align, using badminton as the immediate example
([11-14](../../../transcripts/Delayed%20Growth%2C%20Exponential%20Jump.md#L11)).

The response models this as hidden accumulation of subskills followed by a
visible threshold when they coordinate
([46-93](../../../transcripts/Delayed%20Growth%2C%20Exponential%20Jump.md#L46)).

`SOURCE`: The relevant personal traits are tolerance for appearing bad,
correctness over ego, delayed gratification, and sustained fundamentals
([115-159](../../../transcripts/Delayed%20Growth%2C%20Exponential%20Jump.md#L115)).

`QUESTION`: The source overstates this as a fixed "learning personality." The
useful evidence is the observed pattern and preference, not a permanent learner
type.

### AI Assistance Contract

The proposed help ladder is:

1. Nudge
2. Structured hint
3. Partial code or skeleton
4. Full solution as last resort

([215-259](../../../transcripts/Delayed%20Growth%2C%20Exponential%20Jump.md#L215))

Before implementation help, ask for the learner's approach so they remain the
architect rather than a reviewer of completed work
([301-320](../../../transcripts/Delayed%20Growth%2C%20Exponential%20Jump.md#L301)).

A task loop:

1. Learner chooses structure.
2. AI probes omitted constraints and failure modes.
3. Learner attempts.
4. AI supplies narrow mechanical help.
5. AI critiques the result.

([323-384](../../../transcripts/Delayed%20Growth%2C%20Exponential%20Jump.md#L323))

The agent should sometimes disagree or present alternatives to force
justification, not to seize the decision
([449-463](../../../transcripts/Delayed%20Growth%2C%20Exponential%20Jump.md#L449)).

### Delegation Threshold

`SOURCE`: Familiarity should increase how much execution can be delegated, but
not how much understanding is abandoned. The meaningful measure is how much of
the system the learner can mentally simulate
([388-416](../../../transcripts/Delayed%20Growth%2C%20Exponential%20Jump.md#L388)).

The source proposes output judgment as a senior signal: detecting fragility,
overengineering, and contextual fitness quickly
([420-445](../../../transcripts/Delayed%20Growth%2C%20Exponential%20Jump.md#L420)).

### Compressing the Slow Phase

`REFINEMENT`: The agent cannot remove the model-building phase. It can compress
time spent in undirected confusion
([518-534](../../../transcripts/Delayed%20Growth%2C%20Exponential%20Jump.md#L518)).

The target is **speed of correct realization**, not generic speed of learning
([538-546](../../../transcripts/Delayed%20Growth%2C%20Exponential%20Jump.md#L538)).

The source calls the desired state **structured confusion**: guiding attention
toward the right struggle
([567-601](../../../transcripts/Delayed%20Growth%2C%20Exponential%20Jump.md#L567)).

Three compression levers:

1. **Reduce randomness** by identifying the most likely conceptual weak point.
2. **Increase feedback clarity** by naming exact conditions and failure modes.
3. **Force correct focus** by removing currently irrelevant material.

([604-657](../../../transcripts/Delayed%20Growth%2C%20Exponential%20Jump.md#L604))

For this learner specifically:

- Front-load the correct struggles
- Increase feedback iterations per hour
- Detect practice-target misalignment early

([692-735](../../../transcripts/Delayed%20Growth%2C%20Exponential%20Jump.md#L692))

When stuck, the agent should identify the current struggle, narrow focus, state
what to ignore, and offer one small next action
([738-748](../../../transcripts/Delayed%20Growth%2C%20Exponential%20Jump.md#L738)).

### Clicks Are Evidence, Not Targets

The user strongly desires recurring step-function gains
([804-806](../../../transcripts/Delayed%20Growth%2C%20Exponential%20Jump.md#L804)).

The response warns against optimizing for intensity and breakthroughs rather
than process. Clicks are side effects of fundamentals, confusion, repeated
adjustment, and eventual compression
([818-888](../../../transcripts/Delayed%20Growth%2C%20Exponential%20Jump.md#L818)).

The desired unit is a high-quality repetition inside confusion, not the
breakthrough feeling itself
([910-967](../../../transcripts/Delayed%20Growth%2C%20Exponential%20Jump.md#L910)).

`REFINEMENT`: Treat visible breakthroughs as checkpoints that validate the
process, not events to manufacture directly
([988-1004](../../../transcripts/Delayed%20Growth%2C%20Exponential%20Jump.md#L988)).

### Signals and Metrics

- Can the learner state an approach before help?
- Can they mentally simulate normal and failure behavior?
- How quickly can they detect bad output?
- How quickly can they identify the precise unknown?
- Are iteration cycles increasing without reducing cognitive ownership?
- Is effort aimed at the actual bottleneck?

The source's strongest metric is the speed with which the learner identifies
what they do not understand
([751-771](../../../transcripts/Delayed%20Growth%2C%20Exponential%20Jump.md#L751)).

### Failure Modes

- Full solutions before an attempt
- Help that jumps several hint levels
- Implementation aid before the learner states a design
- Delegating code the learner cannot simulate
- Increasing practice volume against the wrong bottleneck
- Making learning smooth by eliminating useful mistakes
- Chasing breakthrough intensity and switching domains prematurely
- Interpreting invisible progress as regression

### Tensions

`QUESTION`: "No full solutions by default" is appropriate for learning mode but
must coexist with a production mode where the learner already owns the model and
delegates execution.

`QUESTION`: The agent is expected to diagnose the likely weak point, but later
sources must establish how it gathers enough evidence rather than guessing.

`SYNTHESIS`: The progressive hint level should be selected from demonstrated
learner state, not a fixed preference.
