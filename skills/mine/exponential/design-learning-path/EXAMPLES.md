# Examples

## Compounding Research Path

Target: reason about distributed systems under failure.

```text
failure domains
-> unreliable communication
-> replication and consistency
-> coordination and consensus
-> operational tradeoffs
```

Example step: unreliable communication.

- **Prior foundation consumed:** process and failure-domain models
- **Limiting model:** a request either succeeds or fails cleanly
- **Breaking experience:** timeout after the remote side commits
- **Artifact:** retryable operation with explicit idempotency behavior
- **Future friction removed:** retries, duplicate delivery, and partial failure
  become one reusable model
- **Successors accelerated:** replication, transactions, queues, and consensus
- **Recontextualization:** earlier "service errors" become uncertain state
  transitions across a boundary
- **Pit of success:** the exercise forces explicit timeout, retry, and duplicate
  handling instead of allowing a happy-path implementation

The step compounds because one uncertainty model explains several later
systems. "Learn networking before databases" would not state that mechanism.

## Development Micro-Path

Blocked action: add transaction retries to an unfamiliar database client.

```text
retry trigger -> transaction boundary -> idempotent side effects -> return
```

The path excludes isolation taxonomy and distributed commit unless the blocker
requires them. Its gate is predicting which operations may repeat, implementing
the retry safely, and returning to the feature.
