# atomic-commits

Split staged git changes into logical atomic commits.

## Install

```bash
npx skills add dibenkobit/atomic-commits
```

Works with: **Claude Code**, **Cursor**, **Windsurf**, **GitHub Copilot**, and [20+ other AI agents](https://skills.sh).

## Usage

```
> commit atomically
```

or

```
> /atomic-commits
```

## What it does

Instead of one big commit:
```
feat: add auth, update deps, fix typo
```

You get atomic commits:
```
feat(auth): implement OAuth2 flow
chore(deps): update dependencies
fix(docs): correct typo in README
```

## Features

- Respects project conventions (commitlint, commitizen, .babygit.json)
- Follows user instructions ("use gitmoji", "write in Russian")
- Falls back to analyzing recent commits style
- Validates all files are included, no duplicates
- Asks for confirmation before committing

## License

MIT
