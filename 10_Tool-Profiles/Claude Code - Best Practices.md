---
type: tool-profile
tool: claude-code
tags:
  - coding-agent
  - prompting
use_cases:
  - implementation
  - refactor
confidence: high
last_reviewed: 2026-04-18
---

## Strengths
- Excellent at multi-step coding tasks
- Good at following structured instructions

## Weaknesses
- Can overreach and modify too much code
- Sometimes assumes missing context

## Best for
- Implementing scoped features
- Refactoring existing code

## Avoid when
- Requirements are vague
- You need high-level architecture thinking

## Prompt Formula
Goal + Constraints + Files + Verification

## Example Good Prompt
"Implement user login using existing auth service. Only modify authController.js and tests. Add unit tests."

## Failure Patterns
- Edits unrelated files
- Hallucinates helper functions

## Related
[[Planning Prompt Template]]
[[Failure Mode - Hallucinated APIs]]