# AI-Accelerated Learning: A Working Discussion

**Status:** User theory exploration. This is not a corpus-derived canonical
concept card, implementation spec, or evidence audit.

**Source:** [braindumpManifesto.md](../../braindumpManifesto.md) remains the
raw source. This companion keeps an extended discussion of its implications
without replacing, correcting, or sanitizing the original train of thought.

## The Starting Observation: AI Leverage Is Uneven

The motivating observation is not that senior developers merely type faster or
know a larger list of APIs. Senior developers can put AI coding tools into a
larger, more reliable production loop. They receive generated code, recognize
the shape of a plausible solution, notice where it violates the system's real
constraints, and repair or redirect it quickly.

Their advantage is therefore not just output generation. It is judgment over
output.

For a familiar stack, an experienced developer can often:

1. State what the change must preserve.
2. Predict the important behavior before running it.
3. Recognize overengineering, missing failure paths, wrong ownership, or a
   confused abstraction boundary.
4. Inspect the generated code through tests, types, logs, architecture, and
   product intent.
5. Turn a failed attempt into a sharper next request or a local repair.

This makes their usable delegation radius much larger. A change can be bigger
because the developer can still evaluate it as a whole.

The same explains why experience transfers across ecosystems. A developer who
has built several real systems has not only learned the named tools in those
systems. They have accumulated patterns for data flow, ownership, lifecycle,
failure, boundaries, observability, testing, and tradeoffs. A new framework is
not blank territory. It is a new surface that can be mapped onto a prior
pattern library.

For someone early in their development, the immediate problem is not simply a
smaller library of facts. It is a smaller set of lived patterns with which to
filter AI output. The person may be able to read generated code, but lack an
active model that says what should be suspicious, what needs a test, and what
will probably matter later.

## Delegation Is a Moving Boundary, Not a Binary Rule

The initial rule, `only delegate what I understand`, protects against blindly
accepting output. It is valuable, but too blunt as the whole learning strategy.
It can turn the current boundary of understanding into a permanent ceiling.

The more useful distinction is between two lanes.

### Production lane

Delegate only work that is sufficiently auditable for the current stakes. The
learner must be able to set constraints, inspect the result, recognize an
invalid result, and recover if it fails.

### Learning lane

Let the agent work beyond the learner's current model, but do not treat the
output as accepted production work. Treat it as a constructed environment:
something to predict, trace, modify, break, compare, rebuild, and judge.

This is how AI can take a learner beyond their present boundary without making
them responsible for un-auditable code in a real system. The unknown output is
not a black box that gets shipped. It becomes material for an intentionally
designed encounter.

The goal is to expand the delegation boundary over time. A useful definition is:

> **Delegation radius** is the size and novelty of a task a learner can give an
> agent while still being able to constrain, evaluate, and repair the result.

It should grow because the learner has stronger models and feedback habits, not
because they have become more comfortable accepting generated code.

## Agents as Learning Compression

The useful reading of agents as compression technology is not merely that they
produce more work in less time. In this learning system, they compress the time
and incidental friction between a learner's attempt, a revealing encounter with
reality, and the next self-owned model update.

```text
learner action or prediction
-> evidence that exposes the important mismatch
-> learner reconstruction
-> verified new capability
```

Without good guidance, the path between those moments can be filled with
irrelevant setup, documentation hunting, boilerplate, version confusion, noisy
experiments, broad unfocused exploration, or failures that do not reveal the
model the learner needs. An agent can remove or shorten that friction by
retrieving narrow evidence, constructing a runnable environment, isolating a
variable, making hidden behavior visible, and returning the learner to the
actual project.

What must remain with the learner is the cognition that makes the compression
matter: forming a rough prediction, selecting or judging an action, noticing
the discrepancy, reconstructing the model, applying it, and eventually
generating the next useful question. The agent is not meant to compress those
operations into a supplied conclusion. It makes the interval around them more
information-dense.

This is why threshold concepts can arrive sooner without becoming borrowed
understanding. The learner reaches more high-signal, causally interpretable
encounters in the same amount of project time, while still doing the actual
model change themselves. The threshold is not handed over; the route to the
threshold becomes less clogged.

The compact thesis is:

> Use AI to compress unimportant friction and the delay between meaningful
> feedback loops, while preserving and sharpening the learner's own inference.

## Meta-Learning: Accelerating the Acceleration

The larger ambition is not simply to add a fixed amount to a learner's rate of
progress. It is to improve the processes by which they learn, notice gaps,
choose experiments, interpret feedback, and transfer a repaired model into the
next unfamiliar system.

Let `U(t)` represent accumulated understanding. The theory is concerned with
more than making `U(t)` rise or even making the understanding rate `U'(t)` rise.
Some learners already have an accelerating understanding rate, represented by
`U''(t)`. The stronger aim is to make that acceleration itself increase: a
positive `U'''(t)`. In the Newtonian analogy, understanding is position, the
rate of understanding is velocity, the growth of that rate is acceleration, and
the growth of that acceleration is jerk.

The system is therefore trying to accelerate the learner's accelerating ability
to understand. A well-designed feedback-and-model-repair flywheel does not just
produce another answer; it improves the learner's capacity to reach the next
answer at a faster increasing rate. Over a compounding phase, that can create
the kind of self-reinforcing, potentially exponential curve the theory is
trying to engineer.

```text
better model
-> better prediction and judgment
-> better question and experiment selection
-> higher-signal feedback
-> faster model repair
-> stronger pattern extraction and transfer
-> a better model for the next domain
```

The agent contributes by shaping this loop, but the metacognitive gain must
become the learner's own. The learner gradually becomes better at:

- Recognizing what they do not yet understand.
- Distinguishing a missing fact from a broken model.
- Finding the assumption that would be most informative to test.
- Designing or requesting the next revealing experiment.
- Compressing a project incident into a reusable pattern.
- Mapping that pattern into a new domain without mistaking analogy for proof.

This is why the theory reaches beyond better tutoring. It treats metacognition
as a trainable capability whose improvement raises the quality of every later
learning loop. The agent does not have to own the learner's thinking for this
to happen. Its job is to make the learner's own cognitive updates more frequent,
sharper, and more transferable until the learner increasingly generates the
loop without external steering.

## Two Invariants at Different Scales

The theory has two invariants, but they are not peer-level alternatives.

1. **Curriculum as leverage architecture** is the primary invariant. It decides
   which capability transitions come first, what each one unlocks, how they
   compound, and how the entire path creates a pit of success.
2. **Mental-model improvement** is the step-level invariant. It is the process
   used to move the learner through one curriculum transition selected by the
   larger path.

The first invariant determines the sequence. The second determines what happens
inside a stage of that sequence. Feedback-loop quality and earned progression
depend first on whether the curriculum selected a meaningful next transition,
made its feedback informative, and connected the resulting capability to a
real successor.

## The Step-Level Invariant: Mental Model Improvement

Mental-model improvement is not a competing curriculum philosophy, prompt
style, or type of exercise. It is the loop that changes what the learner can
perceive and do after the curriculum has selected the next transition.

```text
current model
-> prediction, explanation, or attempt
-> targeted encounter with reality
-> noticed mismatch
-> self-owned reconstruction
-> application in an artifact
-> pattern compression
-> transfer or a slightly larger delegation boundary
```

A mental model here is not a polished verbal explanation. It is an active
structure that lets the learner predict behavior, select an action, review
generated code, detect an important difference, and know what evidence would
change their mind.

Refinement can happen in several directions:

- **Addition:** a missing primitive, relationship, or constraint becomes
  available.
- **Reorganization:** formerly separate facts become one generative model.
- **Subtraction:** an appealing but wrong default assumption is removed.
- **Reframing:** the same material is viewed through a more useful coordinate
  system.
- **Compression:** many surface cases become one reusable pattern.
- **Boundary discovery:** the learner sees where a model stops applying.

This explains why learning can feel contradictory. Sometimes progress feels
like adding a new layer. Sometimes it feels like stripping one away. Sometimes
the same concept appears in a strange context and suddenly becomes more real.
Those are different kinds of model change, not evidence that the theory has
lost its shape.

The learner's limited active attention is a design constraint for the loop.
Each encounter should isolate a small causal surface, then let the resulting
relations coalesce into a chunk before adding another foreign surface. This is
why a tiny executable example can be more educational than a broad explanation:
it can make one relationship observable without demanding that every other
relationship be held in mind at once.

## Tools Are Not the Theory

Inversion, targeted examples, hidden-control-flow traces, contrastive cases,
tiny projects, counterexamples, and worked examples are not competing learning
philosophies. They are tool types inside the same refinement loop.

The tool should be chosen from the learner's limiting model and the domain's
causal structure.

| When the learner needs to see... | Useful intervention shape |
| --- | --- |
| Ordering, time, hidden execution, or lifecycle | Trace, prediction gate, or altered event order |
| A default assumption that appears invisible | Inversion, removal, or a boundary case |
| Two cases that look the same but behave differently | Controlled contrast pair |
| An abstraction whose machinery is hidden | Minimal rebuild or simplified toy implementation |
| Whether a model survives integration | Tiny real project or constrained feature slice |
| Whether they can judge agent output | Plausible alternatives, review, and failure diagnosis |
| Whether the model transfers | A new context with the same structural demand |

The agent should not select a tool because it has a favorite teaching style. It
should first form a tentative diagnosis: what does the learner currently expect
to happen, and which one assumption would produce the most informative
mismatch? The intervention is then selected for its ability to expose that
assumption while keeping the learner inside a solvable world.

## The Primary Invariant: Curriculum as Leverage Architecture

The curriculum-design philosophy here is the synthesis of
[S01: Actual Roadmap](sources/S01-actual-roadmap.md) and
[S02: Elite Hacker Roadmap](sources/S02-elite-hacker-roadmap.md). The earlier
idea of different "exponential steps formations" is central, but there are two
nested scales that must not be collapsed.

At the **curriculum scale**, the philosophy is invariant across every learning
goal. It designs a sequence of model transitions so that each step consumes
earlier foundations, increases generative capability, reduces the friction and
active cognitive burden of later learning, and unlocks stronger questions,
feedback, artifacts, and choices. The sequence is designed so that the correct
next action becomes the easiest natural action: a pit of success.

That means every curriculum, whether it starts from a build blocker, a research
question, a new framework, or a long-term project goal, follows the same
sequencing logic:

1. Define the target generative capability and independent success condition.
2. Map the domain's thresholds, prerequisites, limiting models, and real use
   conditions.
3. Locate the learner from evidence rather than assumed exposure.
4. Choose the highest-leverage reachable transition.
5. Sequence it so it reuses prior foundations and makes later transitions
   cheaper.
6. Give the learner a pit-of-success environment with a generative gate,
   artifact, and fast reality feedback.
7. Recontextualize, compress, and replan from the new evidence.

### Feedback Loops and Gamification Depend on the Sequence

A feedback loop is not high quality merely because it is fast. Its quality
comes from where it sits in the curriculum. A well-sequenced transition gives
the learner a challenge they can meaningfully attempt, makes the result
interpretable through the foundations they already own, exposes the next
important mismatch, and turns the repair into an action that unlocks a real
successor.

Gamification follows the same architecture. It should not paste rewards onto
arbitrary activity. Each level, unlock, visible capability delta, and final boss
should correspond to a real transition in the leverage graph. The learner is
pulled forward because the prior step made the next meaningful action newly
possible and naturally attractive: the curriculum itself creates the pit of
success.

At the **step scale**, the mental-model refinement loop is how one selected
transition is actually lived through. This is where an agent uses a prediction,
controlled collision, inversion, targeted example, tiny project, or another
tool to reveal and repair one limiting assumption.

Mission does not change the curriculum philosophy or the logic by which steps
compound. It changes the target, the domain graph, the learner's starting
location, the appropriate step size, and the concrete form of the
pit-of-success environment. It may also change the point at which the learner
returns to building, broadens into research, or proves transfer.

| Mission | What the path optimizes | Stop condition |
| --- | --- | --- |
| Unblock a build | The smallest untanglement that restores a real next action | The learner can make the relevant project decision and continue building |
| Research a domain | A navigable map of primitives, boundaries, unknowns, and worthwhile next questions | The learner can orient themselves and choose credible experiments |
| Untangle an abstraction | Visibility into the mechanism the abstraction hides | The learner can predict, alter, or reconstruct the important mechanism |
| Build a layered roadmap | A sequence in which each capability is reused and makes the next one cheaper | Each level creates a real artifact and unlocks its successor |
| Transfer or final boss | Evidence that the model survives a novel constraint or setting | The learner recognizes the same structure without cosmetic prompting |

The universal curriculum architecture is therefore:

```text
mission and target capability
-> domain threshold graph and learner evidence
-> highest-leverage reachable transition
-> path step that consumes prior foundations
-> step-scale model refinement and real feedback
-> pit-of-success next action and artifact
-> compression, transfer, and updated learner evidence
-> reordered or extended path
```

`design-learning-path` should be driven by this choice of mission before it
orders a path. It should not treat an urgent build blocker as a miniature
semester, or a research mission as a series of forced quick wins. Mission
changes the concrete path, but the compounding sequencing philosophy remains
the same. Mental-model refinement is the engine inside each path step, not a
replacement for curriculum design.

## The Deep Dilemma: Who Generates the Questions?

The most ambitious part of the manifesto is not that AI can generate examples
or explain a framework. It is the concern that recursive questioning itself may
be part of the faculty that enlarges understanding.

If an agent always supplies the diagnostic question, a learner may become very
good at responding to well-formed prompts without becoming better at noticing
which question needs to be asked. That would create a sophisticated dependency:
the agent improves local answers but owns the steering loop.

The response is not to ban agent-generated questions. Some unknown unknowns
are genuinely outside the learner's present frame, and the agent can function
as an external source of comparison, examples, and candidate experiments. The
design requirement is that external question generation must become visible and
eventually transferable.

```text
1. Agent supplies a diagnostic question.
2. Learner explains what makes that question diagnostic.
3. Learner proposes the next probe, inversion, or boundary case.
4. Agent judges the information value of that probe and supplies a sharper
   alternative when needed.
5. Learner runs the same probing operation in a new domain.
6. Agent recedes to blind-spot checking and evidence retrieval.
```

The system should occasionally reveal its own reasoning in an operational form:

- What competing models did this question distinguish?
- What observation would each model predict?
- Why is this a better next question than another plausible question?
- What would change the current diagnosis?

The target is not a learner who asks many recursive questions. It is a learner
who can generate questions with high information value: questions that divide
plausible models, expose a hidden dependency, locate a boundary, or identify
the next useful experiment.

This turns the apparent cap into a product requirement. The agent is not merely
the Socratic questioner. It is a temporary coach for the learner's own question
generation process.

## What "Exponential" Can Mean Here

The term is not about promising a magical numeric growth curve. It names a
compounding mechanism: one successful repair should improve several later
loops, not only solve the immediate exercise.

A high-leverage model repair can improve:

- The learner's ability to predict the next system.
- The quality of the constraints they give an agent.
- Their ability to recognize bad generated code.
- Their debugging speed after a failure.
- Their ability to map a new library onto a known structure.
- Their ability to generate the next discriminating question.
- Their delegation radius.

The compounding system has at least three nested loops:

```text
real artifact feedback
-> better domain model
-> stronger pattern extraction and transfer
-> better metacognitive probes
-> better choice of the next artifact feedback loop
```

The agent's leverage is not that it completes every step. Its leverage is that
it can reduce the time spent in uninformative wandering, construct a more
revealing next encounter, and preserve the evidence that makes the repair
reusable later.

## Engagement and Pits of Success

Gamification, in this theory, should not mean points pasted onto arbitrary
lessons. It should make capability growth legible and make the worthwhile next
move easier to take.

The design system is what gets gamified, not the learner's cognition. The agent
can shape missions, constraints, progression, feedback surfaces, unlocks,
artifacts, and the next reachable challenge. The learner must still form the
prediction, notice the mismatch, judge the evidence, reconstruct the model,
and carry the model into a new setting. The system makes those cognitive acts
more compelling, more visible, and more frequently successful; it does not
replace them with a generated conclusion.

A good loop has:

```text
meaningful goal
-> challenge with a visible success condition
-> a mismatch that can be repaired
-> an earned capability delta
-> a real artifact or newly available action
-> authentic curiosity about the next frontier
```

The reward is not a streak. It is the felt difference between not being able to
predict, build, review, or delegate something and then being able to do it.
That is the form of obsession worth designing for: return driven by growing
agency and meaningful work, not by artificial incompleteness or borrowed
pressure.

### Rollout: Default Core, Later Opt-In Deep Engagement

The immediate system does not need the full game-design layer to be useful. The
default should remain the existing core:

```text
leverage-ordered curriculum
-> Socratic probe or targeted exercise for one path step
-> learner-owned repair and verification
-> return to the real artifact or next path step
```

That solves the current need while the system earns trust through real use. A
later **deep-engagement mode** can be explicitly opted into for demanding,
longer learning missions such as category theory, Rust, Scala, or another
subject where sustained contact and a richer progression structure help.

This mode should make the work intensely absorbing through meaningful missions,
visible earned progression, short high-signal loops, reachable next challenges,
real artifacts, and an intelligible path toward a final boss. It must still be
voluntary and preserve the learner's ability to pause, change modes, or leave.
The goal is not to make the learner unable to avoid the system. It is to make
returning feel compelling because each session visibly enlarges their agency
and makes the next worthwhile action available.

The mode remains deferred until the basic curriculum-and-probe loop has been
field-tested. It is an environment layer around learner-owned cognition, not a
replacement for it.

For programming, the strongest proof of progress is often not an exercise score
but a changed project action: a stuck feature moves, a debugging session becomes
directed, a library's behavior becomes legible, or a formerly frightening diff
becomes reviewable.

## How This Becomes a Coding Learning System

The system should operate in contact with real code, not only in conversations
about code. A useful development session can be represented as:

```text
artifact goal
-> learner attempt
-> observed blocker
-> mission classification
-> current-model capture
-> targeted probe or environment change
-> learner prediction and repair
-> return to the artifact
-> verification
-> pattern and delegation-boundary update
```

For example, a learner blocked by an unfamiliar framework feature should not be
sent immediately into an entire tutorial. The system can identify whether the
blocker is about data flow, control flow, lifecycle, typing, ownership, or a
project-local convention. It can then construct the smallest example that
preserves the causal relationship the project depends on, let the learner make
a prediction, and return them to the feature with a model that is now usable.

The development loop also creates the "battle-tested" quality the manifesto
cares about. A pattern is no longer only theoretically understood when it has
survived a real constraint, made a prediction possible, helped diagnose a
failure, and been recognized in a different context.

## Recursive Curriculum and Workspace Shape

Longer goals can recurse the curriculum architecture. A root curriculum does
not need to flatten every threshold into one enormous list. When one transition
has its own target capability, prerequisite graph, several meaningful stages,
and a clear contribution back to its parent, it can become a child curriculum.

```text
root mission
-> root curriculum transition: become capable of X
   -> child curriculum: acquire the threshold sequence for X
      -> one selected path step
         -> mental-model improvement exercise
            -> verified record returns an unlock to the child path
   -> child completion returns an unlocked capability to the root path
```

This is close in spirit to
[handoff](../../skills/other/productivity/handoff/SKILL.md): each scope needs a
compact resume point that lets the next session or agent continue without
reconstructing an entire conversation. The difference is that a curriculum
handoff is not a transcript summary. It carries the learning state that changes
the next action: target capability, current path node, evidence, verified
models, unresolved questions, and the parent return contract.

### Proposal: Separate the Lab from the Learning State

A root-level `scratchpad/` is a good default for new coding projects, but it
should be the **runnable lab**, not the sole registry for curriculum state. It
is where targeted examples, minimal reproductions, traces, toy systems, and
failure experiments live. Keeping durable learning context only beside those
files would mix executable experiments with the state that explains why they
exist and what they proved.

Use the workspace-local `.learning/` state for that durable context and
`scratchpad/` for the code that makes a model visible:

```text
<project>/
├── .learning/
│   ├── MISSION.md
│   ├── CURRICULUM.md
│   ├── STATE.md
│   ├── records/
│   │   └── <verified-model-transition>.md
│   └── paths/                         # Create only when recursion is useful
│       └── <capability-slug>/
│           ├── CURRICULUM.md
│           ├── STATE.md
│           └── records/
└── scratchpad/
    └── <capability-or-step-slug>/
        ├── EXERCISE.md
        ├── <runnable-example>
        └── <minimal-reproduction-or-trace>
```

`EXERCISE.md` should stay small: its parent path, the one question or prediction,
how to run the experiment, and the expected evidence. The verified conclusion
belongs in `.learning/records/`, where it can update the curriculum and be
found by a later session without reading every scratch file.

Create a child curriculum only when it has an independent target, multiple
transitions, and a meaningful return condition. A single controlled collision
should remain a path step with a record, not become a folder hierarchy. This
keeps recursion useful instead of turning the learning system into paperwork.

The version-control treatment of `.learning/` and `scratchpad/` should remain a
deliberate project decision. The useful structural boundary exists either way:
durable curriculum evidence is separate from disposable experimental code.

## Candidate Programmer Helper: Untangle a Library Knot

An unfamiliar library, framework, or abstraction is not one unknown. It bundles
several untouched primitives behind a convenient surface: purpose, input and
output shape, hidden control flow, lifecycle, ownership, failure semantics,
composition rules, and project conventions. A learner blocked by it needs a
helper that turns this bundle into the smallest useful model path, not a broad
tutorial or a dump of source code.

This helper should be a programmer-specific operator used by `learn-deeply`,
not a replacement for either `learn-deeply` or `design-learning-path`.

```text
design-learning-path
-> selects the high-leverage library/framework transition
   -> learn-deeply
      -> invokes untangle-library-knot for the step's abstraction
         -> learner-owned repair and project return
```

### Contract

**Inputs**

- Exact project action currently blocked or the research capability desired
- Library/framework name, installed version, and relevant API surface
- Learner's current theory or prediction, however rough
- Real evidence: code, types, diagnostics, tests, logs, runtime trace, or docs
- Mode: unblock/build or research/untangle

**Outputs**

- One named knot and the smallest model delta that matters now
- A runnable scratchpad experiment or a grounded project probe
- A verified rule, boundary, and immediate project return action
- A local model-transition record when the repair survives verification

### Procedure

1. Ground the real version and disputed behavior before teaching it.
2. Separate the bundle into candidate knots: purpose, primitive, control flow,
   lifecycle, type shape, ownership, composition, failure boundary, or local
   convention.
3. Choose only the upstream knot that blocks the active path step. In build
   mode, choose the minimum knot needed to resume the feature; in research
   mode, choose the next leverage threshold in the wider abstraction map.
4. Ask for a prediction or attempted explanation that makes the current model
   visible.
5. Select the intervention that exposes the hidden mechanism:
   source-contract reading, a type-shape probe, a runtime trace, a contrast
   pair, omitted-step inversion, failure injection, or a minimal rebuild.
6. Let the learner interpret the result, name the failed assumption, and state
   the repaired model.
7. Reapply the model immediately in the real project or verify it in a novel
   case. A passing scratchpad alone is not completion.

### Scratchpad Shape

```text
scratchpad/<library-knot>/
├── EXERCISE.md        # Question, prediction, run command, expected evidence
├── baseline.<ext>     # The smallest normal case
├── boundary.<ext>     # One changed variable or failure case
└── trace.<ext>        # Optional observability when timing/control flow matters
```

The scratchpad is an environment the agent curates for FAFO. It should preserve
the causal relationship from the project while removing irrelevant setup and
documentation hunting. It should not become a detached collection of examples.

### Candidate Internal Operators

Do not create a separate tool for each item yet. First field-test the whole
library-knot helper on real blockers. Repeated operations can later become
small, reusable tools:

- **API surface mapper:** identify the narrow type, declaration, source, and
  version facts that define the current contract.
- **Control-flow tracer:** make construction, execution, scheduling, callback,
  error, and resource behavior visible.
- **Collision generator:** construct a baseline, contrast, inversion, or
  failure case for one limiting assumption.
- **Minimal rebuild guide:** expose an abstraction by recreating only its
  load-bearing primitive or relation.
- **Project bridge:** apply the repaired model to the original feature and
  record the return action.

The first field-test question is simple: after using this helper on an actual
library knot, can the learner predict the relevant behavior, alter it safely,
review generated code using the model, and resume the project? If not, the
helper created an interesting exercise but did not untangle the abstraction.

## Global and Local Learning Context

The system needs two contexts because "the learner knows X" and "this project
uses X in this particular way" are different facts.

### Global: portable learner evidence

`~/.learning/` follows the learner across workspaces. It is not a giant profile
or a list of topics they have encountered. It is a compact, queryable library of
evidence-backed anchors that an agent can reuse when a new project has the same
underlying structure.

```text
~/.learning/
├── LEARNER.md       # Short index of demonstrated anchors and calibration
├── PATTERNS.md      # Cross-domain patterns and their failure boundaries
└── records/         # Detailed verified transitions and supersession history
```

An anchor should say more than "knows React" or "knows concurrency":

```md
## Anchor: UI state, render, and effect lifecycle
- Status: candidate | verified | challenged | superseded
- Demonstrated capability and evidence:
- Reusable structure:
- Use as an analogy for:
- Known boundaries and non-transfer:
- Source records:
- Last verified:
```

The learner can explicitly declare an anchor they want the agent to use. The
agent should record that as a candidate when no demonstration exists yet, start
from it rather than reteaching the whole topic, and still seek a quick relevant
prediction or reconstruction before allowing it to skip an important
prerequisite.

### Local: mission and project reality

`<workspace>/.learning/` belongs to the active project. It records the current
artifact, versions, architecture, constraints, current path node, blocker,
sandbox, and return action. This is the context that keeps an agent from
applying a true global pattern in the wrong local situation.

```text
<project>/.learning/
├── MISSION.md
├── PROJECT.md
├── CURRICULUM.md
├── STATE.md
├── records/
└── paths/
```

Local state should reference a global anchor by its identifier and record only
the current mapping, not copy the whole global record:

```md
## Relevant global anchors
- Anchor: ui-state-render-effect-lifecycle
  Shared structure: state change -> scheduled work -> observable output
  New-project delta: server/client boundary and framework-specific lifecycle
  Boundary to verify: which work is server-only and when it actually runs
```

### Retrieval and Promotion Flow

When entering a new project, the agent should:

1. Read the local mission and project evidence first.
2. Retrieve only a small number of global anchors relevant to the current
   target, not the entire learner history.
3. State the structural mapping and the expected difference when an anchor is
   used to compress the path.
4. Use current project evidence, types, tests, runtime behavior, and learner
   responses to confirm or reject that mapping.
5. Write new project-specific findings locally.
6. Promote a local finding globally only after it has been compressed into a
   portable pattern and survived transfer or reconstruction evidence.

This gives the agent the behavior you want: in a new project it can say, "you
already have a demonstrated model for X, so I will build from it; here is the
delta that matters in this system." It does not need to re-teach X, and it does
not pretend that knowing X proves the new library or project behaves the same
way.

The rule is: **global context supplies anchors; local context supplies truth for
the active mission.**

## What Would Count as Evidence That the System Is Working?

Visible completion alone is weak evidence. The theory should look for changes
in behavior that make larger, safer AI-assisted work possible.

- The learner predicts important behavior before running code more often and
  with greater accuracy.
- They state constraints and failure paths before asking an agent to implement.
- They detect a suspicious or invalid generated solution without needing the
  agent to point it out first.
- They recover from a failed generation by forming a sharper diagnosis.
- They produce a useful next question, boundary case, or experiment on their
  own.
- A pattern learned in one library appears in their reasoning about another.
- Their acceptable delegation radius expands while their review quality holds.
- They return from learning detours to the real artifact with a concrete action.

These behaviors matter more than how many topics, examples, prompts, or
sessions have been completed.

## Open Questions Worth Keeping Open

This theory is strongest when it keeps its hard questions visible instead of
declaring the system finished.

1. How does the agent distinguish productive confusion from overload early
   enough to adjust the environment without stealing the learner's repair?
2. How can it infer a limiting model from sparse code, language, or behavior
   without pretending to know the learner's mind?
3. What is the right intervention when the learner lacks a model versus when
   they simply lack a retrievable fact, tool command, or version-specific detail?
4. How should review and production taste be trained, not only conceptual
   correctness?
5. What evidence shows that an apparent insight has become transferable rather
   than remaining tied to the exact example that produced it?
6. When does a real project contain too much incidental complexity, requiring a
   toy world, and when does simplification remove the very feedback that makes
   the lesson matter?
7. How can the system make its own choice of probes legible without turning
   every learning moment into a meta-lecture?
8. What is the smallest durable learner state that preserves model changes,
   question-generation growth, and delegation calibration without becoming a
   surveillance archive or a burden to maintain?

## Working Thesis

AI can make learning dramatically faster when it is used neither as a mere
answer machine nor as a strict gatekeeper that refuses to go beyond the
learner's current knowledge. It should act as a feedback-loop designer: it
constructs informative encounters, preserves learner ownership of the model
repair, grounds the loop in real artifacts, and gradually transfers the ability
to choose the next question.

For coding, the intended result is not simply more completed code. It is a
learner whose internal pattern library, review judgment, diagnostic ability,
question generation, and delegation radius grow together. That is how AI output
can become a route to genuine production capability rather than a substitute
for it.
