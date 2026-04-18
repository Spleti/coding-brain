---
type: tool-profile
tool: codex
tags:
  - coding-agent
  - prompting
use_cases:
  - implementation
  - debugging
  - testing
confidence: high
last_reviewed: 2026-04-18
---

## Strengths
- Strong at executing well-defined coding tasks end-to-end
- Can modify multiple files and run workflows (tests, commands)
- Good at verifying its own work when instructed
- Works well in CLI/agent-style workflows

## Weaknesses
- Can go off-track if task is too vague
- May over-automate or take unintended actions
- Requires clear constraints to avoid breaking things

## Best for
- Implementing features in an existing codebase
- Writing and fixing tests
- Debugging reproducible issues
- Multi-step coding tasks with clear scope

## Avoid when
- You need high-level architecture thinking
- Requirements are unclear or exploratory
- You haven’t defined file boundaries or constraints

## Prompt Formula
Goal + Context + Constraints + Verification

## Example Good Prompt
"Add unit tests for userService.js. Only modify test files. Use existing test framework. Ensure all edge cases are covered and tests pass."

## Failure Patterns
- Modifies unrelated files
- Assumes incorrect project structure
- Skips validation steps
- Hallucinates missing dependencies

## Key Principles
- Break tasks into smaller steps → better results :contentReference[oaicite:0]{index=0}
- Always include verification (tests, lint, run checks) :contentReference[oaicite:1]{index=1}
- Treat Codex like a teammate, not a one-shot tool :contentReference[oaicite:2]{index=2}
- You are the reviewer, not the coder :contentReference[oaicite:3]{index=3}

## Related
[[Implementation Prompt Template]]
[[Failure Mode - Over-broad Edits]]
[[Decision Rules - Model Selection]]