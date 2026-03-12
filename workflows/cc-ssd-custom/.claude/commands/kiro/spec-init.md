---
description: Initialize a new specification with detailed project description
allowed-tools: Bash, Read, Write, Glob, AskUserQuestion
argument-hint: <project-description>
---

# Spec Initialization

<background_information>

- **Mission**: Initialize the first phase of spec-driven development by creating directory structure and metadata for a new specification
- **Success Criteria**:
  - Generate appropriate feature name from project description
  - Create unique spec structure without conflicts
  - Provide clear path to next phase (requirements generation)
    </background_information>

<instructions>
## Core Task
Generate a unique feature name from the project description ($ARGUMENTS) and initialize the specification structure.

## Execution Steps

1. **Check Uniqueness**: Verify `.kiro/specs/` for naming conflicts (append number suffix if needed)
2. **Create Directory**: `.kiro/specs/[feature-name]/`
   - If the directory already exists (e.g., from a prior `/kiro:intent-explore` session), reuse it instead of creating a new one
3. **Check for Prior Intent Exploration**: Check `.kiro/specs/[feature-name]/` for existing exploration artifacts
   - If **intent-spec.md exists**: proceed silently. Set `"intentSpec": true` in spec.json. The intentSpec grounds all subsequent phases.
   - If **not found**: Use `AskUserQuestion` to prompt:
     > "No intent exploration found for this feature. How would you like to ground requirements?"
     - Options: `"Run /kiro:intent-explore first (recommended)"` | `"Skip — proceed without grounding"`
     - If intent-explore: respond with `/kiro:intent-explore "[original description]"` and stop
     - If skip: proceed and set `"intentSpec": false` in spec.json
4. **Initialize Files Using Templates**:
   - Read `.kiro/settings/templates/specs/init.json`
   - Read `.kiro/settings/templates/specs/requirements-init.md`
   - Replace placeholders:
     - `{{FEATURE_NAME}}` → generated feature name
     - `{{TIMESTAMP}}` → current ISO 8601 timestamp
     - `{{PROJECT_DESCRIPTION}}` → $ARGUMENTS
   - Write `spec.json` and `requirements.md` to spec directory

## Important Constraints

- DO NOT generate requirements/design/tasks at this stage
- Follow stage-by-stage development principles
- Maintain strict phase separation
- Only initialization is performed in this phase
  </instructions>

## Tool Guidance

- Use **Glob** to check existing spec directories for name uniqueness
- Use **Read** to fetch templates: `init.json` and `requirements-init.md`
- Use **Write** to create spec.json and requirements.md after placeholder replacement
- Perform validation before any file write operation

## Output Description

Provide output in the language specified in `spec.json` with the following structure:

1. **Generated Feature Name**: `feature-name` format with 1-2 sentence rationale
2. **Project Summary**: Brief summary (1 sentence)
3. **Created Files**: Bullet list with full paths
4. **Grounding Status**:
   - If `intent-spec.md` exists: state which job statement, outcomes, and exploration mode will ground the requirements
   - If user skipped: note requirements will be description-only (ungrounded in user needs)
5. **Next Step**: Command block showing `/kiro:spec-requirements <feature-name>`
6. **Notes**: Explain why only initialization was performed (2-3 sentences on phase separation)

**Format Requirements**:

- Use Markdown headings (##, ###)
- Wrap commands in code blocks
- Keep total output concise (under 250 words)
- Use clear, professional language per `spec.json.language`

## Safety & Fallback

- **Ambiguous Feature Name**: If feature name generation is unclear, propose 2-3 options and ask user to select
- **Template Missing**: If template files don't exist in `.kiro/settings/templates/specs/`, report error with specific missing file path and suggest checking repository setup
- **Directory Conflict**: If feature name already exists, append numeric suffix (e.g., `feature-name-2`) and notify user of automatic conflict resolution
- **Write Failure**: Report error with specific path and suggest checking permissions or disk space
