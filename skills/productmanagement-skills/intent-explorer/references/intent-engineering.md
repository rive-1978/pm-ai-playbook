# Intent Engineering Reference

## Definition

Intent Engineering is the discipline of specifying what you want built precisely enough that an AI agent can execute it without guessing. It translates user problems and product objectives into structured specifications that both humans and AI systems can understand without ambiguity.

## Why It Matters

Traditional workflows (tickets, PRDs, verbal handoffs) rely on shared human context that AI agents lack. A vague request like "improve checkout speed" forces agents to guess at success metrics, constraints, and priorities. Intent Engineering eliminates guesswork by making requirements explicit and testable.

With AI coding agents capable of writing code instantly, specification quality has become the bottleneck.

## The IntentSpec — Five-Part Structure

Every intent specification follows this framework:

1. **Objective** — The user problem and why it matters (grounded in real evidence)
2. **User Goal** — The job-to-be-done from the user's perspective
3. **Outcomes** — Measurable success criteria (e.g., "reduce form completion to under 45 seconds")
4. **Edge Cases** — Boundary conditions and failure modes
5. **Verification** — How to confirm completion and validate the solution

## How IntentSpec Differs from Other Formats

| Format          | Focus                     | Gap                                                 |
| --------------- | ------------------------- | --------------------------------------------------- |
| **PRD**         | Describes features        | Doesn't define the user problem or success criteria |
| **User Story**  | Captures desires          | Missing evidence, completion criteria, constraints  |
| **Jira Ticket** | Assumes human context     | AI agents have no tribal knowledge                  |
| **Prompt**      | Optimizes one interaction | Doesn't structure the entire problem                |

IntentSpec adds evidence (why it matters), completion criteria (what "done" means), and constraints (what must not break). Designed for both human and machine consumption.

## Key Principle

A PRD says "add a dashboard." An IntentSpec states "users cannot find weekly metrics — surface them in under 2 clicks with <500ms load time."
