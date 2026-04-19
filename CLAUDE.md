# less-opinionated-superpowers

Personal fork of [`obra/superpowers`](https://github.com/obra/superpowers). Minimal diff — only behavioral changes are applied; everything else is byte-for-byte upstream.

## Fork diff summary

- **Deleted:** `finishing-a-development-branch`
- **Kept as manual-only:** `subagent-driven-development`
- **Neutralized descriptions** (suppress auto-invoke): `brainstorming`, `executing-plans`, `requesting-code-review`, `writing-plans`
- **Patched body:** `executing-plans` — removed `finishing-a-development-branch` required sub-skill chain
- **Rewritten:** `using-superpowers` — replaced mandatory 1%-chance protocol with a light informational note listing auto-invoke vs manual-only skills

## Syncing upstream

```bash
git fetch upstream
git merge upstream/main
```

Resolve any conflicts against the fork diff above.
