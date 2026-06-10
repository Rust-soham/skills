# Domain Adapter Contract

A domain adapter supplies reality and curriculum structure to the universal
learning engine. It contains no learner-specific state.

## Required Sections

### Scope

- Domain or subdomain
- Capabilities included
- Explicit exclusions
- Conditions and versions that limit validity

### Ground Truth

- Primary or high-trust sources
- Executable or observable evidence
- Tools available for inspection
- Provenance and version for each unstable claim

### Domain Structure

- Core primitives
- Invariants and boundary conditions
- Prerequisite relations
- High-leverage thresholds
- Capabilities each threshold unlocks

### Limiting Models

For each common or observed misconception:

- Plausible old model
- Context where it works
- Condition where it fails
- More generative model
- Evidence distinguishing them

### Probe Library

For each probe:

- Target belief or capability
- Required prerequisites
- Prompt, task, or environment
- Prediction requested
- Variable isolated
- Expected evidence
- Hint ladder
- Verification and transfer task

### Artifacts and Gates

- Durable outputs that demonstrate capability
- Generative crossing criteria
- Supporting fluency that is not itself a threshold

## Authorship and Revision

Build adapters from:

- Trusted domain sources
- Expert accounts of changed perception
- Real use conditions and failure evidence
- Learner responses that expose previously missing misconceptions

New learner-derived misconceptions enter as candidates. Promote them only after
technical verification; recurrence may raise priority but does not make them
true.

Every factual claim that can change by version needs provenance. The adapter
must distinguish domain truth from a teaching hypothesis.

## Separation Rules

- Domain graph: what capabilities and transformations exist
- Learner graph: which models this learner currently demonstrates
- Project state: which versions, constraints, and failures exist here

Link these structures during a session. Do not merge them into one ontology.

Evidence:
[S01 domain autopsy](sources/S01-actual-roadmap.md#0-domain-autopsy),
[S02 threshold graph](sources/S02-elite-hacker-roadmap.md#threshold-graph),
[S09 universal adapters](sources/S09-socrates-product-exploration.md#universal-core-and-domain-adapters),
[S13 mutable belief graph](sources/S13-threshold-unlocks.md#belief-transition-graph).
