# Skills

skills that I use daily, some curated, some my own.

inspired from [Matt Pocock](https://github.com/mattpocock.skills)'s skill repository.

## Install

List the available skills in this repo:

```bash
npx skills@latest add rust-soham/skills --list
```

Install both exponential learning skills:

```bash
npx skills@latest add rust-soham/skills \
  --skill design-learning-path \
  --skill learn-deeply \
  --agent codex
```

Install one skill:

```bash
npx skills@latest add rust-soham/skills \
  --skill learn-deeply \
  --agent codex
```

The main public package is under
[`skills/mine/exponential`](./skills/mine/exponential/INDEX.md). The `other`
tree contains reference, inherited, experimental, or personal skills that are
not the center of this repo's public theory.

## Mine

- [Exponential learning](./skills/mine/exponential/INDEX.md)
- [design-learning-path](./skills/mine/exponential/design-learning-path/SKILL.md)
- [learn-deeply](./skills/mine/exponential/learn-deeply/SKILL.md)

## Other

- [Engineering](./skills/other/engineering/README.md)
- [Productivity](./skills/other/productivity/README.md)
- [Misc](./skills/other/misc/README.md)
- [Personal](./skills/other/personal/README.md)
- [In progress](./skills/other/in-progress/README.md)
- [Deprecated](./skills/other/deprecated/README.md)

## Development

List all local skill packages:

```bash
./scripts/list-skills.sh
```

Link active skills into the local Claude skills directory:

```bash
./scripts/link-skills.sh
```

Create a release note for user-facing changes:

```bash
npm run changeset
```

Merges to `main` run the release workflow, which opens or updates a Changesets
version PR. Merging that version PR creates tags and GitHub releases.
