---
name: using-superpowers
description: Overview of available superpowers skills and their invocation mode
---

# Superpowers Skills

This plugin provides the following skills:

| Skill | Description |
|---|---|
| `superpowers:brainstorming` | Explores requirements and design before implementation |
| `superpowers:dispatching-parallel-agents` | Runs independent tasks in parallel subagents |
| `superpowers:executing-plans` | Executes a written implementation plan step by step |
| `superpowers:receiving-code-review` | Processes incoming code review feedback rigorously |
| `superpowers:requesting-code-review` | Dispatches a code reviewer subagent |
| `superpowers:systematic-debugging` | Structured root-cause analysis for bugs and failures |
| `superpowers:test-driven-development` | Red-green-refactor TDD workflow |
| `superpowers:using-git-worktrees` | Sets up isolated git worktrees for feature work |
| `superpowers:verification-before-completion` | Runs verification before claiming work is done |
| `superpowers:writing-plans` | Produces implementation plans from specs |
| `superpowers:writing-skills` | Creates new agent skills |

## Auto-Invoke Allowlist

These skills fire automatically when their trigger conditions are met:

- `superpowers:systematic-debugging` — any bug, test failure, or unexpected behavior
- `superpowers:verification-before-completion` — before claiming work is done or creating PRs
- `superpowers:using-git-worktrees` — when starting feature work that needs isolation
- `superpowers:receiving-code-review` — when receiving code review feedback
- `superpowers:dispatching-parallel-agents` — when facing 2+ independent parallelizable tasks
- `superpowers:test-driven-development` — any feature implementation or bugfix

## Manual-Only

These skills require explicit invocation by you or the user:

- `superpowers:brainstorming`
- `superpowers:writing-plans`
- `superpowers:executing-plans`
- `superpowers:requesting-code-review`
- `superpowers:writing-skills`
