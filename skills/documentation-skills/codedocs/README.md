# codedocs

Use this skill when generating AI-agent-friendly documentation for a git repo or directory, answering questions about a codebase from existing docs, or incrementally updating documentation after code changes. Triggers on codedocs:generate, codedocs:ask, codedocs:update, "document this codebase", "generate docs for this repo", "what does this project do", "update the docs after my changes", or any task requiring structured codebase documentation that serves AI agents, developers, and new team members.

## Overview

Codedocs generates structured, layered documentation for any git repository or code
directory - documentation designed to be consumed by AI agents first and human developers
second. Instead of flat READMEs that lose context, codedocs produces a `docs/` tree with
an architecture overview, per-module deep dives, cross-cutting pattern files, and a
manifest that tracks what has been documented and when. Once docs exist, the skill answers
questions from the docs (not by re-reading source code), and supports incremental updates
via targeted scope or git-diff detection.


