# Changesets

This repo uses Changesets for user-facing release notes, version bumps, git
tags, and GitHub releases.

For a public skill or tooling change, run:

```bash
npm run changeset
```

Commit the generated `.changeset/*.md` file with the change. When it reaches
`main`, the release workflow opens or updates the version PR.
