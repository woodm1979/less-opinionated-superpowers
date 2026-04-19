# less-opinionated-superpowers

Minimal-diff fork of [`obra/superpowers`](https://github.com/obra/superpowers). Preserves the `superpowers:*` skill namespace and all unchanged skills byte-for-byte. Only behavioral changes are applied.

## What's different from upstream

| Skill | Change |
|---|---|
| `brainstorming` | Description neutralized — no longer auto-invokes |
| `executing-plans` | Description neutralized; `finishing-a-development-branch` sub-skill chain removed from body |
| `requesting-code-review` | Description neutralized — no longer auto-invokes |
| `writing-plans` | Description neutralized — no longer auto-invokes |
| `using-superpowers` | Rewritten as light informational note with explicit auto-invoke vs manual-only lists |
| `finishing-a-development-branch` | **Deleted** |
| `subagent-driven-development` | **Deleted** |

## Installation

```bash
claude plugin marketplace add woodm1979/less-opinionated-superpowers
claude plugin install superpowers@less-opinionated-superpowers
```

## Auto-invoke skills

These fire automatically when their trigger conditions are met:

- `superpowers:systematic-debugging`
- `superpowers:verification-before-completion`
- `superpowers:using-git-worktrees`
- `superpowers:receiving-code-review`
- `superpowers:dispatching-parallel-agents`
- `superpowers:test-driven-development`

## Manual-only skills

These require explicit invocation:

- `superpowers:brainstorming`
- `superpowers:writing-plans`
- `superpowers:executing-plans`
- `superpowers:requesting-code-review`
- `superpowers:writing-skills`

## Syncing upstream

```bash
git fetch upstream
git merge upstream/main
```

## License

MIT — see LICENSE file.
