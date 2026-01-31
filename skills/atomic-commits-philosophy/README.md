# atomic-commits-philosophy

Make your AI agent commit atomically by default — no commands needed.

## Install

```bash
npx skills add dibenkobit/skills
```

## What It Does

This is a **philosophy skill**, not a command. Once installed, your agent will:

- Commit after each logical unit of work
- Never bundle unrelated changes
- Use clear, conventional commit messages
- Split large changes into small commits

## No Invocation Needed

Unlike command-based skills, this one is always active. The agent internalizes the principle and applies it automatically when working with git.

## Example Behavior

You ask: "Add user authentication"

Agent does:
```
feat(auth): add User model with password hashing
feat(auth): add login endpoint
feat(auth): add JWT token generation
feat(auth): add auth middleware
test(auth): add authentication tests
docs(api): document auth endpoints
```

Instead of:
```
feat: add user authentication
```

## Also Available

If you prefer explicit control, see [atomic-commits](../atomic-commits/) — a command-based version you invoke with "commit atomically".

## License

MIT
