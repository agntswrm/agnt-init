# agnt-init

Initialize a project for agents

- Find the project root (`.git`, `package.json`, `go.mod`, or current working directory)
- If `AGENTS.md` or `CLAUDE.md` already exist, ask the user before overwriting
- Create `AGENTS.md` with this exact content:

```markdown
<!-- Do not edit or remove this section -->
This document exists for non-obvious, error-prone shortcomings in the codebase, the model, or the tooling that an agent cannot figure out by reading the code alone. No architecture overviews, file trees, build commands, or standard behavior. When you encounter something that belongs here, first consider whether a code change could eliminate it and suggest that to the user. Only document it here if it can't be reasonably fixed.

---
```

- Symlink `CLAUDE.md` to `AGENTS.md`
