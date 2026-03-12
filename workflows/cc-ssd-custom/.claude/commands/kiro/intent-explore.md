---
description: Explore user intent before specification work. Delegates to intent-explorer skill when available.
argument-hint: <problem-or-idea-description>
---

Invoke the `intent-explorer` skill with args `$ARGUMENTS`.

If the skill is not found, ask the user whether to install it or skip to `/kiro:spec-init "$ARGUMENTS"`.
